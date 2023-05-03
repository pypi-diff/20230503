# Comparing `tmp/argshell-1.1.0.tar.gz` & `tmp/argshell-1.2.0.tar.gz`

## Comparing `argshell-1.1.0.tar` & `argshell-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 argshell-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    34238 2020-02-02 00:00:00.000000 argshell-1.1.0/docs/argshell.html
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 argshell-1.1.0/docs/index.html
--rw-r--r--   0        0        0    37968 2020-02-02 00:00:00.000000 argshell-1.1.0/docs/search.js
--rw-r--r--   0        0        0   206454 2020-02-02 00:00:00.000000 argshell-1.1.0/docs/argshell/argshell.html
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 argshell-1.1.0/src/argshell/__init__.py
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 argshell-1.1.0/src/argshell/argshell.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 argshell-1.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 argshell-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 argshell-1.1.0/README.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argshell-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 argshell-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 argshell-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34238 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/argshell.html
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/index.html
+-rw-r--r--   0        0        0    38481 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/search.js
+-rw-r--r--   0        0        0   210283 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/argshell/argshell.html
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 argshell-1.2.0/src/argshell/__init__.py
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 argshell-1.2.0/src/argshell/argshell.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 argshell-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 argshell-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 argshell-1.2.0/README.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argshell-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 argshell-1.2.0/PKG-INFO
```

### Comparing `argshell-1.1.0/CHANGELOG.md` & `argshell-1.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `argshell-1.1.0/docs/argshell.html` & `argshell-1.2.0/docs/argshell.html`

 * *Files identical despite different names*

### Comparing `argshell-1.1.0/docs/search.js` & `argshell-1.2.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -742,14 +742,22 @@
         "modulename": "argshell.argshell",
         "qualname": "ArgShell.do_quit",
         "kind": "function",
         "doc": "<p>Quit shell.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">command</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "argshell.argshell.ArgShell.do_sys",
+        "modulename": "argshell.argshell",
+        "qualname": "ArgShell.do_sys",
+        "kind": "function",
+        "doc": "<p>Execute command with <code>os.system()</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">command</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "argshell.argshell.ArgShell.do_help",
         "modulename": "argshell.argshell",
         "qualname": "ArgShell.do_help",
         "kind": "function",
         "doc": "<p>List available commands with \"help\" or detailed help with \"help cmd\".\nIf using 'help cmd' and the cmd is decorated with a parser, the parser help will also be printed.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">arg</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
```

### Comparing `argshell-1.1.0/docs/argshell/argshell.html` & `argshell-1.2.0/docs/argshell/argshell.html`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
             <li>
                     <a class="class" href="#ArgShell">ArgShell</a>
                             <ul class="memberlist">
                         <li>
                                 <a class="function" href="#ArgShell.do_quit">do_quit</a>
                         </li>
                         <li>
+                                <a class="function" href="#ArgShell.do_sys">do_sys</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#ArgShell.do_help">do_help</a>
                         </li>
                         <li>
                                 <a class="function" href="#ArgShell.cmdloop">cmdloop</a>
                         </li>
                 </ul>
 
@@ -88,269 +91,274 @@
                 
                         <input id="mod-argshell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-argshell-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">cmd</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">shlex</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">sys</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">import</span> <span class="nn">traceback</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">functools</span> <span class="kn">import</span> <span class="n">wraps</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">shlex</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">import</span> <span class="nn">sys</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">import</span> <span class="nn">traceback</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">functools</span> <span class="kn">import</span> <span class="n">wraps</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="k">class</span> <span class="nc">Namespace</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="sd">&quot;&quot;&quot;Simple object for storing attributes.</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">    Implements equality by attribute names and values, and provides a simple string representation.&quot;&quot;&quot;</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="k">class</span> <span class="nc">Namespace</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="sd">&quot;&quot;&quot;Simple object for storing attributes.</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="sd">    Implements equality by attribute names and values, and provides a simple string representation.&quot;&quot;&quot;</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="k">class</span> <span class="nc">ArgShellParser</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">):</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="sd">&quot;&quot;&quot;***Overrides exit, error, and parse_args methods***</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    Object for parsing command line strings into Python objects.</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">    Keyword Arguments:</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="sd">        - prog -- The name of the program (default:</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">            ``os.path.basename(sys.argv[0])``)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="sd">        - usage -- A usage message (default: auto-generated from arguments)</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">        - description -- A description of what the program does</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="sd">        - epilog -- Text following the argument descriptions</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">        - parents -- Parsers whose arguments should be copied into this one</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">        - formatter_class -- HelpFormatter class for printing help messages</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">        - prefix_chars -- Characters that prefix optional arguments</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">        - fromfile_prefix_chars -- Characters that prefix files containing</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">            additional arguments</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">        - argument_default -- The default value for all arguments</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">        - conflict_handler -- String indicating how to handle conflicts</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">        - add_help -- Add a -h/-help option</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">        - allow_abbrev -- Allow long options to be abbreviated unambiguously</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">        - exit_on_error -- Determines whether or not ArgumentParser exits with</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">            error info when an error occurs</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="k">class</span> <span class="nc">ArgShellParser</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">):</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="sd">&quot;&quot;&quot;***Overrides exit, error, and parse_args methods***</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">    Object for parsing command line strings into Python objects.</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="sd">    Keyword Arguments:</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">        - prog -- The name of the program (default:</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="sd">            ``os.path.basename(sys.argv[0])``)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">        - usage -- A usage message (default: auto-generated from arguments)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="sd">        - description -- A description of what the program does</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">        - epilog -- Text following the argument descriptions</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">        - parents -- Parsers whose arguments should be copied into this one</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">        - formatter_class -- HelpFormatter class for printing help messages</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">        - prefix_chars -- Characters that prefix optional arguments</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">        - fromfile_prefix_chars -- Characters that prefix files containing</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">            additional arguments</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">        - argument_default -- The default value for all arguments</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">        - conflict_handler -- String indicating how to handle conflicts</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">        - add_help -- Add a -h/-help option</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">        - allow_abbrev -- Allow long options to be abbreviated unambiguously</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">        - exit_on_error -- Determines whether or not ArgumentParser exits with</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">            error info when an error occurs</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
 </span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="k">class</span> <span class="nc">ArgShell</span><span class="p">(</span><span class="n">cmd</span><span class="o">.</span><span class="n">Cmd</span><span class="p">):</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="sd">&quot;&quot;&quot;Subclass this to create custom ArgShells.&quot;&quot;&quot;</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Entering argshell...&quot;</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;argshell&gt;&quot;</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="c1"># XXX check arg syntax</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>                    <span class="c1"># =========================Modification start=========================</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>                        <span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>                        <span class="k">return</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                    <span class="k">pass</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>                <span class="k">return</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="n">func</span><span class="p">()</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                        <span class="k">continue</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">        the remainder of the line as argument.</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="k">class</span> <span class="nc">ArgShell</span><span class="p">(</span><span class="n">cmd</span><span class="o">.</span><span class="n">Cmd</span><span class="p">):</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="sd">&quot;&quot;&quot;Subclass this to create custom ArgShells.&quot;&quot;&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Entering argshell...&quot;</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;argshell&gt;&quot;</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">do_sys</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;Execute command with `os.system()`.&quot;&quot;&quot;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>            <span class="c1"># XXX check arg syntax</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>                    <span class="c1"># =========================Modification start=========================</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>                        <span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>                        <span class="k">return</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                    <span class="k">pass</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                <span class="k">return</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="n">func</span><span class="p">()</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>                        <span class="k">continue</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
 </span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">        the remainder of the line as argument.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                <span class="k">pass</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                <span class="c1"># ===========Modification start===========</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                <span class="c1"># ===========Modification stop===========</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="k">finally</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                    <span class="k">pass</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="k">pass</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>                <span class="c1"># ===========Modification start===========</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="c1"># ===========Modification stop===========</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
 </span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>                    <span class="k">pass</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>                        <span class="k">pass</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">return</span> <span class="n">inner</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>                        <span class="k">pass</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="k">return</span> <span class="n">inner</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Namespace">
                             <input id="Namespace-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -358,18 +366,18 @@
     <span class="def">class</span>
     <span class="name">Namespace</span><wbr>(<span class="base">argparse.Namespace</span>):
 
                 <label class="view-source-button" for="Namespace-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Namespace"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Namespace-11"><a href="#Namespace-11"><span class="linenos">11</span></a><span class="k">class</span> <span class="nc">Namespace</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="Namespace-12"><a href="#Namespace-12"><span class="linenos">12</span></a>    <span class="sd">&quot;&quot;&quot;Simple object for storing attributes.</span>
-</span><span id="Namespace-13"><a href="#Namespace-13"><span class="linenos">13</span></a>
-</span><span id="Namespace-14"><a href="#Namespace-14"><span class="linenos">14</span></a><span class="sd">    Implements equality by attribute names and values, and provides a simple string representation.&quot;&quot;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Namespace-12"><a href="#Namespace-12"><span class="linenos">12</span></a><span class="k">class</span> <span class="nc">Namespace</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="Namespace-13"><a href="#Namespace-13"><span class="linenos">13</span></a>    <span class="sd">&quot;&quot;&quot;Simple object for storing attributes.</span>
+</span><span id="Namespace-14"><a href="#Namespace-14"><span class="linenos">14</span></a>
+</span><span id="Namespace-15"><a href="#Namespace-15"><span class="linenos">15</span></a><span class="sd">    Implements equality by attribute names and values, and provides a simple string representation.&quot;&quot;&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Simple object for storing attributes.</p>
 
 <p>Implements equality by attribute names and values, and provides a simple string representation.</p>
 </div>
@@ -392,49 +400,49 @@
     <span class="def">class</span>
     <span class="name">ArgShellParser</span><wbr>(<span class="base">argparse.ArgumentParser</span>):
 
                 <label class="view-source-button" for="ArgShellParser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShellParser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser-17"><a href="#ArgShellParser-17"><span class="linenos">17</span></a><span class="k">class</span> <span class="nc">ArgShellParser</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">):</span>
-</span><span id="ArgShellParser-18"><a href="#ArgShellParser-18"><span class="linenos">18</span></a>    <span class="sd">&quot;&quot;&quot;***Overrides exit, error, and parse_args methods***</span>
-</span><span id="ArgShellParser-19"><a href="#ArgShellParser-19"><span class="linenos">19</span></a>
-</span><span id="ArgShellParser-20"><a href="#ArgShellParser-20"><span class="linenos">20</span></a><span class="sd">    Object for parsing command line strings into Python objects.</span>
-</span><span id="ArgShellParser-21"><a href="#ArgShellParser-21"><span class="linenos">21</span></a>
-</span><span id="ArgShellParser-22"><a href="#ArgShellParser-22"><span class="linenos">22</span></a><span class="sd">    Keyword Arguments:</span>
-</span><span id="ArgShellParser-23"><a href="#ArgShellParser-23"><span class="linenos">23</span></a><span class="sd">        - prog -- The name of the program (default:</span>
-</span><span id="ArgShellParser-24"><a href="#ArgShellParser-24"><span class="linenos">24</span></a><span class="sd">            ``os.path.basename(sys.argv[0])``)</span>
-</span><span id="ArgShellParser-25"><a href="#ArgShellParser-25"><span class="linenos">25</span></a><span class="sd">        - usage -- A usage message (default: auto-generated from arguments)</span>
-</span><span id="ArgShellParser-26"><a href="#ArgShellParser-26"><span class="linenos">26</span></a><span class="sd">        - description -- A description of what the program does</span>
-</span><span id="ArgShellParser-27"><a href="#ArgShellParser-27"><span class="linenos">27</span></a><span class="sd">        - epilog -- Text following the argument descriptions</span>
-</span><span id="ArgShellParser-28"><a href="#ArgShellParser-28"><span class="linenos">28</span></a><span class="sd">        - parents -- Parsers whose arguments should be copied into this one</span>
-</span><span id="ArgShellParser-29"><a href="#ArgShellParser-29"><span class="linenos">29</span></a><span class="sd">        - formatter_class -- HelpFormatter class for printing help messages</span>
-</span><span id="ArgShellParser-30"><a href="#ArgShellParser-30"><span class="linenos">30</span></a><span class="sd">        - prefix_chars -- Characters that prefix optional arguments</span>
-</span><span id="ArgShellParser-31"><a href="#ArgShellParser-31"><span class="linenos">31</span></a><span class="sd">        - fromfile_prefix_chars -- Characters that prefix files containing</span>
-</span><span id="ArgShellParser-32"><a href="#ArgShellParser-32"><span class="linenos">32</span></a><span class="sd">            additional arguments</span>
-</span><span id="ArgShellParser-33"><a href="#ArgShellParser-33"><span class="linenos">33</span></a><span class="sd">        - argument_default -- The default value for all arguments</span>
-</span><span id="ArgShellParser-34"><a href="#ArgShellParser-34"><span class="linenos">34</span></a><span class="sd">        - conflict_handler -- String indicating how to handle conflicts</span>
-</span><span id="ArgShellParser-35"><a href="#ArgShellParser-35"><span class="linenos">35</span></a><span class="sd">        - add_help -- Add a -h/-help option</span>
-</span><span id="ArgShellParser-36"><a href="#ArgShellParser-36"><span class="linenos">36</span></a><span class="sd">        - allow_abbrev -- Allow long options to be abbreviated unambiguously</span>
-</span><span id="ArgShellParser-37"><a href="#ArgShellParser-37"><span class="linenos">37</span></a><span class="sd">        - exit_on_error -- Determines whether or not ArgumentParser exits with</span>
-</span><span id="ArgShellParser-38"><a href="#ArgShellParser-38"><span class="linenos">38</span></a><span class="sd">            error info when an error occurs</span>
-</span><span id="ArgShellParser-39"><a href="#ArgShellParser-39"><span class="linenos">39</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="ArgShellParser-40"><a href="#ArgShellParser-40"><span class="linenos">40</span></a>
-</span><span id="ArgShellParser-41"><a href="#ArgShellParser-41"><span class="linenos">41</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="ArgShellParser-42"><a href="#ArgShellParser-42"><span class="linenos">42</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
-</span><span id="ArgShellParser-43"><a href="#ArgShellParser-43"><span class="linenos">43</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
-</span><span id="ArgShellParser-44"><a href="#ArgShellParser-44"><span class="linenos">44</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
-</span><span id="ArgShellParser-45"><a href="#ArgShellParser-45"><span class="linenos">45</span></a>
-</span><span id="ArgShellParser-46"><a href="#ArgShellParser-46"><span class="linenos">46</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
-</span><span id="ArgShellParser-47"><a href="#ArgShellParser-47"><span class="linenos">47</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ArgShellParser-48"><a href="#ArgShellParser-48"><span class="linenos">48</span></a>
-</span><span id="ArgShellParser-49"><a href="#ArgShellParser-49"><span class="linenos">49</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
-</span><span id="ArgShellParser-50"><a href="#ArgShellParser-50"><span class="linenos">50</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="ArgShellParser-51"><a href="#ArgShellParser-51"><span class="linenos">51</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser-18"><a href="#ArgShellParser-18"><span class="linenos">18</span></a><span class="k">class</span> <span class="nc">ArgShellParser</span><span class="p">(</span><span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">):</span>
+</span><span id="ArgShellParser-19"><a href="#ArgShellParser-19"><span class="linenos">19</span></a>    <span class="sd">&quot;&quot;&quot;***Overrides exit, error, and parse_args methods***</span>
+</span><span id="ArgShellParser-20"><a href="#ArgShellParser-20"><span class="linenos">20</span></a>
+</span><span id="ArgShellParser-21"><a href="#ArgShellParser-21"><span class="linenos">21</span></a><span class="sd">    Object for parsing command line strings into Python objects.</span>
+</span><span id="ArgShellParser-22"><a href="#ArgShellParser-22"><span class="linenos">22</span></a>
+</span><span id="ArgShellParser-23"><a href="#ArgShellParser-23"><span class="linenos">23</span></a><span class="sd">    Keyword Arguments:</span>
+</span><span id="ArgShellParser-24"><a href="#ArgShellParser-24"><span class="linenos">24</span></a><span class="sd">        - prog -- The name of the program (default:</span>
+</span><span id="ArgShellParser-25"><a href="#ArgShellParser-25"><span class="linenos">25</span></a><span class="sd">            ``os.path.basename(sys.argv[0])``)</span>
+</span><span id="ArgShellParser-26"><a href="#ArgShellParser-26"><span class="linenos">26</span></a><span class="sd">        - usage -- A usage message (default: auto-generated from arguments)</span>
+</span><span id="ArgShellParser-27"><a href="#ArgShellParser-27"><span class="linenos">27</span></a><span class="sd">        - description -- A description of what the program does</span>
+</span><span id="ArgShellParser-28"><a href="#ArgShellParser-28"><span class="linenos">28</span></a><span class="sd">        - epilog -- Text following the argument descriptions</span>
+</span><span id="ArgShellParser-29"><a href="#ArgShellParser-29"><span class="linenos">29</span></a><span class="sd">        - parents -- Parsers whose arguments should be copied into this one</span>
+</span><span id="ArgShellParser-30"><a href="#ArgShellParser-30"><span class="linenos">30</span></a><span class="sd">        - formatter_class -- HelpFormatter class for printing help messages</span>
+</span><span id="ArgShellParser-31"><a href="#ArgShellParser-31"><span class="linenos">31</span></a><span class="sd">        - prefix_chars -- Characters that prefix optional arguments</span>
+</span><span id="ArgShellParser-32"><a href="#ArgShellParser-32"><span class="linenos">32</span></a><span class="sd">        - fromfile_prefix_chars -- Characters that prefix files containing</span>
+</span><span id="ArgShellParser-33"><a href="#ArgShellParser-33"><span class="linenos">33</span></a><span class="sd">            additional arguments</span>
+</span><span id="ArgShellParser-34"><a href="#ArgShellParser-34"><span class="linenos">34</span></a><span class="sd">        - argument_default -- The default value for all arguments</span>
+</span><span id="ArgShellParser-35"><a href="#ArgShellParser-35"><span class="linenos">35</span></a><span class="sd">        - conflict_handler -- String indicating how to handle conflicts</span>
+</span><span id="ArgShellParser-36"><a href="#ArgShellParser-36"><span class="linenos">36</span></a><span class="sd">        - add_help -- Add a -h/-help option</span>
+</span><span id="ArgShellParser-37"><a href="#ArgShellParser-37"><span class="linenos">37</span></a><span class="sd">        - allow_abbrev -- Allow long options to be abbreviated unambiguously</span>
+</span><span id="ArgShellParser-38"><a href="#ArgShellParser-38"><span class="linenos">38</span></a><span class="sd">        - exit_on_error -- Determines whether or not ArgumentParser exits with</span>
+</span><span id="ArgShellParser-39"><a href="#ArgShellParser-39"><span class="linenos">39</span></a><span class="sd">            error info when an error occurs</span>
+</span><span id="ArgShellParser-40"><a href="#ArgShellParser-40"><span class="linenos">40</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="ArgShellParser-41"><a href="#ArgShellParser-41"><span class="linenos">41</span></a>
+</span><span id="ArgShellParser-42"><a href="#ArgShellParser-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="ArgShellParser-43"><a href="#ArgShellParser-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
+</span><span id="ArgShellParser-44"><a href="#ArgShellParser-44"><span class="linenos">44</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
+</span><span id="ArgShellParser-45"><a href="#ArgShellParser-45"><span class="linenos">45</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+</span><span id="ArgShellParser-46"><a href="#ArgShellParser-46"><span class="linenos">46</span></a>
+</span><span id="ArgShellParser-47"><a href="#ArgShellParser-47"><span class="linenos">47</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
+</span><span id="ArgShellParser-48"><a href="#ArgShellParser-48"><span class="linenos">48</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ArgShellParser-49"><a href="#ArgShellParser-49"><span class="linenos">49</span></a>
+</span><span id="ArgShellParser-50"><a href="#ArgShellParser-50"><span class="linenos">50</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
+</span><span id="ArgShellParser-51"><a href="#ArgShellParser-51"><span class="linenos">51</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="ArgShellParser-52"><a href="#ArgShellParser-52"><span class="linenos">52</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
 </span></pre></div>
 
 
             <div class="docstring"><p><strong><em>Overrides exit, error, and parse_args methods</em></strong></p>
 
 <p>Object for parsing command line strings into Python objects.</p>
 
@@ -465,18 +473,18 @@
         <span class="def">def</span>
         <span class="name">exit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">status</span><span class="o">=</span><span class="mi">0</span>, </span><span class="param"><span class="n">message</span><span class="o">=</span><span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ArgShellParser.exit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShellParser.exit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.exit-41"><a href="#ArgShellParser.exit-41"><span class="linenos">41</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="ArgShellParser.exit-42"><a href="#ArgShellParser.exit-42"><span class="linenos">42</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
-</span><span id="ArgShellParser.exit-43"><a href="#ArgShellParser.exit-43"><span class="linenos">43</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
-</span><span id="ArgShellParser.exit-44"><a href="#ArgShellParser.exit-44"><span class="linenos">44</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.exit-42"><a href="#ArgShellParser.exit-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">exit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">status</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">message</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="ArgShellParser.exit-43"><a href="#ArgShellParser.exit-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Override to prevent shell exit when passing -h/--help switches.&quot;&quot;&quot;</span>
+</span><span id="ArgShellParser.exit-44"><a href="#ArgShellParser.exit-44"><span class="linenos">44</span></a>        <span class="k">if</span> <span class="n">message</span><span class="p">:</span>
+</span><span id="ArgShellParser.exit-45"><a href="#ArgShellParser.exit-45"><span class="linenos">45</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_print_message</span><span class="p">(</span><span class="n">message</span><span class="p">,</span> <span class="n">sys</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Override to prevent shell exit when passing -h/--help switches.</p>
 </div>
 
 
@@ -488,16 +496,16 @@
         <span class="def">def</span>
         <span class="name">error</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ArgShellParser.error-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShellParser.error"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.error-46"><a href="#ArgShellParser.error-46"><span class="linenos">46</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
-</span><span id="ArgShellParser.error-47"><a href="#ArgShellParser.error-47"><span class="linenos">47</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.error-47"><a href="#ArgShellParser.error-47"><span class="linenos">47</span></a>    <span class="k">def</span> <span class="nf">error</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">):</span>
+</span><span id="ArgShellParser.error-48"><a href="#ArgShellParser.error-48"><span class="linenos">48</span></a>        <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;prog: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prog</span><span class="si">}</span><span class="s2">, message: </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>error(message: string)</p>
 
 <p>Prints a usage message incorporating the message to stderr and
 exits.</p>
@@ -515,17 +523,17 @@
         <span class="def">def</span>
         <span class="name">parse_args</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="o">*</span><span class="n">args</span>, </span><span class="param"><span class="o">**</span><span class="n">kwargs</span></span><span class="return-annotation">) -> <span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span>:</span></span>
 
                 <label class="view-source-button" for="ArgShellParser.parse_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShellParser.parse_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.parse_args-49"><a href="#ArgShellParser.parse_args-49"><span class="linenos">49</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
-</span><span id="ArgShellParser.parse_args-50"><a href="#ArgShellParser.parse_args-50"><span class="linenos">50</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="ArgShellParser.parse_args-51"><a href="#ArgShellParser.parse_args-51"><span class="linenos">51</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShellParser.parse_args-50"><a href="#ArgShellParser.parse_args-50"><span class="linenos">50</span></a>    <span class="k">def</span> <span class="nf">parse_args</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Namespace</span><span class="p">:</span>
+</span><span id="ArgShellParser.parse_args-51"><a href="#ArgShellParser.parse_args-51"><span class="linenos">51</span></a>        <span class="n">parsed_args</span><span class="p">:</span> <span class="n">Namespace</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="ArgShellParser.parse_args-52"><a href="#ArgShellParser.parse_args-52"><span class="linenos">52</span></a>        <span class="k">return</span> <span class="n">parsed_args</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div class="inherited">
@@ -563,138 +571,142 @@
     <span class="def">class</span>
     <span class="name">ArgShell</span><wbr>(<span class="base">cmd.Cmd</span>):
 
                 <label class="view-source-button" for="ArgShell-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShell"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell-54"><a href="#ArgShell-54"><span class="linenos"> 54</span></a><span class="k">class</span> <span class="nc">ArgShell</span><span class="p">(</span><span class="n">cmd</span><span class="o">.</span><span class="n">Cmd</span><span class="p">):</span>
-</span><span id="ArgShell-55"><a href="#ArgShell-55"><span class="linenos"> 55</span></a>    <span class="sd">&quot;&quot;&quot;Subclass this to create custom ArgShells.&quot;&quot;&quot;</span>
-</span><span id="ArgShell-56"><a href="#ArgShell-56"><span class="linenos"> 56</span></a>
-</span><span id="ArgShell-57"><a href="#ArgShell-57"><span class="linenos"> 57</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Entering argshell...&quot;</span>
-</span><span id="ArgShell-58"><a href="#ArgShell-58"><span class="linenos"> 58</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;argshell&gt;&quot;</span>
-</span><span id="ArgShell-59"><a href="#ArgShell-59"><span class="linenos"> 59</span></a>
-</span><span id="ArgShell-60"><a href="#ArgShell-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="ArgShell-61"><a href="#ArgShell-61"><span class="linenos"> 61</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
-</span><span id="ArgShell-62"><a href="#ArgShell-62"><span class="linenos"> 62</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="ArgShell-63"><a href="#ArgShell-63"><span class="linenos"> 63</span></a>
-</span><span id="ArgShell-64"><a href="#ArgShell-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
-</span><span id="ArgShell-65"><a href="#ArgShell-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
-</span><span id="ArgShell-66"><a href="#ArgShell-66"><span class="linenos"> 66</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
-</span><span id="ArgShell-67"><a href="#ArgShell-67"><span class="linenos"> 67</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="ArgShell-68"><a href="#ArgShell-68"><span class="linenos"> 68</span></a>            <span class="c1"># XXX check arg syntax</span>
-</span><span id="ArgShell-69"><a href="#ArgShell-69"><span class="linenos"> 69</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-70"><a href="#ArgShell-70"><span class="linenos"> 70</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="ArgShell-71"><a href="#ArgShell-71"><span class="linenos"> 71</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="ArgShell-72"><a href="#ArgShell-72"><span class="linenos"> 72</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-73"><a href="#ArgShell-73"><span class="linenos"> 73</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="ArgShell-74"><a href="#ArgShell-74"><span class="linenos"> 74</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
-</span><span id="ArgShell-75"><a href="#ArgShell-75"><span class="linenos"> 75</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
-</span><span id="ArgShell-76"><a href="#ArgShell-76"><span class="linenos"> 76</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
-</span><span id="ArgShell-77"><a href="#ArgShell-77"><span class="linenos"> 77</span></a>                    <span class="c1"># =========================Modification start=========================</span>
-</span><span id="ArgShell-78"><a href="#ArgShell-78"><span class="linenos"> 78</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
-</span><span id="ArgShell-79"><a href="#ArgShell-79"><span class="linenos"> 79</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="ArgShell-80"><a href="#ArgShell-80"><span class="linenos"> 80</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
-</span><span id="ArgShell-81"><a href="#ArgShell-81"><span class="linenos"> 81</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="ArgShell-82"><a href="#ArgShell-82"><span class="linenos"> 82</span></a>                        <span class="p">)</span>
-</span><span id="ArgShell-83"><a href="#ArgShell-83"><span class="linenos"> 83</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
-</span><span id="ArgShell-84"><a href="#ArgShell-84"><span class="linenos"> 84</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="ArgShell-85"><a href="#ArgShell-85"><span class="linenos"> 85</span></a>                        <span class="k">return</span>
-</span><span id="ArgShell-86"><a href="#ArgShell-86"><span class="linenos"> 86</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
-</span><span id="ArgShell-87"><a href="#ArgShell-87"><span class="linenos"> 87</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="ArgShell-88"><a href="#ArgShell-88"><span class="linenos"> 88</span></a>                    <span class="k">pass</span>
-</span><span id="ArgShell-89"><a href="#ArgShell-89"><span class="linenos"> 89</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
-</span><span id="ArgShell-90"><a href="#ArgShell-90"><span class="linenos"> 90</span></a>                <span class="k">return</span>
-</span><span id="ArgShell-91"><a href="#ArgShell-91"><span class="linenos"> 91</span></a>            <span class="n">func</span><span class="p">()</span>
-</span><span id="ArgShell-92"><a href="#ArgShell-92"><span class="linenos"> 92</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell-93"><a href="#ArgShell-93"><span class="linenos"> 93</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
-</span><span id="ArgShell-94"><a href="#ArgShell-94"><span class="linenos"> 94</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="ArgShell-95"><a href="#ArgShell-95"><span class="linenos"> 95</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="ArgShell-96"><a href="#ArgShell-96"><span class="linenos"> 96</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
-</span><span id="ArgShell-97"><a href="#ArgShell-97"><span class="linenos"> 97</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="ArgShell-98"><a href="#ArgShell-98"><span class="linenos"> 98</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
-</span><span id="ArgShell-99"><a href="#ArgShell-99"><span class="linenos"> 99</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
-</span><span id="ArgShell-100"><a href="#ArgShell-100"><span class="linenos">100</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="ArgShell-101"><a href="#ArgShell-101"><span class="linenos">101</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
-</span><span id="ArgShell-102"><a href="#ArgShell-102"><span class="linenos">102</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ArgShell-103"><a href="#ArgShell-103"><span class="linenos">103</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="ArgShell-104"><a href="#ArgShell-104"><span class="linenos">104</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
-</span><span id="ArgShell-105"><a href="#ArgShell-105"><span class="linenos">105</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
-</span><span id="ArgShell-106"><a href="#ArgShell-106"><span class="linenos">106</span></a>                        <span class="k">continue</span>
-</span><span id="ArgShell-107"><a href="#ArgShell-107"><span class="linenos">107</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
-</span><span id="ArgShell-108"><a href="#ArgShell-108"><span class="linenos">108</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
-</span><span id="ArgShell-109"><a href="#ArgShell-109"><span class="linenos">109</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
-</span><span id="ArgShell-110"><a href="#ArgShell-110"><span class="linenos">110</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell-111"><a href="#ArgShell-111"><span class="linenos">111</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell-112"><a href="#ArgShell-112"><span class="linenos">112</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
-</span><span id="ArgShell-113"><a href="#ArgShell-113"><span class="linenos">113</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell-114"><a href="#ArgShell-114"><span class="linenos">114</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell-115"><a href="#ArgShell-115"><span class="linenos">115</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell-116"><a href="#ArgShell-116"><span class="linenos">116</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
-</span><span id="ArgShell-117"><a href="#ArgShell-117"><span class="linenos">117</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="ArgShell-118"><a href="#ArgShell-118"><span class="linenos">118</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="ArgShell-119"><a href="#ArgShell-119"><span class="linenos">119</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="ArgShell-120"><a href="#ArgShell-120"><span class="linenos">120</span></a>
-</span><span id="ArgShell-121"><a href="#ArgShell-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="ArgShell-122"><a href="#ArgShell-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
-</span><span id="ArgShell-123"><a href="#ArgShell-123"><span class="linenos">123</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
-</span><span id="ArgShell-124"><a href="#ArgShell-124"><span class="linenos">124</span></a><span class="sd">        the remainder of the line as argument.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell-55"><a href="#ArgShell-55"><span class="linenos"> 55</span></a><span class="k">class</span> <span class="nc">ArgShell</span><span class="p">(</span><span class="n">cmd</span><span class="o">.</span><span class="n">Cmd</span><span class="p">):</span>
+</span><span id="ArgShell-56"><a href="#ArgShell-56"><span class="linenos"> 56</span></a>    <span class="sd">&quot;&quot;&quot;Subclass this to create custom ArgShells.&quot;&quot;&quot;</span>
+</span><span id="ArgShell-57"><a href="#ArgShell-57"><span class="linenos"> 57</span></a>
+</span><span id="ArgShell-58"><a href="#ArgShell-58"><span class="linenos"> 58</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Entering argshell...&quot;</span>
+</span><span id="ArgShell-59"><a href="#ArgShell-59"><span class="linenos"> 59</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;argshell&gt;&quot;</span>
+</span><span id="ArgShell-60"><a href="#ArgShell-60"><span class="linenos"> 60</span></a>
+</span><span id="ArgShell-61"><a href="#ArgShell-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="ArgShell-62"><a href="#ArgShell-62"><span class="linenos"> 62</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
+</span><span id="ArgShell-63"><a href="#ArgShell-63"><span class="linenos"> 63</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="ArgShell-64"><a href="#ArgShell-64"><span class="linenos"> 64</span></a>
+</span><span id="ArgShell-65"><a href="#ArgShell-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">do_sys</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="ArgShell-66"><a href="#ArgShell-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Execute command with `os.system()`.&quot;&quot;&quot;</span>
+</span><span id="ArgShell-67"><a href="#ArgShell-67"><span class="linenos"> 67</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="ArgShell-68"><a href="#ArgShell-68"><span class="linenos"> 68</span></a>
+</span><span id="ArgShell-69"><a href="#ArgShell-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
+</span><span id="ArgShell-70"><a href="#ArgShell-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
+</span><span id="ArgShell-71"><a href="#ArgShell-71"><span class="linenos"> 71</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
+</span><span id="ArgShell-72"><a href="#ArgShell-72"><span class="linenos"> 72</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="ArgShell-73"><a href="#ArgShell-73"><span class="linenos"> 73</span></a>            <span class="c1"># XXX check arg syntax</span>
+</span><span id="ArgShell-74"><a href="#ArgShell-74"><span class="linenos"> 74</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-75"><a href="#ArgShell-75"><span class="linenos"> 75</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="ArgShell-76"><a href="#ArgShell-76"><span class="linenos"> 76</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="ArgShell-77"><a href="#ArgShell-77"><span class="linenos"> 77</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-78"><a href="#ArgShell-78"><span class="linenos"> 78</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="ArgShell-79"><a href="#ArgShell-79"><span class="linenos"> 79</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
+</span><span id="ArgShell-80"><a href="#ArgShell-80"><span class="linenos"> 80</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
+</span><span id="ArgShell-81"><a href="#ArgShell-81"><span class="linenos"> 81</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
+</span><span id="ArgShell-82"><a href="#ArgShell-82"><span class="linenos"> 82</span></a>                    <span class="c1"># =========================Modification start=========================</span>
+</span><span id="ArgShell-83"><a href="#ArgShell-83"><span class="linenos"> 83</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
+</span><span id="ArgShell-84"><a href="#ArgShell-84"><span class="linenos"> 84</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="ArgShell-85"><a href="#ArgShell-85"><span class="linenos"> 85</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
+</span><span id="ArgShell-86"><a href="#ArgShell-86"><span class="linenos"> 86</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="ArgShell-87"><a href="#ArgShell-87"><span class="linenos"> 87</span></a>                        <span class="p">)</span>
+</span><span id="ArgShell-88"><a href="#ArgShell-88"><span class="linenos"> 88</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
+</span><span id="ArgShell-89"><a href="#ArgShell-89"><span class="linenos"> 89</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="ArgShell-90"><a href="#ArgShell-90"><span class="linenos"> 90</span></a>                        <span class="k">return</span>
+</span><span id="ArgShell-91"><a href="#ArgShell-91"><span class="linenos"> 91</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
+</span><span id="ArgShell-92"><a href="#ArgShell-92"><span class="linenos"> 92</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="ArgShell-93"><a href="#ArgShell-93"><span class="linenos"> 93</span></a>                    <span class="k">pass</span>
+</span><span id="ArgShell-94"><a href="#ArgShell-94"><span class="linenos"> 94</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
+</span><span id="ArgShell-95"><a href="#ArgShell-95"><span class="linenos"> 95</span></a>                <span class="k">return</span>
+</span><span id="ArgShell-96"><a href="#ArgShell-96"><span class="linenos"> 96</span></a>            <span class="n">func</span><span class="p">()</span>
+</span><span id="ArgShell-97"><a href="#ArgShell-97"><span class="linenos"> 97</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell-98"><a href="#ArgShell-98"><span class="linenos"> 98</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
+</span><span id="ArgShell-99"><a href="#ArgShell-99"><span class="linenos"> 99</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="ArgShell-100"><a href="#ArgShell-100"><span class="linenos">100</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="ArgShell-101"><a href="#ArgShell-101"><span class="linenos">101</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
+</span><span id="ArgShell-102"><a href="#ArgShell-102"><span class="linenos">102</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="ArgShell-103"><a href="#ArgShell-103"><span class="linenos">103</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
+</span><span id="ArgShell-104"><a href="#ArgShell-104"><span class="linenos">104</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
+</span><span id="ArgShell-105"><a href="#ArgShell-105"><span class="linenos">105</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="ArgShell-106"><a href="#ArgShell-106"><span class="linenos">106</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
+</span><span id="ArgShell-107"><a href="#ArgShell-107"><span class="linenos">107</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ArgShell-108"><a href="#ArgShell-108"><span class="linenos">108</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="ArgShell-109"><a href="#ArgShell-109"><span class="linenos">109</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
+</span><span id="ArgShell-110"><a href="#ArgShell-110"><span class="linenos">110</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
+</span><span id="ArgShell-111"><a href="#ArgShell-111"><span class="linenos">111</span></a>                        <span class="k">continue</span>
+</span><span id="ArgShell-112"><a href="#ArgShell-112"><span class="linenos">112</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
+</span><span id="ArgShell-113"><a href="#ArgShell-113"><span class="linenos">113</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
+</span><span id="ArgShell-114"><a href="#ArgShell-114"><span class="linenos">114</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
+</span><span id="ArgShell-115"><a href="#ArgShell-115"><span class="linenos">115</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell-116"><a href="#ArgShell-116"><span class="linenos">116</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell-117"><a href="#ArgShell-117"><span class="linenos">117</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
+</span><span id="ArgShell-118"><a href="#ArgShell-118"><span class="linenos">118</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell-119"><a href="#ArgShell-119"><span class="linenos">119</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell-120"><a href="#ArgShell-120"><span class="linenos">120</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell-121"><a href="#ArgShell-121"><span class="linenos">121</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
+</span><span id="ArgShell-122"><a href="#ArgShell-122"><span class="linenos">122</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="ArgShell-123"><a href="#ArgShell-123"><span class="linenos">123</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="ArgShell-124"><a href="#ArgShell-124"><span class="linenos">124</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
 </span><span id="ArgShell-125"><a href="#ArgShell-125"><span class="linenos">125</span></a>
-</span><span id="ArgShell-126"><a href="#ArgShell-126"><span class="linenos">126</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="ArgShell-127"><a href="#ArgShell-127"><span class="linenos">127</span></a>
-</span><span id="ArgShell-128"><a href="#ArgShell-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
-</span><span id="ArgShell-129"><a href="#ArgShell-129"><span class="linenos">129</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="ArgShell-130"><a href="#ArgShell-130"><span class="linenos">130</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-131"><a href="#ArgShell-131"><span class="linenos">131</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="ArgShell-126"><a href="#ArgShell-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="ArgShell-127"><a href="#ArgShell-127"><span class="linenos">127</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
+</span><span id="ArgShell-128"><a href="#ArgShell-128"><span class="linenos">128</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
+</span><span id="ArgShell-129"><a href="#ArgShell-129"><span class="linenos">129</span></a><span class="sd">        the remainder of the line as argument.</span>
+</span><span id="ArgShell-130"><a href="#ArgShell-130"><span class="linenos">130</span></a>
+</span><span id="ArgShell-131"><a href="#ArgShell-131"><span class="linenos">131</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="ArgShell-132"><a href="#ArgShell-132"><span class="linenos">132</span></a>
-</span><span id="ArgShell-133"><a href="#ArgShell-133"><span class="linenos">133</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell-134"><a href="#ArgShell-134"><span class="linenos">134</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell-135"><a href="#ArgShell-135"><span class="linenos">135</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell-136"><a href="#ArgShell-136"><span class="linenos">136</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="ArgShell-137"><a href="#ArgShell-137"><span class="linenos">137</span></a>                <span class="k">pass</span>
-</span><span id="ArgShell-138"><a href="#ArgShell-138"><span class="linenos">138</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-139"><a href="#ArgShell-139"><span class="linenos">139</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ArgShell-140"><a href="#ArgShell-140"><span class="linenos">140</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
-</span><span id="ArgShell-141"><a href="#ArgShell-141"><span class="linenos">141</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
-</span><span id="ArgShell-142"><a href="#ArgShell-142"><span class="linenos">142</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ArgShell-143"><a href="#ArgShell-143"><span class="linenos">143</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="ArgShell-144"><a href="#ArgShell-144"><span class="linenos">144</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
-</span><span id="ArgShell-145"><a href="#ArgShell-145"><span class="linenos">145</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
-</span><span id="ArgShell-146"><a href="#ArgShell-146"><span class="linenos">146</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="ArgShell-147"><a href="#ArgShell-147"><span class="linenos">147</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell-148"><a href="#ArgShell-148"><span class="linenos">148</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
-</span><span id="ArgShell-149"><a href="#ArgShell-149"><span class="linenos">149</span></a>                        <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-150"><a href="#ArgShell-150"><span class="linenos">150</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="ArgShell-151"><a href="#ArgShell-151"><span class="linenos">151</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
-</span><span id="ArgShell-152"><a href="#ArgShell-152"><span class="linenos">152</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="ArgShell-153"><a href="#ArgShell-153"><span class="linenos">153</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell-154"><a href="#ArgShell-154"><span class="linenos">154</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="ArgShell-155"><a href="#ArgShell-155"><span class="linenos">155</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
-</span><span id="ArgShell-156"><a href="#ArgShell-156"><span class="linenos">156</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
-</span><span id="ArgShell-157"><a href="#ArgShell-157"><span class="linenos">157</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
-</span><span id="ArgShell-158"><a href="#ArgShell-158"><span class="linenos">158</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="ArgShell-159"><a href="#ArgShell-159"><span class="linenos">159</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell-160"><a href="#ArgShell-160"><span class="linenos">160</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ArgShell-161"><a href="#ArgShell-161"><span class="linenos">161</span></a>                <span class="c1"># ===========Modification start===========</span>
-</span><span id="ArgShell-162"><a href="#ArgShell-162"><span class="linenos">162</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-163"><a href="#ArgShell-163"><span class="linenos">163</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell-164"><a href="#ArgShell-164"><span class="linenos">164</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell-165"><a href="#ArgShell-165"><span class="linenos">165</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell-166"><a href="#ArgShell-166"><span class="linenos">166</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="ArgShell-167"><a href="#ArgShell-167"><span class="linenos">167</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
-</span><span id="ArgShell-168"><a href="#ArgShell-168"><span class="linenos">168</span></a>                <span class="c1"># ===========Modification stop===========</span>
-</span><span id="ArgShell-169"><a href="#ArgShell-169"><span class="linenos">169</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
-</span><span id="ArgShell-170"><a href="#ArgShell-170"><span class="linenos">170</span></a>        <span class="k">finally</span><span class="p">:</span>
-</span><span id="ArgShell-171"><a href="#ArgShell-171"><span class="linenos">171</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="ArgShell-172"><a href="#ArgShell-172"><span class="linenos">172</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell-173"><a href="#ArgShell-173"><span class="linenos">173</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
-</span><span id="ArgShell-174"><a href="#ArgShell-174"><span class="linenos">174</span></a>
-</span><span id="ArgShell-175"><a href="#ArgShell-175"><span class="linenos">175</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell-176"><a href="#ArgShell-176"><span class="linenos">176</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="ArgShell-177"><a href="#ArgShell-177"><span class="linenos">177</span></a>                    <span class="k">pass</span>
+</span><span id="ArgShell-133"><a href="#ArgShell-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
+</span><span id="ArgShell-134"><a href="#ArgShell-134"><span class="linenos">134</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="ArgShell-135"><a href="#ArgShell-135"><span class="linenos">135</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-136"><a href="#ArgShell-136"><span class="linenos">136</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="ArgShell-137"><a href="#ArgShell-137"><span class="linenos">137</span></a>
+</span><span id="ArgShell-138"><a href="#ArgShell-138"><span class="linenos">138</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell-139"><a href="#ArgShell-139"><span class="linenos">139</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell-140"><a href="#ArgShell-140"><span class="linenos">140</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell-141"><a href="#ArgShell-141"><span class="linenos">141</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="ArgShell-142"><a href="#ArgShell-142"><span class="linenos">142</span></a>                <span class="k">pass</span>
+</span><span id="ArgShell-143"><a href="#ArgShell-143"><span class="linenos">143</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-144"><a href="#ArgShell-144"><span class="linenos">144</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ArgShell-145"><a href="#ArgShell-145"><span class="linenos">145</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
+</span><span id="ArgShell-146"><a href="#ArgShell-146"><span class="linenos">146</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
+</span><span id="ArgShell-147"><a href="#ArgShell-147"><span class="linenos">147</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ArgShell-148"><a href="#ArgShell-148"><span class="linenos">148</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="ArgShell-149"><a href="#ArgShell-149"><span class="linenos">149</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
+</span><span id="ArgShell-150"><a href="#ArgShell-150"><span class="linenos">150</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
+</span><span id="ArgShell-151"><a href="#ArgShell-151"><span class="linenos">151</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="ArgShell-152"><a href="#ArgShell-152"><span class="linenos">152</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell-153"><a href="#ArgShell-153"><span class="linenos">153</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
+</span><span id="ArgShell-154"><a href="#ArgShell-154"><span class="linenos">154</span></a>                        <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-155"><a href="#ArgShell-155"><span class="linenos">155</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="ArgShell-156"><a href="#ArgShell-156"><span class="linenos">156</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
+</span><span id="ArgShell-157"><a href="#ArgShell-157"><span class="linenos">157</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="ArgShell-158"><a href="#ArgShell-158"><span class="linenos">158</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell-159"><a href="#ArgShell-159"><span class="linenos">159</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="ArgShell-160"><a href="#ArgShell-160"><span class="linenos">160</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
+</span><span id="ArgShell-161"><a href="#ArgShell-161"><span class="linenos">161</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
+</span><span id="ArgShell-162"><a href="#ArgShell-162"><span class="linenos">162</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
+</span><span id="ArgShell-163"><a href="#ArgShell-163"><span class="linenos">163</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="ArgShell-164"><a href="#ArgShell-164"><span class="linenos">164</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell-165"><a href="#ArgShell-165"><span class="linenos">165</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ArgShell-166"><a href="#ArgShell-166"><span class="linenos">166</span></a>                <span class="c1"># ===========Modification start===========</span>
+</span><span id="ArgShell-167"><a href="#ArgShell-167"><span class="linenos">167</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-168"><a href="#ArgShell-168"><span class="linenos">168</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell-169"><a href="#ArgShell-169"><span class="linenos">169</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell-170"><a href="#ArgShell-170"><span class="linenos">170</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell-171"><a href="#ArgShell-171"><span class="linenos">171</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="ArgShell-172"><a href="#ArgShell-172"><span class="linenos">172</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
+</span><span id="ArgShell-173"><a href="#ArgShell-173"><span class="linenos">173</span></a>                <span class="c1"># ===========Modification stop===========</span>
+</span><span id="ArgShell-174"><a href="#ArgShell-174"><span class="linenos">174</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
+</span><span id="ArgShell-175"><a href="#ArgShell-175"><span class="linenos">175</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="ArgShell-176"><a href="#ArgShell-176"><span class="linenos">176</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="ArgShell-177"><a href="#ArgShell-177"><span class="linenos">177</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell-178"><a href="#ArgShell-178"><span class="linenos">178</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="ArgShell-179"><a href="#ArgShell-179"><span class="linenos">179</span></a>
+</span><span id="ArgShell-180"><a href="#ArgShell-180"><span class="linenos">180</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell-181"><a href="#ArgShell-181"><span class="linenos">181</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="ArgShell-182"><a href="#ArgShell-182"><span class="linenos">182</span></a>                    <span class="k">pass</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -705,92 +717,114 @@
         <span class="def">def</span>
         <span class="name">do_quit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ArgShell.do_quit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShell.do_quit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.do_quit-60"><a href="#ArgShell.do_quit-60"><span class="linenos">60</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="ArgShell.do_quit-61"><a href="#ArgShell.do_quit-61"><span class="linenos">61</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
-</span><span id="ArgShell.do_quit-62"><a href="#ArgShell.do_quit-62"><span class="linenos">62</span></a>        <span class="k">return</span> <span class="kc">True</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.do_quit-61"><a href="#ArgShell.do_quit-61"><span class="linenos">61</span></a>    <span class="k">def</span> <span class="nf">do_quit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="ArgShell.do_quit-62"><a href="#ArgShell.do_quit-62"><span class="linenos">62</span></a>        <span class="sd">&quot;&quot;&quot;Quit shell.&quot;&quot;&quot;</span>
+</span><span id="ArgShell.do_quit-63"><a href="#ArgShell.do_quit-63"><span class="linenos">63</span></a>        <span class="k">return</span> <span class="kc">True</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Quit shell.</p>
 </div>
 
 
                             </div>
+                            <div id="ArgShell.do_sys" class="classattr">
+                                        <input id="ArgShell.do_sys-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">do_sys</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="ArgShell.do_sys-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#ArgShell.do_sys"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.do_sys-65"><a href="#ArgShell.do_sys-65"><span class="linenos">65</span></a>    <span class="k">def</span> <span class="nf">do_sys</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="ArgShell.do_sys-66"><a href="#ArgShell.do_sys-66"><span class="linenos">66</span></a>        <span class="sd">&quot;&quot;&quot;Execute command with `os.system()`.&quot;&quot;&quot;</span>
+</span><span id="ArgShell.do_sys-67"><a href="#ArgShell.do_sys-67"><span class="linenos">67</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Execute command with <code>os.system()</code>.</p>
+</div>
+
+
+                            </div>
                             <div id="ArgShell.do_help" class="classattr">
                                         <input id="ArgShell.do_help-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">do_help</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ArgShell.do_help-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShell.do_help"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.do_help-64"><a href="#ArgShell.do_help-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
-</span><span id="ArgShell.do_help-65"><a href="#ArgShell.do_help-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
-</span><span id="ArgShell.do_help-66"><a href="#ArgShell.do_help-66"><span class="linenos"> 66</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
-</span><span id="ArgShell.do_help-67"><a href="#ArgShell.do_help-67"><span class="linenos"> 67</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-68"><a href="#ArgShell.do_help-68"><span class="linenos"> 68</span></a>            <span class="c1"># XXX check arg syntax</span>
-</span><span id="ArgShell.do_help-69"><a href="#ArgShell.do_help-69"><span class="linenos"> 69</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-70"><a href="#ArgShell.do_help-70"><span class="linenos"> 70</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-71"><a href="#ArgShell.do_help-71"><span class="linenos"> 71</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-72"><a href="#ArgShell.do_help-72"><span class="linenos"> 72</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-73"><a href="#ArgShell.do_help-73"><span class="linenos"> 73</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-74"><a href="#ArgShell.do_help-74"><span class="linenos"> 74</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
-</span><span id="ArgShell.do_help-75"><a href="#ArgShell.do_help-75"><span class="linenos"> 75</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-76"><a href="#ArgShell.do_help-76"><span class="linenos"> 76</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
-</span><span id="ArgShell.do_help-77"><a href="#ArgShell.do_help-77"><span class="linenos"> 77</span></a>                    <span class="c1"># =========================Modification start=========================</span>
-</span><span id="ArgShell.do_help-78"><a href="#ArgShell.do_help-78"><span class="linenos"> 78</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
-</span><span id="ArgShell.do_help-79"><a href="#ArgShell.do_help-79"><span class="linenos"> 79</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="ArgShell.do_help-80"><a href="#ArgShell.do_help-80"><span class="linenos"> 80</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
-</span><span id="ArgShell.do_help-81"><a href="#ArgShell.do_help-81"><span class="linenos"> 81</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="ArgShell.do_help-82"><a href="#ArgShell.do_help-82"><span class="linenos"> 82</span></a>                        <span class="p">)</span>
-</span><span id="ArgShell.do_help-83"><a href="#ArgShell.do_help-83"><span class="linenos"> 83</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-84"><a href="#ArgShell.do_help-84"><span class="linenos"> 84</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
-</span><span id="ArgShell.do_help-85"><a href="#ArgShell.do_help-85"><span class="linenos"> 85</span></a>                        <span class="k">return</span>
-</span><span id="ArgShell.do_help-86"><a href="#ArgShell.do_help-86"><span class="linenos"> 86</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
-</span><span id="ArgShell.do_help-87"><a href="#ArgShell.do_help-87"><span class="linenos"> 87</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-88"><a href="#ArgShell.do_help-88"><span class="linenos"> 88</span></a>                    <span class="k">pass</span>
-</span><span id="ArgShell.do_help-89"><a href="#ArgShell.do_help-89"><span class="linenos"> 89</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
-</span><span id="ArgShell.do_help-90"><a href="#ArgShell.do_help-90"><span class="linenos"> 90</span></a>                <span class="k">return</span>
-</span><span id="ArgShell.do_help-91"><a href="#ArgShell.do_help-91"><span class="linenos"> 91</span></a>            <span class="n">func</span><span class="p">()</span>
-</span><span id="ArgShell.do_help-92"><a href="#ArgShell.do_help-92"><span class="linenos"> 92</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-93"><a href="#ArgShell.do_help-93"><span class="linenos"> 93</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
-</span><span id="ArgShell.do_help-94"><a href="#ArgShell.do_help-94"><span class="linenos"> 94</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="ArgShell.do_help-95"><a href="#ArgShell.do_help-95"><span class="linenos"> 95</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="ArgShell.do_help-96"><a href="#ArgShell.do_help-96"><span class="linenos"> 96</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
-</span><span id="ArgShell.do_help-97"><a href="#ArgShell.do_help-97"><span class="linenos"> 97</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-98"><a href="#ArgShell.do_help-98"><span class="linenos"> 98</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-99"><a href="#ArgShell.do_help-99"><span class="linenos"> 99</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
-</span><span id="ArgShell.do_help-100"><a href="#ArgShell.do_help-100"><span class="linenos">100</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="ArgShell.do_help-101"><a href="#ArgShell.do_help-101"><span class="linenos">101</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
-</span><span id="ArgShell.do_help-102"><a href="#ArgShell.do_help-102"><span class="linenos">102</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ArgShell.do_help-103"><a href="#ArgShell.do_help-103"><span class="linenos">103</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-104"><a href="#ArgShell.do_help-104"><span class="linenos">104</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-105"><a href="#ArgShell.do_help-105"><span class="linenos">105</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-106"><a href="#ArgShell.do_help-106"><span class="linenos">106</span></a>                        <span class="k">continue</span>
-</span><span id="ArgShell.do_help-107"><a href="#ArgShell.do_help-107"><span class="linenos">107</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
-</span><span id="ArgShell.do_help-108"><a href="#ArgShell.do_help-108"><span class="linenos">108</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
-</span><span id="ArgShell.do_help-109"><a href="#ArgShell.do_help-109"><span class="linenos">109</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-110"><a href="#ArgShell.do_help-110"><span class="linenos">110</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-111"><a href="#ArgShell.do_help-111"><span class="linenos">111</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-112"><a href="#ArgShell.do_help-112"><span class="linenos">112</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-113"><a href="#ArgShell.do_help-113"><span class="linenos">113</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-114"><a href="#ArgShell.do_help-114"><span class="linenos">114</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell.do_help-115"><a href="#ArgShell.do_help-115"><span class="linenos">115</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-116"><a href="#ArgShell.do_help-116"><span class="linenos">116</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
-</span><span id="ArgShell.do_help-117"><a href="#ArgShell.do_help-117"><span class="linenos">117</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-118"><a href="#ArgShell.do_help-118"><span class="linenos">118</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
-</span><span id="ArgShell.do_help-119"><a href="#ArgShell.do_help-119"><span class="linenos">119</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.do_help-69"><a href="#ArgShell.do_help-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">):</span>
+</span><span id="ArgShell.do_help-70"><a href="#ArgShell.do_help-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.</span>
+</span><span id="ArgShell.do_help-71"><a href="#ArgShell.do_help-71"><span class="linenos"> 71</span></a><span class="sd">        If using &#39;help cmd&#39; and the cmd is decorated with a parser, the parser help will also be printed.&quot;&quot;&quot;</span>
+</span><span id="ArgShell.do_help-72"><a href="#ArgShell.do_help-72"><span class="linenos"> 72</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-73"><a href="#ArgShell.do_help-73"><span class="linenos"> 73</span></a>            <span class="c1"># XXX check arg syntax</span>
+</span><span id="ArgShell.do_help-74"><a href="#ArgShell.do_help-74"><span class="linenos"> 74</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-75"><a href="#ArgShell.do_help-75"><span class="linenos"> 75</span></a>                <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;help_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-76"><a href="#ArgShell.do_help-76"><span class="linenos"> 76</span></a>            <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-77"><a href="#ArgShell.do_help-77"><span class="linenos"> 77</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-78"><a href="#ArgShell.do_help-78"><span class="linenos"> 78</span></a>                    <span class="n">func</span> <span class="o">=</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="s2">&quot;do_&quot;</span> <span class="o">+</span> <span class="n">arg</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-79"><a href="#ArgShell.do_help-79"><span class="linenos"> 79</span></a>                    <span class="n">doc</span> <span class="o">=</span> <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span>
+</span><span id="ArgShell.do_help-80"><a href="#ArgShell.do_help-80"><span class="linenos"> 80</span></a>                    <span class="k">if</span> <span class="n">doc</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-81"><a href="#ArgShell.do_help-81"><span class="linenos"> 81</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="n">doc</span><span class="p">))</span>
+</span><span id="ArgShell.do_help-82"><a href="#ArgShell.do_help-82"><span class="linenos"> 82</span></a>                    <span class="c1"># =========================Modification start=========================</span>
+</span><span id="ArgShell.do_help-83"><a href="#ArgShell.do_help-83"><span class="linenos"> 83</span></a>                    <span class="c1"># Check for decorator and call decorated function with &quot;--help&quot;</span>
+</span><span id="ArgShell.do_help-84"><a href="#ArgShell.do_help-84"><span class="linenos"> 84</span></a>                    <span class="k">if</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="ArgShell.do_help-85"><a href="#ArgShell.do_help-85"><span class="linenos"> 85</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
+</span><span id="ArgShell.do_help-86"><a href="#ArgShell.do_help-86"><span class="linenos"> 86</span></a>                            <span class="sa">f</span><span class="s2">&quot;Parser help for </span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;do_&#39;</span><span class="p">,</span><span class="s1">&#39;&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">:</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="ArgShell.do_help-87"><a href="#ArgShell.do_help-87"><span class="linenos"> 87</span></a>                        <span class="p">)</span>
+</span><span id="ArgShell.do_help-88"><a href="#ArgShell.do_help-88"><span class="linenos"> 88</span></a>                        <span class="n">func</span><span class="p">(</span><span class="s2">&quot;--help&quot;</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-89"><a href="#ArgShell.do_help-89"><span class="linenos"> 89</span></a>                    <span class="k">if</span> <span class="n">doc</span> <span class="ow">or</span> <span class="nb">hasattr</span><span class="p">(</span><span class="n">func</span><span class="p">,</span> <span class="s2">&quot;__wrapped__&quot;</span><span class="p">):</span>
+</span><span id="ArgShell.do_help-90"><a href="#ArgShell.do_help-90"><span class="linenos"> 90</span></a>                        <span class="k">return</span>
+</span><span id="ArgShell.do_help-91"><a href="#ArgShell.do_help-91"><span class="linenos"> 91</span></a>                    <span class="c1"># =========================Modification stop=========================</span>
+</span><span id="ArgShell.do_help-92"><a href="#ArgShell.do_help-92"><span class="linenos"> 92</span></a>                <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-93"><a href="#ArgShell.do_help-93"><span class="linenos"> 93</span></a>                    <span class="k">pass</span>
+</span><span id="ArgShell.do_help-94"><a href="#ArgShell.do_help-94"><span class="linenos"> 94</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">nohelp</span> <span class="o">%</span> <span class="p">(</span><span class="n">arg</span><span class="p">,)))</span>
+</span><span id="ArgShell.do_help-95"><a href="#ArgShell.do_help-95"><span class="linenos"> 95</span></a>                <span class="k">return</span>
+</span><span id="ArgShell.do_help-96"><a href="#ArgShell.do_help-96"><span class="linenos"> 96</span></a>            <span class="n">func</span><span class="p">()</span>
+</span><span id="ArgShell.do_help-97"><a href="#ArgShell.do_help-97"><span class="linenos"> 97</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-98"><a href="#ArgShell.do_help-98"><span class="linenos"> 98</span></a>            <span class="n">names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_names</span><span class="p">()</span>
+</span><span id="ArgShell.do_help-99"><a href="#ArgShell.do_help-99"><span class="linenos"> 99</span></a>            <span class="n">cmds_doc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="ArgShell.do_help-100"><a href="#ArgShell.do_help-100"><span class="linenos">100</span></a>            <span class="n">cmds_undoc</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="ArgShell.do_help-101"><a href="#ArgShell.do_help-101"><span class="linenos">101</span></a>            <span class="n">topics</span> <span class="o">=</span> <span class="nb">set</span><span class="p">()</span>
+</span><span id="ArgShell.do_help-102"><a href="#ArgShell.do_help-102"><span class="linenos">102</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-103"><a href="#ArgShell.do_help-103"><span class="linenos">103</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">5</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;help_&quot;</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-104"><a href="#ArgShell.do_help-104"><span class="linenos">104</span></a>                    <span class="n">topics</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">name</span><span class="p">[</span><span class="mi">5</span><span class="p">:])</span>
+</span><span id="ArgShell.do_help-105"><a href="#ArgShell.do_help-105"><span class="linenos">105</span></a>            <span class="n">names</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="ArgShell.do_help-106"><a href="#ArgShell.do_help-106"><span class="linenos">106</span></a>            <span class="c1"># There can be duplicates if routines overridden</span>
+</span><span id="ArgShell.do_help-107"><a href="#ArgShell.do_help-107"><span class="linenos">107</span></a>            <span class="n">prevname</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ArgShell.do_help-108"><a href="#ArgShell.do_help-108"><span class="linenos">108</span></a>            <span class="k">for</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">names</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-109"><a href="#ArgShell.do_help-109"><span class="linenos">109</span></a>                <span class="k">if</span> <span class="n">name</span><span class="p">[:</span><span class="mi">3</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;do_&quot;</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-110"><a href="#ArgShell.do_help-110"><span class="linenos">110</span></a>                    <span class="k">if</span> <span class="n">name</span> <span class="o">==</span> <span class="n">prevname</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-111"><a href="#ArgShell.do_help-111"><span class="linenos">111</span></a>                        <span class="k">continue</span>
+</span><span id="ArgShell.do_help-112"><a href="#ArgShell.do_help-112"><span class="linenos">112</span></a>                    <span class="n">prevname</span> <span class="o">=</span> <span class="n">name</span>
+</span><span id="ArgShell.do_help-113"><a href="#ArgShell.do_help-113"><span class="linenos">113</span></a>                    <span class="n">cmd</span> <span class="o">=</span> <span class="n">name</span><span class="p">[</span><span class="mi">3</span><span class="p">:]</span>
+</span><span id="ArgShell.do_help-114"><a href="#ArgShell.do_help-114"><span class="linenos">114</span></a>                    <span class="k">if</span> <span class="n">cmd</span> <span class="ow">in</span> <span class="n">topics</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-115"><a href="#ArgShell.do_help-115"><span class="linenos">115</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-116"><a href="#ArgShell.do_help-116"><span class="linenos">116</span></a>                        <span class="n">topics</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-117"><a href="#ArgShell.do_help-117"><span class="linenos">117</span></a>                    <span class="k">elif</span> <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__doc__</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-118"><a href="#ArgShell.do_help-118"><span class="linenos">118</span></a>                        <span class="n">cmds_doc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-119"><a href="#ArgShell.do_help-119"><span class="linenos">119</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell.do_help-120"><a href="#ArgShell.do_help-120"><span class="linenos">120</span></a>                        <span class="n">cmds_undoc</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cmd</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-121"><a href="#ArgShell.do_help-121"><span class="linenos">121</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">%s</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">%</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_leader</span><span class="p">))</span>
+</span><span id="ArgShell.do_help-122"><a href="#ArgShell.do_help-122"><span class="linenos">122</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">doc_header</span><span class="p">,</span> <span class="n">cmds_doc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-123"><a href="#ArgShell.do_help-123"><span class="linenos">123</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">misc_header</span><span class="p">,</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">topics</span><span class="p">),</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
+</span><span id="ArgShell.do_help-124"><a href="#ArgShell.do_help-124"><span class="linenos">124</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">print_topics</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">undoc_header</span><span class="p">,</span> <span class="n">cmds_undoc</span><span class="p">,</span> <span class="mi">15</span><span class="p">,</span> <span class="mi">80</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>List available commands with "help" or detailed help with "help cmd".
 If using 'help cmd' and the cmd is decorated with a parser, the parser help will also be printed.</p>
 </div>
 
@@ -803,71 +837,71 @@
         <span class="def">def</span>
         <span class="name">cmdloop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">intro</span><span class="o">=</span><span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ArgShell.cmdloop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ArgShell.cmdloop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.cmdloop-121"><a href="#ArgShell.cmdloop-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="ArgShell.cmdloop-122"><a href="#ArgShell.cmdloop-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
-</span><span id="ArgShell.cmdloop-123"><a href="#ArgShell.cmdloop-123"><span class="linenos">123</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
-</span><span id="ArgShell.cmdloop-124"><a href="#ArgShell.cmdloop-124"><span class="linenos">124</span></a><span class="sd">        the remainder of the line as argument.</span>
-</span><span id="ArgShell.cmdloop-125"><a href="#ArgShell.cmdloop-125"><span class="linenos">125</span></a>
-</span><span id="ArgShell.cmdloop-126"><a href="#ArgShell.cmdloop-126"><span class="linenos">126</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="ArgShell.cmdloop-127"><a href="#ArgShell.cmdloop-127"><span class="linenos">127</span></a>
-</span><span id="ArgShell.cmdloop-128"><a href="#ArgShell.cmdloop-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
-</span><span id="ArgShell.cmdloop-129"><a href="#ArgShell.cmdloop-129"><span class="linenos">129</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-130"><a href="#ArgShell.cmdloop-130"><span class="linenos">130</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-131"><a href="#ArgShell.cmdloop-131"><span class="linenos">131</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.cmdloop-126"><a href="#ArgShell.cmdloop-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">cmdloop</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">intro</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="ArgShell.cmdloop-127"><a href="#ArgShell.cmdloop-127"><span class="linenos">127</span></a>        <span class="sd">&quot;&quot;&quot;Repeatedly issue a prompt, accept input, parse an initial prefix</span>
+</span><span id="ArgShell.cmdloop-128"><a href="#ArgShell.cmdloop-128"><span class="linenos">128</span></a><span class="sd">        off the received input, and dispatch to action methods, passing them</span>
+</span><span id="ArgShell.cmdloop-129"><a href="#ArgShell.cmdloop-129"><span class="linenos">129</span></a><span class="sd">        the remainder of the line as argument.</span>
+</span><span id="ArgShell.cmdloop-130"><a href="#ArgShell.cmdloop-130"><span class="linenos">130</span></a>
+</span><span id="ArgShell.cmdloop-131"><a href="#ArgShell.cmdloop-131"><span class="linenos">131</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="ArgShell.cmdloop-132"><a href="#ArgShell.cmdloop-132"><span class="linenos">132</span></a>
-</span><span id="ArgShell.cmdloop-133"><a href="#ArgShell.cmdloop-133"><span class="linenos">133</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell.cmdloop-134"><a href="#ArgShell.cmdloop-134"><span class="linenos">134</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell.cmdloop-135"><a href="#ArgShell.cmdloop-135"><span class="linenos">135</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell.cmdloop-136"><a href="#ArgShell.cmdloop-136"><span class="linenos">136</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-137"><a href="#ArgShell.cmdloop-137"><span class="linenos">137</span></a>                <span class="k">pass</span>
-</span><span id="ArgShell.cmdloop-138"><a href="#ArgShell.cmdloop-138"><span class="linenos">138</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-139"><a href="#ArgShell.cmdloop-139"><span class="linenos">139</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-140"><a href="#ArgShell.cmdloop-140"><span class="linenos">140</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
-</span><span id="ArgShell.cmdloop-141"><a href="#ArgShell.cmdloop-141"><span class="linenos">141</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-142"><a href="#ArgShell.cmdloop-142"><span class="linenos">142</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-143"><a href="#ArgShell.cmdloop-143"><span class="linenos">143</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="ArgShell.cmdloop-144"><a href="#ArgShell.cmdloop-144"><span class="linenos">144</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-145"><a href="#ArgShell.cmdloop-145"><span class="linenos">145</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-146"><a href="#ArgShell.cmdloop-146"><span class="linenos">146</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-147"><a href="#ArgShell.cmdloop-147"><span class="linenos">147</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-148"><a href="#ArgShell.cmdloop-148"><span class="linenos">148</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-149"><a href="#ArgShell.cmdloop-149"><span class="linenos">149</span></a>                        <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-150"><a href="#ArgShell.cmdloop-150"><span class="linenos">150</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-151"><a href="#ArgShell.cmdloop-151"><span class="linenos">151</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-152"><a href="#ArgShell.cmdloop-152"><span class="linenos">152</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="ArgShell.cmdloop-153"><a href="#ArgShell.cmdloop-153"><span class="linenos">153</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-154"><a href="#ArgShell.cmdloop-154"><span class="linenos">154</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-155"><a href="#ArgShell.cmdloop-155"><span class="linenos">155</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
-</span><span id="ArgShell.cmdloop-156"><a href="#ArgShell.cmdloop-156"><span class="linenos">156</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
-</span><span id="ArgShell.cmdloop-157"><a href="#ArgShell.cmdloop-157"><span class="linenos">157</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
-</span><span id="ArgShell.cmdloop-158"><a href="#ArgShell.cmdloop-158"><span class="linenos">158</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
-</span><span id="ArgShell.cmdloop-159"><a href="#ArgShell.cmdloop-159"><span class="linenos">159</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-160"><a href="#ArgShell.cmdloop-160"><span class="linenos">160</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-161"><a href="#ArgShell.cmdloop-161"><span class="linenos">161</span></a>                <span class="c1"># ===========Modification start===========</span>
-</span><span id="ArgShell.cmdloop-162"><a href="#ArgShell.cmdloop-162"><span class="linenos">162</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-163"><a href="#ArgShell.cmdloop-163"><span class="linenos">163</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-164"><a href="#ArgShell.cmdloop-164"><span class="linenos">164</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-165"><a href="#ArgShell.cmdloop-165"><span class="linenos">165</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
-</span><span id="ArgShell.cmdloop-166"><a href="#ArgShell.cmdloop-166"><span class="linenos">166</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-167"><a href="#ArgShell.cmdloop-167"><span class="linenos">167</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
-</span><span id="ArgShell.cmdloop-168"><a href="#ArgShell.cmdloop-168"><span class="linenos">168</span></a>                <span class="c1"># ===========Modification stop===========</span>
-</span><span id="ArgShell.cmdloop-169"><a href="#ArgShell.cmdloop-169"><span class="linenos">169</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
-</span><span id="ArgShell.cmdloop-170"><a href="#ArgShell.cmdloop-170"><span class="linenos">170</span></a>        <span class="k">finally</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-171"><a href="#ArgShell.cmdloop-171"><span class="linenos">171</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-172"><a href="#ArgShell.cmdloop-172"><span class="linenos">172</span></a>                <span class="k">try</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-173"><a href="#ArgShell.cmdloop-173"><span class="linenos">173</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
-</span><span id="ArgShell.cmdloop-174"><a href="#ArgShell.cmdloop-174"><span class="linenos">174</span></a>
-</span><span id="ArgShell.cmdloop-175"><a href="#ArgShell.cmdloop-175"><span class="linenos">175</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="ArgShell.cmdloop-176"><a href="#ArgShell.cmdloop-176"><span class="linenos">176</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
-</span><span id="ArgShell.cmdloop-177"><a href="#ArgShell.cmdloop-177"><span class="linenos">177</span></a>                    <span class="k">pass</span>
+</span><span id="ArgShell.cmdloop-133"><a href="#ArgShell.cmdloop-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">preloop</span><span class="p">()</span>
+</span><span id="ArgShell.cmdloop-134"><a href="#ArgShell.cmdloop-134"><span class="linenos">134</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-135"><a href="#ArgShell.cmdloop-135"><span class="linenos">135</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-136"><a href="#ArgShell.cmdloop-136"><span class="linenos">136</span></a>                <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="ArgShell.cmdloop-137"><a href="#ArgShell.cmdloop-137"><span class="linenos">137</span></a>
+</span><span id="ArgShell.cmdloop-138"><a href="#ArgShell.cmdloop-138"><span class="linenos">138</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span> <span class="o">=</span> <span class="n">readline</span><span class="o">.</span><span class="n">get_completer</span><span class="p">()</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell.cmdloop-139"><a href="#ArgShell.cmdloop-139"><span class="linenos">139</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">complete</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell.cmdloop-140"><a href="#ArgShell.cmdloop-140"><span class="linenos">140</span></a>                <span class="n">readline</span><span class="o">.</span><span class="n">parse_and_bind</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">completekey</span> <span class="o">+</span> <span class="s2">&quot;: complete&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell.cmdloop-141"><a href="#ArgShell.cmdloop-141"><span class="linenos">141</span></a>            <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-142"><a href="#ArgShell.cmdloop-142"><span class="linenos">142</span></a>                <span class="k">pass</span>
+</span><span id="ArgShell.cmdloop-143"><a href="#ArgShell.cmdloop-143"><span class="linenos">143</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-144"><a href="#ArgShell.cmdloop-144"><span class="linenos">144</span></a>            <span class="k">if</span> <span class="n">intro</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-145"><a href="#ArgShell.cmdloop-145"><span class="linenos">145</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">intro</span> <span class="o">=</span> <span class="n">intro</span>
+</span><span id="ArgShell.cmdloop-146"><a href="#ArgShell.cmdloop-146"><span class="linenos">146</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-147"><a href="#ArgShell.cmdloop-147"><span class="linenos">147</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">intro</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-148"><a href="#ArgShell.cmdloop-148"><span class="linenos">148</span></a>            <span class="n">stop</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="ArgShell.cmdloop-149"><a href="#ArgShell.cmdloop-149"><span class="linenos">149</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">stop</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-150"><a href="#ArgShell.cmdloop-150"><span class="linenos">150</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-151"><a href="#ArgShell.cmdloop-151"><span class="linenos">151</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cmdqueue</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-152"><a href="#ArgShell.cmdloop-152"><span class="linenos">152</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-153"><a href="#ArgShell.cmdloop-153"><span class="linenos">153</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-154"><a href="#ArgShell.cmdloop-154"><span class="linenos">154</span></a>                        <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-155"><a href="#ArgShell.cmdloop-155"><span class="linenos">155</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-156"><a href="#ArgShell.cmdloop-156"><span class="linenos">156</span></a>                        <span class="k">except</span> <span class="ne">EOFError</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-157"><a href="#ArgShell.cmdloop-157"><span class="linenos">157</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="ArgShell.cmdloop-158"><a href="#ArgShell.cmdloop-158"><span class="linenos">158</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-159"><a href="#ArgShell.cmdloop-159"><span class="linenos">159</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prompt</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-160"><a href="#ArgShell.cmdloop-160"><span class="linenos">160</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span><span class="o">.</span><span class="n">flush</span><span class="p">()</span>
+</span><span id="ArgShell.cmdloop-161"><a href="#ArgShell.cmdloop-161"><span class="linenos">161</span></a>                        <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stdin</span><span class="o">.</span><span class="n">readline</span><span class="p">()</span>
+</span><span id="ArgShell.cmdloop-162"><a href="#ArgShell.cmdloop-162"><span class="linenos">162</span></a>                        <span class="k">if</span> <span class="ow">not</span> <span class="nb">len</span><span class="p">(</span><span class="n">line</span><span class="p">):</span>
+</span><span id="ArgShell.cmdloop-163"><a href="#ArgShell.cmdloop-163"><span class="linenos">163</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="s2">&quot;EOF&quot;</span>
+</span><span id="ArgShell.cmdloop-164"><a href="#ArgShell.cmdloop-164"><span class="linenos">164</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-165"><a href="#ArgShell.cmdloop-165"><span class="linenos">165</span></a>                            <span class="n">line</span> <span class="o">=</span> <span class="n">line</span><span class="o">.</span><span class="n">rstrip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\r\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-166"><a href="#ArgShell.cmdloop-166"><span class="linenos">166</span></a>                <span class="c1"># ===========Modification start===========</span>
+</span><span id="ArgShell.cmdloop-167"><a href="#ArgShell.cmdloop-167"><span class="linenos">167</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-168"><a href="#ArgShell.cmdloop-168"><span class="linenos">168</span></a>                    <span class="n">line</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">precmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-169"><a href="#ArgShell.cmdloop-169"><span class="linenos">169</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">onecmd</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-170"><a href="#ArgShell.cmdloop-170"><span class="linenos">170</span></a>                    <span class="n">stop</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">postcmd</span><span class="p">(</span><span class="n">stop</span><span class="p">,</span> <span class="n">line</span><span class="p">)</span>
+</span><span id="ArgShell.cmdloop-171"><a href="#ArgShell.cmdloop-171"><span class="linenos">171</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-172"><a href="#ArgShell.cmdloop-172"><span class="linenos">172</span></a>                    <span class="n">traceback</span><span class="o">.</span><span class="n">print_exc</span><span class="p">()</span>
+</span><span id="ArgShell.cmdloop-173"><a href="#ArgShell.cmdloop-173"><span class="linenos">173</span></a>                <span class="c1"># ===========Modification stop===========</span>
+</span><span id="ArgShell.cmdloop-174"><a href="#ArgShell.cmdloop-174"><span class="linenos">174</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">postloop</span><span class="p">()</span>
+</span><span id="ArgShell.cmdloop-175"><a href="#ArgShell.cmdloop-175"><span class="linenos">175</span></a>        <span class="k">finally</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-176"><a href="#ArgShell.cmdloop-176"><span class="linenos">176</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-177"><a href="#ArgShell.cmdloop-177"><span class="linenos">177</span></a>                <span class="k">try</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-178"><a href="#ArgShell.cmdloop-178"><span class="linenos">178</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
+</span><span id="ArgShell.cmdloop-179"><a href="#ArgShell.cmdloop-179"><span class="linenos">179</span></a>
+</span><span id="ArgShell.cmdloop-180"><a href="#ArgShell.cmdloop-180"><span class="linenos">180</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="ArgShell.cmdloop-181"><a href="#ArgShell.cmdloop-181"><span class="linenos">181</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+</span><span id="ArgShell.cmdloop-182"><a href="#ArgShell.cmdloop-182"><span class="linenos">182</span></a>                    <span class="k">pass</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Repeatedly issue a prompt, accept input, parse an initial prefix
 off the received input, and dispatch to action methods, passing them
 the remainder of the line as argument.</p>
 </div>
@@ -906,93 +940,93 @@
         <span class="def">def</span>
         <span class="name">with_parser</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n"><a href="#ArgShellParser">argshell.argshell.ArgShellParser</a></span><span class="p">]</span>,</span><span class="param">	<span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Callable</span><span class="p">[[</span><span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">],</span> <span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">]]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">) -> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]</span>:</span></span>
 
                 <label class="view-source-button" for="with_parser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#with_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="with_parser-180"><a href="#with_parser-180"><span class="linenos">180</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
-</span><span id="with_parser-181"><a href="#with_parser-181"><span class="linenos">181</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
-</span><span id="with_parser-182"><a href="#with_parser-182"><span class="linenos">182</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
-</span><span id="with_parser-183"><a href="#with_parser-183"><span class="linenos">183</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
-</span><span id="with_parser-184"><a href="#with_parser-184"><span class="linenos">184</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
-</span><span id="with_parser-185"><a href="#with_parser-185"><span class="linenos">185</span></a>
-</span><span id="with_parser-186"><a href="#with_parser-186"><span class="linenos">186</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
-</span><span id="with_parser-187"><a href="#with_parser-187"><span class="linenos">187</span></a>
-</span><span id="with_parser-188"><a href="#with_parser-188"><span class="linenos">188</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
-</span><span id="with_parser-189"><a href="#with_parser-189"><span class="linenos">189</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="with_parser-185"><a href="#with_parser-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
+</span><span id="with_parser-186"><a href="#with_parser-186"><span class="linenos">186</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
+</span><span id="with_parser-187"><a href="#with_parser-187"><span class="linenos">187</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
+</span><span id="with_parser-188"><a href="#with_parser-188"><span class="linenos">188</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
+</span><span id="with_parser-189"><a href="#with_parser-189"><span class="linenos">189</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
 </span><span id="with_parser-190"><a href="#with_parser-190"><span class="linenos">190</span></a>
-</span><span id="with_parser-191"><a href="#with_parser-191"><span class="linenos">191</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
-</span><span id="with_parser-192"><a href="#with_parser-192"><span class="linenos">192</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
-</span><span id="with_parser-193"><a href="#with_parser-193"><span class="linenos">193</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
-</span><span id="with_parser-194"><a href="#with_parser-194"><span class="linenos">194</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
-</span><span id="with_parser-195"><a href="#with_parser-195"><span class="linenos">195</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
-</span><span id="with_parser-196"><a href="#with_parser-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-197"><a href="#with_parser-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
-</span><span id="with_parser-198"><a href="#with_parser-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="with_parser-199"><a href="#with_parser-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
-</span><span id="with_parser-200"><a href="#with_parser-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
-</span><span id="with_parser-201"><a href="#with_parser-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
-</span><span id="with_parser-202"><a href="#with_parser-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="with_parser-203"><a href="#with_parser-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-204"><a href="#with_parser-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="with_parser-205"><a href="#with_parser-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
-</span><span id="with_parser-206"><a href="#with_parser-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="with_parser-207"><a href="#with_parser-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-208"><a href="#with_parser-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
-</span><span id="with_parser-209"><a href="#with_parser-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
-</span><span id="with_parser-210"><a href="#with_parser-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
-</span><span id="with_parser-211"><a href="#with_parser-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-212"><a href="#with_parser-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
-</span><span id="with_parser-213"><a href="#with_parser-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
-</span><span id="with_parser-214"><a href="#with_parser-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
-</span><span id="with_parser-215"><a href="#with_parser-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-216"><a href="#with_parser-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
-</span><span id="with_parser-217"><a href="#with_parser-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
-</span><span id="with_parser-218"><a href="#with_parser-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
-</span><span id="with_parser-219"><a href="#with_parser-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
-</span><span id="with_parser-220"><a href="#with_parser-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
-</span><span id="with_parser-221"><a href="#with_parser-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
-</span><span id="with_parser-222"><a href="#with_parser-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
-</span><span id="with_parser-223"><a href="#with_parser-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
-</span><span id="with_parser-224"><a href="#with_parser-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
-</span><span id="with_parser-225"><a href="#with_parser-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
-</span><span id="with_parser-226"><a href="#with_parser-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
-</span><span id="with_parser-227"><a href="#with_parser-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
-</span><span id="with_parser-228"><a href="#with_parser-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
-</span><span id="with_parser-229"><a href="#with_parser-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
-</span><span id="with_parser-230"><a href="#with_parser-230"><span class="linenos">230</span></a>
-</span><span id="with_parser-231"><a href="#with_parser-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
-</span><span id="with_parser-232"><a href="#with_parser-232"><span class="linenos">232</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
-</span><span id="with_parser-233"><a href="#with_parser-233"><span class="linenos">233</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="with_parser-234"><a href="#with_parser-234"><span class="linenos">234</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
-</span><span id="with_parser-235"><a href="#with_parser-235"><span class="linenos">235</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="with_parser-236"><a href="#with_parser-236"><span class="linenos">236</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="with_parser-237"><a href="#with_parser-237"><span class="linenos">237</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
-</span><span id="with_parser-238"><a href="#with_parser-238"><span class="linenos">238</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="with_parser-239"><a href="#with_parser-239"><span class="linenos">239</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
-</span><span id="with_parser-240"><a href="#with_parser-240"><span class="linenos">240</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="with_parser-241"><a href="#with_parser-241"><span class="linenos">241</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="with_parser-242"><a href="#with_parser-242"><span class="linenos">242</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="with_parser-243"><a href="#with_parser-243"><span class="linenos">243</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="with_parser-244"><a href="#with_parser-244"><span class="linenos">244</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
-</span><span id="with_parser-245"><a href="#with_parser-245"><span class="linenos">245</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="with_parser-246"><a href="#with_parser-246"><span class="linenos">246</span></a>                        <span class="k">pass</span>
-</span><span id="with_parser-247"><a href="#with_parser-247"><span class="linenos">247</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="with_parser-248"><a href="#with_parser-248"><span class="linenos">248</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
-</span><span id="with_parser-249"><a href="#with_parser-249"><span class="linenos">249</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="with_parser-250"><a href="#with_parser-250"><span class="linenos">250</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="with_parser-251"><a href="#with_parser-251"><span class="linenos">251</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
-</span><span id="with_parser-252"><a href="#with_parser-252"><span class="linenos">252</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="with_parser-253"><a href="#with_parser-253"><span class="linenos">253</span></a>
-</span><span id="with_parser-254"><a href="#with_parser-254"><span class="linenos">254</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="with_parser-255"><a href="#with_parser-255"><span class="linenos">255</span></a>
-</span><span id="with_parser-256"><a href="#with_parser-256"><span class="linenos">256</span></a>        <span class="k">return</span> <span class="n">inner</span>
-</span><span id="with_parser-257"><a href="#with_parser-257"><span class="linenos">257</span></a>
-</span><span id="with_parser-258"><a href="#with_parser-258"><span class="linenos">258</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+</span><span id="with_parser-191"><a href="#with_parser-191"><span class="linenos">191</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
+</span><span id="with_parser-192"><a href="#with_parser-192"><span class="linenos">192</span></a>
+</span><span id="with_parser-193"><a href="#with_parser-193"><span class="linenos">193</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
+</span><span id="with_parser-194"><a href="#with_parser-194"><span class="linenos">194</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="with_parser-195"><a href="#with_parser-195"><span class="linenos">195</span></a>
+</span><span id="with_parser-196"><a href="#with_parser-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
+</span><span id="with_parser-197"><a href="#with_parser-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
+</span><span id="with_parser-198"><a href="#with_parser-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
+</span><span id="with_parser-199"><a href="#with_parser-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
+</span><span id="with_parser-200"><a href="#with_parser-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
+</span><span id="with_parser-201"><a href="#with_parser-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-202"><a href="#with_parser-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
+</span><span id="with_parser-203"><a href="#with_parser-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="with_parser-204"><a href="#with_parser-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
+</span><span id="with_parser-205"><a href="#with_parser-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
+</span><span id="with_parser-206"><a href="#with_parser-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
+</span><span id="with_parser-207"><a href="#with_parser-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="with_parser-208"><a href="#with_parser-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-209"><a href="#with_parser-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="with_parser-210"><a href="#with_parser-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
+</span><span id="with_parser-211"><a href="#with_parser-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="with_parser-212"><a href="#with_parser-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-213"><a href="#with_parser-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
+</span><span id="with_parser-214"><a href="#with_parser-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
+</span><span id="with_parser-215"><a href="#with_parser-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
+</span><span id="with_parser-216"><a href="#with_parser-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-217"><a href="#with_parser-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
+</span><span id="with_parser-218"><a href="#with_parser-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
+</span><span id="with_parser-219"><a href="#with_parser-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
+</span><span id="with_parser-220"><a href="#with_parser-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-221"><a href="#with_parser-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
+</span><span id="with_parser-222"><a href="#with_parser-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
+</span><span id="with_parser-223"><a href="#with_parser-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
+</span><span id="with_parser-224"><a href="#with_parser-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
+</span><span id="with_parser-225"><a href="#with_parser-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
+</span><span id="with_parser-226"><a href="#with_parser-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
+</span><span id="with_parser-227"><a href="#with_parser-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
+</span><span id="with_parser-228"><a href="#with_parser-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
+</span><span id="with_parser-229"><a href="#with_parser-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
+</span><span id="with_parser-230"><a href="#with_parser-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
+</span><span id="with_parser-231"><a href="#with_parser-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
+</span><span id="with_parser-232"><a href="#with_parser-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
+</span><span id="with_parser-233"><a href="#with_parser-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
+</span><span id="with_parser-234"><a href="#with_parser-234"><span class="linenos">234</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
+</span><span id="with_parser-235"><a href="#with_parser-235"><span class="linenos">235</span></a>
+</span><span id="with_parser-236"><a href="#with_parser-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
+</span><span id="with_parser-237"><a href="#with_parser-237"><span class="linenos">237</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
+</span><span id="with_parser-238"><a href="#with_parser-238"><span class="linenos">238</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="with_parser-239"><a href="#with_parser-239"><span class="linenos">239</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
+</span><span id="with_parser-240"><a href="#with_parser-240"><span class="linenos">240</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="with_parser-241"><a href="#with_parser-241"><span class="linenos">241</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="with_parser-242"><a href="#with_parser-242"><span class="linenos">242</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
+</span><span id="with_parser-243"><a href="#with_parser-243"><span class="linenos">243</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="with_parser-244"><a href="#with_parser-244"><span class="linenos">244</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
+</span><span id="with_parser-245"><a href="#with_parser-245"><span class="linenos">245</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="with_parser-246"><a href="#with_parser-246"><span class="linenos">246</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="with_parser-247"><a href="#with_parser-247"><span class="linenos">247</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="with_parser-248"><a href="#with_parser-248"><span class="linenos">248</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="with_parser-249"><a href="#with_parser-249"><span class="linenos">249</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
+</span><span id="with_parser-250"><a href="#with_parser-250"><span class="linenos">250</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="with_parser-251"><a href="#with_parser-251"><span class="linenos">251</span></a>                        <span class="k">pass</span>
+</span><span id="with_parser-252"><a href="#with_parser-252"><span class="linenos">252</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="with_parser-253"><a href="#with_parser-253"><span class="linenos">253</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
+</span><span id="with_parser-254"><a href="#with_parser-254"><span class="linenos">254</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="with_parser-255"><a href="#with_parser-255"><span class="linenos">255</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="with_parser-256"><a href="#with_parser-256"><span class="linenos">256</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
+</span><span id="with_parser-257"><a href="#with_parser-257"><span class="linenos">257</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="with_parser-258"><a href="#with_parser-258"><span class="linenos">258</span></a>
+</span><span id="with_parser-259"><a href="#with_parser-259"><span class="linenos">259</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="with_parser-260"><a href="#with_parser-260"><span class="linenos">260</span></a>
+</span><span id="with_parser-261"><a href="#with_parser-261"><span class="linenos">261</span></a>        <span class="k">return</span> <span class="n">inner</span>
+</span><span id="with_parser-262"><a href="#with_parser-262"><span class="linenos">262</span></a>
+</span><span id="with_parser-263"><a href="#with_parser-263"><span class="linenos">263</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Decorate a 'do_*' function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</p>
 
 <h6 id="parameters">Parameters</h6>
```

#### html2text {}

```diff
@@ -6,355 +6,361 @@
     * Namespace
     * ArgShellParser
           o exit
           o error
           o parse_args
     * ArgShell
           o do_quit
+          o do_sys
           o do_help
           o cmdloop
     * with_parser
 built_with_pdoc[pdoc_logo]
 
 ****** argshell.argshell ******
 ⁰ View Source
 __1import argparse
 __2import cmd
-__3import shlex
-__4import sys
-__5import traceback
-__6from functools import wraps
-__7from typing import Any, Callable
-__8
+__3import os
+__4import shlex
+__5import sys
+__6import traceback
+__7from functools import wraps
+__8from typing import Any, Callable
 __9
-_10class Namespace(argparse.Namespace):
-_11    """Simple object for storing attributes.
-_12
-_13    Implements equality by attribute names and values, and provides a simple
+_10
+_11class Namespace(argparse.Namespace):
+_12    """Simple object for storing attributes.
+_13
+_14    Implements equality by attribute names and values, and provides a simple
 string representation."""
-_14
 _15
-_16class ArgShellParser(argparse.ArgumentParser):
-_17    """***Overrides exit, error, and parse_args methods***
-_18
-_19    Object for parsing command line strings into Python objects.
-_20
-_21    Keyword Arguments:
-_22        - prog -- The name of the program (default:
-_23            ``os.path.basename(sys.argv[0])``)
-_24        - usage -- A usage message (default: auto-generated from arguments)
-_25        - description -- A description of what the program does
-_26        - epilog -- Text following the argument descriptions
-_27        - parents -- Parsers whose arguments should be copied into this one
-_28        - formatter_class -- HelpFormatter class for printing help messages
-_29        - prefix_chars -- Characters that prefix optional arguments
-_30        - fromfile_prefix_chars -- Characters that prefix files containing
-_31            additional arguments
-_32        - argument_default -- The default value for all arguments
-_33        - conflict_handler -- String indicating how to handle conflicts
-_34        - add_help -- Add a -h/-help option
-_35        - allow_abbrev -- Allow long options to be abbreviated unambiguously
-_36        - exit_on_error -- Determines whether or not ArgumentParser exits
+_16
+_17class ArgShellParser(argparse.ArgumentParser):
+_18    """***Overrides exit, error, and parse_args methods***
+_19
+_20    Object for parsing command line strings into Python objects.
+_21
+_22    Keyword Arguments:
+_23        - prog -- The name of the program (default:
+_24            ``os.path.basename(sys.argv[0])``)
+_25        - usage -- A usage message (default: auto-generated from arguments)
+_26        - description -- A description of what the program does
+_27        - epilog -- Text following the argument descriptions
+_28        - parents -- Parsers whose arguments should be copied into this one
+_29        - formatter_class -- HelpFormatter class for printing help messages
+_30        - prefix_chars -- Characters that prefix optional arguments
+_31        - fromfile_prefix_chars -- Characters that prefix files containing
+_32            additional arguments
+_33        - argument_default -- The default value for all arguments
+_34        - conflict_handler -- String indicating how to handle conflicts
+_35        - add_help -- Add a -h/-help option
+_36        - allow_abbrev -- Allow long options to be abbreviated unambiguously
+_37        - exit_on_error -- Determines whether or not ArgumentParser exits
 with
-_37            error info when an error occurs
-_38    """
-_39
-_40    def exit(self, status=0, message=None):
-_41        """Override to prevent shell exit when passing -h/--help
+_38            error info when an error occurs
+_39    """
+_40
+_41    def exit(self, status=0, message=None):
+_42        """Override to prevent shell exit when passing -h/--help
 switches."""
-_42        if message:
-_43            self._print_message(message, sys.stderr)
-_44
-_45    def error(self, message):
-_46        raise Exception(f"prog: {self.prog}, message: {message}")
-_47
-_48    def parse_args(self, *args, **kwargs) -> Namespace:
-_49        parsed_args: Namespace = super().parse_args(*args, **kwargs)
-_50        return parsed_args
-_51
+_43        if message:
+_44            self._print_message(message, sys.stderr)
+_45
+_46    def error(self, message):
+_47        raise Exception(f"prog: {self.prog}, message: {message}")
+_48
+_49    def parse_args(self, *args, **kwargs) -> Namespace:
+_50        parsed_args: Namespace = super().parse_args(*args, **kwargs)
+_51        return parsed_args
 _52
-_53class ArgShell(cmd.Cmd):
-_54    """Subclass this to create custom ArgShells."""
-_55
-_56    intro = "Entering argshell..."
-_57    prompt = "argshell>"
-_58
-_59    def do_quit(self, command: str):
-_60        """Quit shell."""
-_61        return True
-_62
-_63    def do_help(self, arg):
-_64        """List available commands with "help" or detailed help with "help
+_53
+_54class ArgShell(cmd.Cmd):
+_55    """Subclass this to create custom ArgShells."""
+_56
+_57    intro = "Entering argshell..."
+_58    prompt = "argshell>"
+_59
+_60    def do_quit(self, command: str):
+_61        """Quit shell."""
+_62        return True
+_63
+_64    def do_sys(self, command: str):
+_65        """Execute command with `os.system()`."""
+_66        os.system(command)
+_67
+_68    def do_help(self, arg):
+_69        """List available commands with "help" or detailed help with "help
 cmd".
-_65        If using 'help cmd' and the cmd is decorated with a parser, the
+_70        If using 'help cmd' and the cmd is decorated with a parser, the
 parser help will also be printed."""
-_66        if arg:
-_67            # XXX check arg syntax
-_68            try:
-_69                func = getattr(self, "help_" + arg)
-_70            except AttributeError:
-_71                try:
-_72                    func = getattr(self, "do_" + arg)
-_73                    doc = func.__doc__
-_74                    if doc:
-_75                        self.stdout.write("%s\n" % str(doc))
-_76                    # =========================Modification
+_71        if arg:
+_72            # XXX check arg syntax
+_73            try:
+_74                func = getattr(self, "help_" + arg)
+_75            except AttributeError:
+_76                try:
+_77                    func = getattr(self, "do_" + arg)
+_78                    doc = func.__doc__
+_79                    if doc:
+_80                        self.stdout.write("%s\n" % str(doc))
+_81                    # =========================Modification
 start=========================
-_77                    # Check for decorator and call decorated function with
+_82                    # Check for decorator and call decorated function with
 "--help"
-_78                    if hasattr(func, "__wrapped__"):
-_79                        self.stdout.write(
-_80                            f"Parser help for {func.__name__.replace
+_83                    if hasattr(func, "__wrapped__"):
+_84                        self.stdout.write(
+_85                            f"Parser help for {func.__name__.replace
 ('do_','')}:\n"
-_81                        )
-_82                        func("--help")
-_83                    if doc or hasattr(func, "__wrapped__"):
-_84                        return
-_85                    # =========================Modification
+_86                        )
+_87                        func("--help")
+_88                    if doc or hasattr(func, "__wrapped__"):
+_89                        return
+_90                    # =========================Modification
 stop=========================
-_86                except AttributeError:
-_87                    pass
-_88                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
-_89                return
-_90            func()
-_91        else:
-_92            names = self.get_names()
-_93            cmds_doc = []
-_94            cmds_undoc = []
-_95            topics = set()
-_96            for name in names:
-_97                if name[:5] == "help_":
-_98                    topics.add(name[5:])
-_99            names.sort()
-100            # There can be duplicates if routines overridden
-101            prevname = ""
-102            for name in names:
-103                if name[:3] == "do_":
-104                    if name == prevname:
-105                        continue
-106                    prevname = name
-107                    cmd = name[3:]
-108                    if cmd in topics:
-109                        cmds_doc.append(cmd)
-110                        topics.remove(cmd)
-111                    elif getattr(self, name).__doc__:
-112                        cmds_doc.append(cmd)
-113                    else:
-114                        cmds_undoc.append(cmd)
-115            self.stdout.write("%s\n" % str(self.doc_leader))
-116            self.print_topics(self.doc_header, cmds_doc, 15, 80)
-117            self.print_topics(self.misc_header, sorted(topics), 15, 80)
-118            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
-119
-120    def cmdloop(self, intro=None):
-121        """Repeatedly issue a prompt, accept input, parse an initial prefix
-122        off the received input, and dispatch to action methods, passing them
-123        the remainder of the line as argument.
+_91                except AttributeError:
+_92                    pass
+_93                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
+_94                return
+_95            func()
+_96        else:
+_97            names = self.get_names()
+_98            cmds_doc = []
+_99            cmds_undoc = []
+100            topics = set()
+101            for name in names:
+102                if name[:5] == "help_":
+103                    topics.add(name[5:])
+104            names.sort()
+105            # There can be duplicates if routines overridden
+106            prevname = ""
+107            for name in names:
+108                if name[:3] == "do_":
+109                    if name == prevname:
+110                        continue
+111                    prevname = name
+112                    cmd = name[3:]
+113                    if cmd in topics:
+114                        cmds_doc.append(cmd)
+115                        topics.remove(cmd)
+116                    elif getattr(self, name).__doc__:
+117                        cmds_doc.append(cmd)
+118                    else:
+119                        cmds_undoc.append(cmd)
+120            self.stdout.write("%s\n" % str(self.doc_leader))
+121            self.print_topics(self.doc_header, cmds_doc, 15, 80)
+122            self.print_topics(self.misc_header, sorted(topics), 15, 80)
+123            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
 124
-125        """
-126
-127        self.preloop()
-128        if self.use_rawinput and self.completekey:
-129            try:
-130                import readline
+125    def cmdloop(self, intro=None):
+126        """Repeatedly issue a prompt, accept input, parse an initial prefix
+127        off the received input, and dispatch to action methods, passing them
+128        the remainder of the line as argument.
+129
+130        """
 131
-132                self.old_completer = readline.get_completer()  # type:
+132        self.preloop()
+133        if self.use_rawinput and self.completekey:
+134            try:
+135                import readline
+136
+137                self.old_completer = readline.get_completer()  # type:
 ignore
-133                readline.set_completer(self.complete)  # type: ignore
-134                readline.parse_and_bind(self.completekey + ": complete")  #
+138                readline.set_completer(self.complete)  # type: ignore
+139                readline.parse_and_bind(self.completekey + ": complete")  #
 type: ignore
-135            except ImportError:
-136                pass
-137        try:
-138            if intro is not None:
-139                self.intro = intro
-140            if self.intro:
-141                self.stdout.write(str(self.intro) + "\n")
-142            stop = None
-143            while not stop:
-144                if self.cmdqueue:
-145                    line = self.cmdqueue.pop(0)
-146                else:
-147                    if self.use_rawinput:
-148                        try:
-149                            line = input(self.prompt)
-150                        except EOFError:
-151                            line = "EOF"
-152                    else:
-153                        self.stdout.write(self.prompt)
-154                        self.stdout.flush()
-155                        line = self.stdin.readline()
-156                        if not len(line):
-157                            line = "EOF"
-158                        else:
-159                            line = line.rstrip("\r\n")
-160                # ===========Modification start===========
-161                try:
-162                    line = self.precmd(line)
-163                    stop = self.onecmd(line)
-164                    stop = self.postcmd(stop, line)
-165                except Exception as e:
-166                    traceback.print_exc()
-167                # ===========Modification stop===========
-168            self.postloop()
-169        finally:
-170            if self.use_rawinput and self.completekey:
-171                try:
-172                    import readline
-173
-174                    readline.set_completer(self.old_completer)  # type:
-ignore
-175                except ImportError:
-176                    pass
-177
+140            except ImportError:
+141                pass
+142        try:
+143            if intro is not None:
+144                self.intro = intro
+145            if self.intro:
+146                self.stdout.write(str(self.intro) + "\n")
+147            stop = None
+148            while not stop:
+149                if self.cmdqueue:
+150                    line = self.cmdqueue.pop(0)
+151                else:
+152                    if self.use_rawinput:
+153                        try:
+154                            line = input(self.prompt)
+155                        except EOFError:
+156                            line = "EOF"
+157                    else:
+158                        self.stdout.write(self.prompt)
+159                        self.stdout.flush()
+160                        line = self.stdin.readline()
+161                        if not len(line):
+162                            line = "EOF"
+163                        else:
+164                            line = line.rstrip("\r\n")
+165                # ===========Modification start===========
+166                try:
+167                    line = self.precmd(line)
+168                    stop = self.onecmd(line)
+169                    stop = self.postcmd(stop, line)
+170                except Exception as e:
+171                    traceback.print_exc()
+172                # ===========Modification stop===========
+173            self.postloop()
+174        finally:
+175            if self.use_rawinput and self.completekey:
+176                try:
+177                    import readline
 178
-179def with_parser(
-180    parser: Callable[..., ArgShellParser],
-181    post_parsers: list[Callable[[Namespace], Namespace]] = [],
-182) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
-183    """Decorate a 'do_*' function in an argshell.ArgShell class with this
+179                    readline.set_completer(self.old_completer)  # type:
+ignore
+180                except ImportError:
+181                    pass
+182
+183
+184def with_parser(
+185    parser: Callable[..., ArgShellParser],
+186    post_parsers: list[Callable[[Namespace], Namespace]] = [],
+187) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
+188    """Decorate a 'do_*' function in an argshell.ArgShell class with this
 function to pass an argshell.Namespace object to the decorated function instead
 of a string.
-184
-185    :param parser: A function that creates an argshell.ArgShellParser
+189
+190    :param parser: A function that creates an argshell.ArgShellParser
 instance, adds arguments to it, and returns the parser.
-186
-187    :param post_parsers: An optional list of functions to execute where each
+191
+192    :param post_parsers: An optional list of functions to execute where each
 function takes an argshell.Namespace instance and returns an argshell.Namespace
 instance.
-188        'post_parser' functions are executed in the order they are supplied.
-189
-190    >>> def get_parser() -> argshell.ArgShellParser:
-191    >>>     parser = argshell.ArgShellParser()
-192    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
+193        'post_parser' functions are executed in the order they are supplied.
+194
+195    >>> def get_parser() -> argshell.ArgShellParser:
+196    >>>     parser = argshell.ArgShellParser()
+197    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
 of first and last names to print.")
-193    >>>     parser.add_argument("-i", "--initials", action="store_true",
+198    >>>     parser.add_argument("-i", "--initials", action="store_true",
 help="Print the initials instead of the full name.")
-194    >>>     return parser
-195    >>>
-196    >>> # Convert list of first and last names to a list of tuples
-197    >>> def names_list_to_tuples(args: argshell.Namespace) -
+199    >>>     return parser
+200    >>>
+201    >>> # Convert list of first and last names to a list of tuples
+202    >>> def names_list_to_tuples(args: argshell.Namespace) -
 > argshell.Namespace:
-198    >>>     args.names = [(first, last) for first, last in zip(args.names[::
+203    >>>     args.names = [(first, last) for first, last in zip(args.names[::
 2], args.names[1::2])]
-199    >>>     if args.initials:
-200    >>>         args.names = [(name[0][0], name[1][0]) for name in
+204    >>>     if args.initials:
+205    >>>         args.names = [(name[0][0], name[1][0]) for name in
 args.names]
-201    >>>     return args
-202    >>>
-203    >>> def capitalize_names(args: argshell.Namespace) -
+206    >>>     return args
+207    >>>
+208    >>> def capitalize_names(args: argshell.Namespace) -
 > argshell.Namespace:
-204    >>>     args.names = [name.capitalize() for name in args.names]
-205    >>>     return args
-206    >>>
-207    >>> class NameShell(ArgShell):
-208    >>>     intro = "Entering nameshell..."
-209    >>>     prompt = "nameshell>"
-210    >>>
-211    >>>     @with_parser(get_parser, [capitalize_names,
+209    >>>     args.names = [name.capitalize() for name in args.names]
+210    >>>     return args
+211    >>>
+212    >>> class NameShell(ArgShell):
+213    >>>     intro = "Entering nameshell..."
+214    >>>     prompt = "nameshell>"
+215    >>>
+216    >>>     @with_parser(get_parser, [capitalize_names,
 names_list_to_tuples])
-212    >>>     def do_printnames(self, args: argshell.Namespace):
-213    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
+217    >>>     def do_printnames(self, args: argshell.Namespace):
+218    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
 sep="\\n")
-214    >>>
-215    >>> NameShell().cmdloop()
-216    >>> Entering nameshell...
-217    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+219    >>>
+220    >>> NameShell().cmdloop()
+221    >>> Entering nameshell...
+222    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno
-218    >>> Karl Marx
-219    >>> Fred Hampton
-220    >>> Emma Goldman
-221    >>> Angela Davis
-222    >>> Nestor Makhno
-223    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+223    >>> Karl Marx
+224    >>> Fred Hampton
+225    >>> Emma Goldman
+226    >>> Angela Davis
+227    >>> Nestor Makhno
+228    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno -i
-224    >>> K M
-225    >>> F H
-226    >>> E G
-227    >>> A D
-228    >>> N M"""
-229
-230    def decorator(
-231        func: Callable[[Any, Namespace], Any | None]
-232    ) -> Callable[[Any, str], Any]:
-233        @wraps(func)
-234        def inner(self: Any, command: str) -> Any:
-235            try:
-236                args = parser().parse_args(shlex.split(command))
-237            except Exception as e:
-238                # On parser error, print help and skip post_parser and func
+229    >>> K M
+230    >>> F H
+231    >>> E G
+232    >>> A D
+233    >>> N M"""
+234
+235    def decorator(
+236        func: Callable[[Any, Namespace], Any | None]
+237    ) -> Callable[[Any, str], Any]:
+238        @wraps(func)
+239        def inner(self: Any, command: str) -> Any:
+240            try:
+241                args = parser().parse_args(shlex.split(command))
+242            except Exception as e:
+243                # On parser error, print help and skip post_parser and func
 execution
-239                if "the following arguments are required" not in str(e):
-240                    print(f"ERROR: {e}")
-241                if "-h" not in command and "--help" not in command:
-242                    try:
-243                        args = parser().parse_args(["--help"])
-244                    except Exception as e:
-245                        pass
-246                return None
-247            # Don't execute function, only print parser help
-248            if "-h" in command or "--help" in command:
-249                return None
-250            for post_parser in post_parsers:
-251                args = post_parser(args)
-252
-253            return func(self, args)
-254
-255        return inner
-256
-257    return decorator
+244                if "the following arguments are required" not in str(e):
+245                    print(f"ERROR: {e}")
+246                if "-h" not in command and "--help" not in command:
+247                    try:
+248                        args = parser().parse_args(["--help"])
+249                    except Exception as e:
+250                        pass
+251                return None
+252            # Don't execute function, only print parser help
+253            if "-h" in command or "--help" in command:
+254                return None
+255            for post_parser in post_parsers:
+256                args = post_parser(args)
+257
+258            return func(self, args)
+259
+260        return inner
+261
+262    return decorator
   ⁰
 class Namespace(argparse.Namespace): View Source
-11class Namespace(argparse.Namespace):
-12    """Simple object for storing attributes.
-13
-14    Implements equality by attribute names and values, and provides a simple
+12class Namespace(argparse.Namespace):
+13    """Simple object for storing attributes.
+14
+15    Implements equality by attribute names and values, and provides a simple
 string representation."""
 Simple object for storing attributes.
 Implements equality by attribute names and values, and provides a simple string
 representation.
 ** Inherited Members **
   ⁰
 class ArgShellParser(argparse.ArgumentParser): View Source
-17class ArgShellParser(argparse.ArgumentParser):
-18    """***Overrides exit, error, and parse_args methods***
-19
-20    Object for parsing command line strings into Python objects.
-21
-22    Keyword Arguments:
-23        - prog -- The name of the program (default:
-24            ``os.path.basename(sys.argv[0])``)
-25        - usage -- A usage message (default: auto-generated from arguments)
-26        - description -- A description of what the program does
-27        - epilog -- Text following the argument descriptions
-28        - parents -- Parsers whose arguments should be copied into this one
-29        - formatter_class -- HelpFormatter class for printing help messages
-30        - prefix_chars -- Characters that prefix optional arguments
-31        - fromfile_prefix_chars -- Characters that prefix files containing
-32            additional arguments
-33        - argument_default -- The default value for all arguments
-34        - conflict_handler -- String indicating how to handle conflicts
-35        - add_help -- Add a -h/-help option
-36        - allow_abbrev -- Allow long options to be abbreviated unambiguously
-37        - exit_on_error -- Determines whether or not ArgumentParser exits
+18class ArgShellParser(argparse.ArgumentParser):
+19    """***Overrides exit, error, and parse_args methods***
+20
+21    Object for parsing command line strings into Python objects.
+22
+23    Keyword Arguments:
+24        - prog -- The name of the program (default:
+25            ``os.path.basename(sys.argv[0])``)
+26        - usage -- A usage message (default: auto-generated from arguments)
+27        - description -- A description of what the program does
+28        - epilog -- Text following the argument descriptions
+29        - parents -- Parsers whose arguments should be copied into this one
+30        - formatter_class -- HelpFormatter class for printing help messages
+31        - prefix_chars -- Characters that prefix optional arguments
+32        - fromfile_prefix_chars -- Characters that prefix files containing
+33            additional arguments
+34        - argument_default -- The default value for all arguments
+35        - conflict_handler -- String indicating how to handle conflicts
+36        - add_help -- Add a -h/-help option
+37        - allow_abbrev -- Allow long options to be abbreviated unambiguously
+38        - exit_on_error -- Determines whether or not ArgumentParser exits
 with
-38            error info when an error occurs
-39    """
-40
-41    def exit(self, status=0, message=None):
-42        """Override to prevent shell exit when passing -h/--help switches."""
-43        if message:
-44            self._print_message(message, sys.stderr)
-45
-46    def error(self, message):
-47        raise Exception(f"prog: {self.prog}, message: {message}")
-48
-49    def parse_args(self, *args, **kwargs) -> Namespace:
-50        parsed_args: Namespace = super().parse_args(*args, **kwargs)
-51        return parsed_args
+39            error info when an error occurs
+40    """
+41
+42    def exit(self, status=0, message=None):
+43        """Override to prevent shell exit when passing -h/--help switches."""
+44        if message:
+45            self._print_message(message, sys.stderr)
+46
+47    def error(self, message):
+48        raise Exception(f"prog: {self.prog}, message: {message}")
+49
+50    def parse_args(self, *args, **kwargs) -> Namespace:
+51        parsed_args: Namespace = super().parse_args(*args, **kwargs)
+52        return parsed_args
 Overrides exit, error, and parse_args methods
 Object for parsing command line strings into Python objects.
 Keyword Arguments: - prog -- The name of the program (default: os.path.basename
 (sys.argv[0])) - usage -- A usage message (default: auto-generated from
 arguments) - description -- A description of what the program does - epilog -
 - Text following the argument descriptions - parents -- Parsers whose arguments
 should be copied into this one - formatter_class -- HelpFormatter class for
@@ -363,410 +369,420 @@
 additional arguments - argument_default -- The default value for all arguments
 - conflict_handler -- String indicating how to handle conflicts - add_help -
 - Add a -h/-help option - allow_abbrev -- Allow long options to be abbreviated
 unambiguously - exit_on_error -- Determines whether or not ArgumentParser exits
 with error info when an error occurs
 ⁰
 def exit(self, status=0, message=None): View Source
-41    def exit(self, status=0, message=None):
-42        """Override to prevent shell exit when passing -h/--help switches."""
-43        if message:
-44            self._print_message(message, sys.stderr)
+42    def exit(self, status=0, message=None):
+43        """Override to prevent shell exit when passing -h/--help switches."""
+44        if message:
+45            self._print_message(message, sys.stderr)
 Override to prevent shell exit when passing -h/--help switches.
 ⁰
 def error(self, message): View Source
-46    def error(self, message):
-47        raise Exception(f"prog: {self.prog}, message: {message}")
+47    def error(self, message):
+48        raise Exception(f"prog: {self.prog}, message: {message}")
 error(message: string)
 Prints a usage message incorporating the message to stderr and exits.
 If you override this in a subclass, it should not return -- it should either
 exit or raise an exception.
 ⁰
 def parse_args(self, *args, **kwargs) -> argshell.argshell.Namespace: View
 Source
-49    def parse_args(self, *args, **kwargs) -> Namespace:
-50        parsed_args: Namespace = super().parse_args(*args, **kwargs)
-51        return parsed_args
+50    def parse_args(self, *args, **kwargs) -> Namespace:
+51        parsed_args: Namespace = super().parse_args(*args, **kwargs)
+52        return parsed_args
 ** Inherited Members **
   ⁰
 class ArgShell(cmd.Cmd): View Source
-_54class ArgShell(cmd.Cmd):
-_55    """Subclass this to create custom ArgShells."""
-_56
-_57    intro = "Entering argshell..."
-_58    prompt = "argshell>"
-_59
-_60    def do_quit(self, command: str):
-_61        """Quit shell."""
-_62        return True
-_63
-_64    def do_help(self, arg):
-_65        """List available commands with "help" or detailed help with "help
+_55class ArgShell(cmd.Cmd):
+_56    """Subclass this to create custom ArgShells."""
+_57
+_58    intro = "Entering argshell..."
+_59    prompt = "argshell>"
+_60
+_61    def do_quit(self, command: str):
+_62        """Quit shell."""
+_63        return True
+_64
+_65    def do_sys(self, command: str):
+_66        """Execute command with `os.system()`."""
+_67        os.system(command)
+_68
+_69    def do_help(self, arg):
+_70        """List available commands with "help" or detailed help with "help
 cmd".
-_66        If using 'help cmd' and the cmd is decorated with a parser, the
+_71        If using 'help cmd' and the cmd is decorated with a parser, the
 parser help will also be printed."""
-_67        if arg:
-_68            # XXX check arg syntax
-_69            try:
-_70                func = getattr(self, "help_" + arg)
-_71            except AttributeError:
-_72                try:
-_73                    func = getattr(self, "do_" + arg)
-_74                    doc = func.__doc__
-_75                    if doc:
-_76                        self.stdout.write("%s\n" % str(doc))
-_77                    # =========================Modification
+_72        if arg:
+_73            # XXX check arg syntax
+_74            try:
+_75                func = getattr(self, "help_" + arg)
+_76            except AttributeError:
+_77                try:
+_78                    func = getattr(self, "do_" + arg)
+_79                    doc = func.__doc__
+_80                    if doc:
+_81                        self.stdout.write("%s\n" % str(doc))
+_82                    # =========================Modification
 start=========================
-_78                    # Check for decorator and call decorated function with
+_83                    # Check for decorator and call decorated function with
 "--help"
-_79                    if hasattr(func, "__wrapped__"):
-_80                        self.stdout.write(
-_81                            f"Parser help for {func.__name__.replace
+_84                    if hasattr(func, "__wrapped__"):
+_85                        self.stdout.write(
+_86                            f"Parser help for {func.__name__.replace
 ('do_','')}:\n"
-_82                        )
-_83                        func("--help")
-_84                    if doc or hasattr(func, "__wrapped__"):
-_85                        return
-_86                    # =========================Modification
+_87                        )
+_88                        func("--help")
+_89                    if doc or hasattr(func, "__wrapped__"):
+_90                        return
+_91                    # =========================Modification
 stop=========================
-_87                except AttributeError:
-_88                    pass
-_89                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
-_90                return
-_91            func()
-_92        else:
-_93            names = self.get_names()
-_94            cmds_doc = []
-_95            cmds_undoc = []
-_96            topics = set()
-_97            for name in names:
-_98                if name[:5] == "help_":
-_99                    topics.add(name[5:])
-100            names.sort()
-101            # There can be duplicates if routines overridden
-102            prevname = ""
-103            for name in names:
-104                if name[:3] == "do_":
-105                    if name == prevname:
-106                        continue
-107                    prevname = name
-108                    cmd = name[3:]
-109                    if cmd in topics:
-110                        cmds_doc.append(cmd)
-111                        topics.remove(cmd)
-112                    elif getattr(self, name).__doc__:
-113                        cmds_doc.append(cmd)
-114                    else:
-115                        cmds_undoc.append(cmd)
-116            self.stdout.write("%s\n" % str(self.doc_leader))
-117            self.print_topics(self.doc_header, cmds_doc, 15, 80)
-118            self.print_topics(self.misc_header, sorted(topics), 15, 80)
-119            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
-120
-121    def cmdloop(self, intro=None):
-122        """Repeatedly issue a prompt, accept input, parse an initial prefix
-123        off the received input, and dispatch to action methods, passing them
-124        the remainder of the line as argument.
+_92                except AttributeError:
+_93                    pass
+_94                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
+_95                return
+_96            func()
+_97        else:
+_98            names = self.get_names()
+_99            cmds_doc = []
+100            cmds_undoc = []
+101            topics = set()
+102            for name in names:
+103                if name[:5] == "help_":
+104                    topics.add(name[5:])
+105            names.sort()
+106            # There can be duplicates if routines overridden
+107            prevname = ""
+108            for name in names:
+109                if name[:3] == "do_":
+110                    if name == prevname:
+111                        continue
+112                    prevname = name
+113                    cmd = name[3:]
+114                    if cmd in topics:
+115                        cmds_doc.append(cmd)
+116                        topics.remove(cmd)
+117                    elif getattr(self, name).__doc__:
+118                        cmds_doc.append(cmd)
+119                    else:
+120                        cmds_undoc.append(cmd)
+121            self.stdout.write("%s\n" % str(self.doc_leader))
+122            self.print_topics(self.doc_header, cmds_doc, 15, 80)
+123            self.print_topics(self.misc_header, sorted(topics), 15, 80)
+124            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
 125
-126        """
-127
-128        self.preloop()
-129        if self.use_rawinput and self.completekey:
-130            try:
-131                import readline
+126    def cmdloop(self, intro=None):
+127        """Repeatedly issue a prompt, accept input, parse an initial prefix
+128        off the received input, and dispatch to action methods, passing them
+129        the remainder of the line as argument.
+130
+131        """
 132
-133                self.old_completer = readline.get_completer()  # type:
+133        self.preloop()
+134        if self.use_rawinput and self.completekey:
+135            try:
+136                import readline
+137
+138                self.old_completer = readline.get_completer()  # type:
 ignore
-134                readline.set_completer(self.complete)  # type: ignore
-135                readline.parse_and_bind(self.completekey + ": complete")  #
+139                readline.set_completer(self.complete)  # type: ignore
+140                readline.parse_and_bind(self.completekey + ": complete")  #
 type: ignore
-136            except ImportError:
-137                pass
-138        try:
-139            if intro is not None:
-140                self.intro = intro
-141            if self.intro:
-142                self.stdout.write(str(self.intro) + "\n")
-143            stop = None
-144            while not stop:
-145                if self.cmdqueue:
-146                    line = self.cmdqueue.pop(0)
-147                else:
-148                    if self.use_rawinput:
-149                        try:
-150                            line = input(self.prompt)
-151                        except EOFError:
-152                            line = "EOF"
-153                    else:
-154                        self.stdout.write(self.prompt)
-155                        self.stdout.flush()
-156                        line = self.stdin.readline()
-157                        if not len(line):
-158                            line = "EOF"
-159                        else:
-160                            line = line.rstrip("\r\n")
-161                # ===========Modification start===========
-162                try:
-163                    line = self.precmd(line)
-164                    stop = self.onecmd(line)
-165                    stop = self.postcmd(stop, line)
-166                except Exception as e:
-167                    traceback.print_exc()
-168                # ===========Modification stop===========
-169            self.postloop()
-170        finally:
-171            if self.use_rawinput and self.completekey:
-172                try:
-173                    import readline
-174
-175                    readline.set_completer(self.old_completer)  # type:
+141            except ImportError:
+142                pass
+143        try:
+144            if intro is not None:
+145                self.intro = intro
+146            if self.intro:
+147                self.stdout.write(str(self.intro) + "\n")
+148            stop = None
+149            while not stop:
+150                if self.cmdqueue:
+151                    line = self.cmdqueue.pop(0)
+152                else:
+153                    if self.use_rawinput:
+154                        try:
+155                            line = input(self.prompt)
+156                        except EOFError:
+157                            line = "EOF"
+158                    else:
+159                        self.stdout.write(self.prompt)
+160                        self.stdout.flush()
+161                        line = self.stdin.readline()
+162                        if not len(line):
+163                            line = "EOF"
+164                        else:
+165                            line = line.rstrip("\r\n")
+166                # ===========Modification start===========
+167                try:
+168                    line = self.precmd(line)
+169                    stop = self.onecmd(line)
+170                    stop = self.postcmd(stop, line)
+171                except Exception as e:
+172                    traceback.print_exc()
+173                # ===========Modification stop===========
+174            self.postloop()
+175        finally:
+176            if self.use_rawinput and self.completekey:
+177                try:
+178                    import readline
+179
+180                    readline.set_completer(self.old_completer)  # type:
 ignore
-176                except ImportError:
-177                    pass
+181                except ImportError:
+182                    pass
 Subclass this to create custom ArgShells.
 ⁰
 def do_quit(self, command: str): View Source
-60    def do_quit(self, command: str):
-61        """Quit shell."""
-62        return True
+61    def do_quit(self, command: str):
+62        """Quit shell."""
+63        return True
 Quit shell.
 ⁰
+def do_sys(self, command: str): View Source
+65    def do_sys(self, command: str):
+66        """Execute command with `os.system()`."""
+67        os.system(command)
+Execute command with os.system().
+⁰
 def do_help(self, arg): View Source
-_64    def do_help(self, arg):
-_65        """List available commands with "help" or detailed help with "help
+_69    def do_help(self, arg):
+_70        """List available commands with "help" or detailed help with "help
 cmd".
-_66        If using 'help cmd' and the cmd is decorated with a parser, the
+_71        If using 'help cmd' and the cmd is decorated with a parser, the
 parser help will also be printed."""
-_67        if arg:
-_68            # XXX check arg syntax
-_69            try:
-_70                func = getattr(self, "help_" + arg)
-_71            except AttributeError:
-_72                try:
-_73                    func = getattr(self, "do_" + arg)
-_74                    doc = func.__doc__
-_75                    if doc:
-_76                        self.stdout.write("%s\n" % str(doc))
-_77                    # =========================Modification
+_72        if arg:
+_73            # XXX check arg syntax
+_74            try:
+_75                func = getattr(self, "help_" + arg)
+_76            except AttributeError:
+_77                try:
+_78                    func = getattr(self, "do_" + arg)
+_79                    doc = func.__doc__
+_80                    if doc:
+_81                        self.stdout.write("%s\n" % str(doc))
+_82                    # =========================Modification
 start=========================
-_78                    # Check for decorator and call decorated function with
+_83                    # Check for decorator and call decorated function with
 "--help"
-_79                    if hasattr(func, "__wrapped__"):
-_80                        self.stdout.write(
-_81                            f"Parser help for {func.__name__.replace
+_84                    if hasattr(func, "__wrapped__"):
+_85                        self.stdout.write(
+_86                            f"Parser help for {func.__name__.replace
 ('do_','')}:\n"
-_82                        )
-_83                        func("--help")
-_84                    if doc or hasattr(func, "__wrapped__"):
-_85                        return
-_86                    # =========================Modification
+_87                        )
+_88                        func("--help")
+_89                    if doc or hasattr(func, "__wrapped__"):
+_90                        return
+_91                    # =========================Modification
 stop=========================
-_87                except AttributeError:
-_88                    pass
-_89                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
-_90                return
-_91            func()
-_92        else:
-_93            names = self.get_names()
-_94            cmds_doc = []
-_95            cmds_undoc = []
-_96            topics = set()
-_97            for name in names:
-_98                if name[:5] == "help_":
-_99                    topics.add(name[5:])
-100            names.sort()
-101            # There can be duplicates if routines overridden
-102            prevname = ""
-103            for name in names:
-104                if name[:3] == "do_":
-105                    if name == prevname:
-106                        continue
-107                    prevname = name
-108                    cmd = name[3:]
-109                    if cmd in topics:
-110                        cmds_doc.append(cmd)
-111                        topics.remove(cmd)
-112                    elif getattr(self, name).__doc__:
-113                        cmds_doc.append(cmd)
-114                    else:
-115                        cmds_undoc.append(cmd)
-116            self.stdout.write("%s\n" % str(self.doc_leader))
-117            self.print_topics(self.doc_header, cmds_doc, 15, 80)
-118            self.print_topics(self.misc_header, sorted(topics), 15, 80)
-119            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
+_92                except AttributeError:
+_93                    pass
+_94                self.stdout.write("%s\n" % str(self.nohelp % (arg,)))
+_95                return
+_96            func()
+_97        else:
+_98            names = self.get_names()
+_99            cmds_doc = []
+100            cmds_undoc = []
+101            topics = set()
+102            for name in names:
+103                if name[:5] == "help_":
+104                    topics.add(name[5:])
+105            names.sort()
+106            # There can be duplicates if routines overridden
+107            prevname = ""
+108            for name in names:
+109                if name[:3] == "do_":
+110                    if name == prevname:
+111                        continue
+112                    prevname = name
+113                    cmd = name[3:]
+114                    if cmd in topics:
+115                        cmds_doc.append(cmd)
+116                        topics.remove(cmd)
+117                    elif getattr(self, name).__doc__:
+118                        cmds_doc.append(cmd)
+119                    else:
+120                        cmds_undoc.append(cmd)
+121            self.stdout.write("%s\n" % str(self.doc_leader))
+122            self.print_topics(self.doc_header, cmds_doc, 15, 80)
+123            self.print_topics(self.misc_header, sorted(topics), 15, 80)
+124            self.print_topics(self.undoc_header, cmds_undoc, 15, 80)
 List available commands with "help" or detailed help with "help cmd". If using
 'help cmd' and the cmd is decorated with a parser, the parser help will also be
 printed.
 ⁰
 def cmdloop(self, intro=None): View Source
-121    def cmdloop(self, intro=None):
-122        """Repeatedly issue a prompt, accept input, parse an initial prefix
-123        off the received input, and dispatch to action methods, passing them
-124        the remainder of the line as argument.
-125
-126        """
-127
-128        self.preloop()
-129        if self.use_rawinput and self.completekey:
-130            try:
-131                import readline
+126    def cmdloop(self, intro=None):
+127        """Repeatedly issue a prompt, accept input, parse an initial prefix
+128        off the received input, and dispatch to action methods, passing them
+129        the remainder of the line as argument.
+130
+131        """
 132
-133                self.old_completer = readline.get_completer()  # type:
+133        self.preloop()
+134        if self.use_rawinput and self.completekey:
+135            try:
+136                import readline
+137
+138                self.old_completer = readline.get_completer()  # type:
 ignore
-134                readline.set_completer(self.complete)  # type: ignore
-135                readline.parse_and_bind(self.completekey + ": complete")  #
+139                readline.set_completer(self.complete)  # type: ignore
+140                readline.parse_and_bind(self.completekey + ": complete")  #
 type: ignore
-136            except ImportError:
-137                pass
-138        try:
-139            if intro is not None:
-140                self.intro = intro
-141            if self.intro:
-142                self.stdout.write(str(self.intro) + "\n")
-143            stop = None
-144            while not stop:
-145                if self.cmdqueue:
-146                    line = self.cmdqueue.pop(0)
-147                else:
-148                    if self.use_rawinput:
-149                        try:
-150                            line = input(self.prompt)
-151                        except EOFError:
-152                            line = "EOF"
-153                    else:
-154                        self.stdout.write(self.prompt)
-155                        self.stdout.flush()
-156                        line = self.stdin.readline()
-157                        if not len(line):
-158                            line = "EOF"
-159                        else:
-160                            line = line.rstrip("\r\n")
-161                # ===========Modification start===========
-162                try:
-163                    line = self.precmd(line)
-164                    stop = self.onecmd(line)
-165                    stop = self.postcmd(stop, line)
-166                except Exception as e:
-167                    traceback.print_exc()
-168                # ===========Modification stop===========
-169            self.postloop()
-170        finally:
-171            if self.use_rawinput and self.completekey:
-172                try:
-173                    import readline
-174
-175                    readline.set_completer(self.old_completer)  # type:
+141            except ImportError:
+142                pass
+143        try:
+144            if intro is not None:
+145                self.intro = intro
+146            if self.intro:
+147                self.stdout.write(str(self.intro) + "\n")
+148            stop = None
+149            while not stop:
+150                if self.cmdqueue:
+151                    line = self.cmdqueue.pop(0)
+152                else:
+153                    if self.use_rawinput:
+154                        try:
+155                            line = input(self.prompt)
+156                        except EOFError:
+157                            line = "EOF"
+158                    else:
+159                        self.stdout.write(self.prompt)
+160                        self.stdout.flush()
+161                        line = self.stdin.readline()
+162                        if not len(line):
+163                            line = "EOF"
+164                        else:
+165                            line = line.rstrip("\r\n")
+166                # ===========Modification start===========
+167                try:
+168                    line = self.precmd(line)
+169                    stop = self.onecmd(line)
+170                    stop = self.postcmd(stop, line)
+171                except Exception as e:
+172                    traceback.print_exc()
+173                # ===========Modification stop===========
+174            self.postloop()
+175        finally:
+176            if self.use_rawinput and self.completekey:
+177                try:
+178                    import readline
+179
+180                    readline.set_completer(self.old_completer)  # type:
 ignore
-176                except ImportError:
-177                    pass
+181                except ImportError:
+182                    pass
 Repeatedly issue a prompt, accept input, parse an initial prefix off the
 received input, and dispatch to action methods, passing them the remainder of
 the line as argument.
 ** Inherited Members **
   ⁰
 def with_parser(
 parser: Callable[..., argshell.argshell.ArgShellParser],
 post_parsers: list[typing.Callable[[argshell.argshell.Namespace],
 argshell.argshell.Namespace]] = []) -> Callable[[Callable[[Any,
 argshell.argshell.Namespace], Any]], Callable[[Any, str], Any]]: View Source
-180def with_parser(
-181    parser: Callable[..., ArgShellParser],
-182    post_parsers: list[Callable[[Namespace], Namespace]] = [],
-183) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
-184    """Decorate a 'do_*' function in an argshell.ArgShell class with this
+185def with_parser(
+186    parser: Callable[..., ArgShellParser],
+187    post_parsers: list[Callable[[Namespace], Namespace]] = [],
+188) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
+189    """Decorate a 'do_*' function in an argshell.ArgShell class with this
 function to pass an argshell.Namespace object to the decorated function instead
 of a string.
-185
-186    :param parser: A function that creates an argshell.ArgShellParser
+190
+191    :param parser: A function that creates an argshell.ArgShellParser
 instance, adds arguments to it, and returns the parser.
-187
-188    :param post_parsers: An optional list of functions to execute where each
+192
+193    :param post_parsers: An optional list of functions to execute where each
 function takes an argshell.Namespace instance and returns an argshell.Namespace
 instance.
-189        'post_parser' functions are executed in the order they are supplied.
-190
-191    >>> def get_parser() -> argshell.ArgShellParser:
-192    >>>     parser = argshell.ArgShellParser()
-193    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
+194        'post_parser' functions are executed in the order they are supplied.
+195
+196    >>> def get_parser() -> argshell.ArgShellParser:
+197    >>>     parser = argshell.ArgShellParser()
+198    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
 of first and last names to print.")
-194    >>>     parser.add_argument("-i", "--initials", action="store_true",
+199    >>>     parser.add_argument("-i", "--initials", action="store_true",
 help="Print the initials instead of the full name.")
-195    >>>     return parser
-196    >>>
-197    >>> # Convert list of first and last names to a list of tuples
-198    >>> def names_list_to_tuples(args: argshell.Namespace) -
+200    >>>     return parser
+201    >>>
+202    >>> # Convert list of first and last names to a list of tuples
+203    >>> def names_list_to_tuples(args: argshell.Namespace) -
 > argshell.Namespace:
-199    >>>     args.names = [(first, last) for first, last in zip(args.names[::
+204    >>>     args.names = [(first, last) for first, last in zip(args.names[::
 2], args.names[1::2])]
-200    >>>     if args.initials:
-201    >>>         args.names = [(name[0][0], name[1][0]) for name in
+205    >>>     if args.initials:
+206    >>>         args.names = [(name[0][0], name[1][0]) for name in
 args.names]
-202    >>>     return args
-203    >>>
-204    >>> def capitalize_names(args: argshell.Namespace) -
+207    >>>     return args
+208    >>>
+209    >>> def capitalize_names(args: argshell.Namespace) -
 > argshell.Namespace:
-205    >>>     args.names = [name.capitalize() for name in args.names]
-206    >>>     return args
-207    >>>
-208    >>> class NameShell(ArgShell):
-209    >>>     intro = "Entering nameshell..."
-210    >>>     prompt = "nameshell>"
-211    >>>
-212    >>>     @with_parser(get_parser, [capitalize_names,
+210    >>>     args.names = [name.capitalize() for name in args.names]
+211    >>>     return args
+212    >>>
+213    >>> class NameShell(ArgShell):
+214    >>>     intro = "Entering nameshell..."
+215    >>>     prompt = "nameshell>"
+216    >>>
+217    >>>     @with_parser(get_parser, [capitalize_names,
 names_list_to_tuples])
-213    >>>     def do_printnames(self, args: argshell.Namespace):
-214    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
+218    >>>     def do_printnames(self, args: argshell.Namespace):
+219    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
 sep="\\n")
-215    >>>
-216    >>> NameShell().cmdloop()
-217    >>> Entering nameshell...
-218    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+220    >>>
+221    >>> NameShell().cmdloop()
+222    >>> Entering nameshell...
+223    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno
-219    >>> Karl Marx
-220    >>> Fred Hampton
-221    >>> Emma Goldman
-222    >>> Angela Davis
-223    >>> Nestor Makhno
-224    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+224    >>> Karl Marx
+225    >>> Fred Hampton
+226    >>> Emma Goldman
+227    >>> Angela Davis
+228    >>> Nestor Makhno
+229    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno -i
-225    >>> K M
-226    >>> F H
-227    >>> E G
-228    >>> A D
-229    >>> N M"""
-230
-231    def decorator(
-232        func: Callable[[Any, Namespace], Any | None]
-233    ) -> Callable[[Any, str], Any]:
-234        @wraps(func)
-235        def inner(self: Any, command: str) -> Any:
-236            try:
-237                args = parser().parse_args(shlex.split(command))
-238            except Exception as e:
-239                # On parser error, print help and skip post_parser and func
+230    >>> K M
+231    >>> F H
+232    >>> E G
+233    >>> A D
+234    >>> N M"""
+235
+236    def decorator(
+237        func: Callable[[Any, Namespace], Any | None]
+238    ) -> Callable[[Any, str], Any]:
+239        @wraps(func)
+240        def inner(self: Any, command: str) -> Any:
+241            try:
+242                args = parser().parse_args(shlex.split(command))
+243            except Exception as e:
+244                # On parser error, print help and skip post_parser and func
 execution
-240                if "the following arguments are required" not in str(e):
-241                    print(f"ERROR: {e}")
-242                if "-h" not in command and "--help" not in command:
-243                    try:
-244                        args = parser().parse_args(["--help"])
-245                    except Exception as e:
-246                        pass
-247                return None
-248            # Don't execute function, only print parser help
-249            if "-h" in command or "--help" in command:
-250                return None
-251            for post_parser in post_parsers:
-252                args = post_parser(args)
-253
-254            return func(self, args)
-255
-256        return inner
-257
-258    return decorator
+245                if "the following arguments are required" not in str(e):
+246                    print(f"ERROR: {e}")
+247                if "-h" not in command and "--help" not in command:
+248                    try:
+249                        args = parser().parse_args(["--help"])
+250                    except Exception as e:
+251                        pass
+252                return None
+253            # Don't execute function, only print parser help
+254            if "-h" in command or "--help" in command:
+255                return None
+256            for post_parser in post_parsers:
+257                args = post_parser(args)
+258
+259            return func(self, args)
+260
+261        return inner
+262
+263    return decorator
 Decorate a 'do_*' function in an argshell.ArgShell class with this function to
 pass an argshell.Namespace object to the decorated function instead of a
 string.
 * Parameters *
     * parser: A function that creates an argshell.ArgShellParser instance, adds
       arguments to it, and returns the parser.
     * post_parsers: An optional list of functions to execute where each
```

### Comparing `argshell-1.1.0/src/argshell/argshell.py` & `argshell-1.2.0/src/argshell/argshell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import cmd
+import os
 import shlex
 import sys
 import traceback
 from functools import wraps
 from typing import Any, Callable
 
 
@@ -56,14 +57,18 @@
     intro = "Entering argshell..."
     prompt = "argshell>"
 
     def do_quit(self, command: str):
         """Quit shell."""
         return True
 
+    def do_sys(self, command: str):
+        """Execute command with `os.system()`."""
+        os.system(command)
+
     def do_help(self, arg):
         """List available commands with "help" or detailed help with "help cmd".
         If using 'help cmd' and the cmd is decorated with a parser, the parser help will also be printed."""
         if arg:
             # XXX check arg syntax
             try:
                 func = getattr(self, "help_" + arg)
```

### Comparing `argshell-1.1.0/LICENSE.txt` & `argshell-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argshell-1.1.0/README.md` & `argshell-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `argshell-1.1.0/pyproject.toml` & `argshell-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6172 6773 6865 6c6c 220d 0a64 6573   "argshell"..des
 00000070: 6372 6970 7469 6f6e 203d 2022 496e 7465  cription = "Inte
 00000080: 6772 6174 6573 2074 6865 2061 7267 7061  grates the argpa
 00000090: 7273 6520 616e 6420 636d 6420 6d6f 6475  rse and cmd modu
 000000a0: 6c65 732e 220d 0a76 6572 7369 6f6e 203d  les."..version =
-000000b0: 2022 312e 312e 3022 0d0a 7265 7175 6972   "1.1.0"..requir
+000000b0: 2022 312e 322e 3022 0d0a 7265 7175 6972   "1.2.0"..requir
 000000c0: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
 000000d0: 2e31 3022 0d0a 6465 7065 6e64 656e 6369  .10"..dependenci
 000000e0: 6573 203d 205b 2270 7974 6573 7422 5d0d  es = ["pytest"].
 000000f0: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
 00000100: 452e 6d64 220d 0a6b 6579 776f 7264 7320  E.md"..keywords 
 00000110: 3d20 5b22 6172 6770 6172 7365 222c 2022  = ["argparse", "
 00000120: 636d 6422 2c20 2273 6865 6c6c 222c 2022  cmd", "shell", "
```

### Comparing `argshell-1.1.0/PKG-INFO` & `argshell-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argshell
-Version: 1.1.0
+Version: 1.2.0
 Summary: Integrates the argparse and cmd modules.
 Project-URL: Homepage, https://github.com/matt-manes/argshell
 Project-URL: Documentation, https://github.com/matt-manes/argshell/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/argshell/tree/main/src/argshell
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: argparse,cmd,commandline,shell,terminal
```

