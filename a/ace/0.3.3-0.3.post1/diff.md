# Comparing `tmp/ace-0.3.3.tar.gz` & `tmp/ace-0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ace-0.3.3.tar", last modified: Wed May  3 06:14:20 2023, max compression
+gzip compressed data, was "dist/ace-0.3.post1.tar", last modified: Mon Feb 15 20:40:54 2016, max compression
```

## Comparing `ace-0.3.3.tar` & `ace-0.3.post1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.476596 ace-0.3.3/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1084 2023-05-03 05:59:35.000000 ace-0.3.3/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)     7765 2023-05-03 06:14:20.476596 ace-0.3.3/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     6677 2023-05-03 05:59:35.000000 ace-0.3.3/README.rst
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.472596 ace-0.3.3/ace/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1517 2023-05-03 05:59:35.000000 ace-0.3.3/ace/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    10049 2023-05-03 06:05:57.000000 ace-0.3.3/ace/ace.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3627 2023-05-03 05:59:35.000000 ace-0.3.3/ace/model.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.476596 ace-0.3.3/ace/samples/
--rw-rw-r--   0 nick      (1000) nick      (1000)       61 2023-05-03 05:59:35.000000 ace-0.3.3/ace/samples/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1713 2023-05-03 05:59:35.000000 ace-0.3.3/ace/samples/breiman85.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1184 2023-05-03 05:59:35.000000 ace-0.3.3/ace/samples/smoother_friedman82.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      866 2023-05-03 05:59:35.000000 ace-0.3.3/ace/samples/supersmoother_friedman82.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      870 2023-05-03 05:59:35.000000 ace-0.3.3/ace/samples/wang04.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12949 2023-05-03 05:59:35.000000 ace-0.3.3/ace/smoother.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7253 2023-05-03 05:59:35.000000 ace-0.3.3/ace/supersmoother.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.476596 ace-0.3.3/ace/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)       31 2023-05-03 05:59:35.000000 ace-0.3.3/ace/tests/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2261 2023-05-03 05:59:35.000000 ace-0.3.3/ace/tests/test_ace.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1729 2023-05-03 05:59:35.000000 ace-0.3.3/ace/tests/test_model.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4339 2023-05-03 05:59:35.000000 ace-0.3.3/ace/tests/test_smoother.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.476596 ace-0.3.3/ace/validation/
--rw-rw-r--   0 nick      (1000) nick      (1000)       23 2023-05-03 05:59:35.000000 ace-0.3.3/ace/validation/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6082 2023-05-03 05:59:35.000000 ace-0.3.3/ace/validation/validate_smoothers.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-03 06:14:20.472596 ace-0.3.3/ace.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     7765 2023-05-03 06:14:20.000000 ace-0.3.3/ace.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      543 2023-05-03 06:14:20.000000 ace-0.3.3/ace.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-03 06:14:20.000000 ace-0.3.3/ace.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-05-03 06:14:20.000000 ace-0.3.3/ace.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        4 2023-05-03 06:14:20.000000 ace-0.3.3/ace.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-03 06:14:20.476596 ace-0.3.3/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)     1359 2023-05-03 06:10:02.000000 ace-0.3.3/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1128 2016-02-15 20:35:04.000000 ace-0.3.post1/setup.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2016-02-15 20:40:54.000000 ace-0.3.post1/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)     8204 2016-02-15 20:40:54.000000 ace-0.3.post1/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6083 2016-02-15 20:19:18.000000 ace-0.3.post1/README.rst
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        4 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     8204 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)       12 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      564 2016-02-15 20:40:54.000000 ace-0.3.post1/ace.egg-info/SOURCES.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/ace/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/ace/validation/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      898 2016-02-15 20:33:22.000000 ace-0.3.post1/ace/validation/run_supsmu.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2014-10-12 19:42:01.000000 ace-0.3.post1/ace/validation/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5715 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/validation/validate_smoothers.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3448 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/model.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    10182 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/ace.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/ace/samples/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      859 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/samples/supersmoother_friedman82.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       61 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/samples/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1210 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/samples/smoother_friedman82.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      755 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/samples/breiman85.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      845 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/samples/wang04.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2016-02-15 20:40:54.000000 ace-0.3.post1/ace/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4312 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/tests/test_smoother.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       31 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/tests/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1671 2014-11-02 05:05:09.000000 ace-0.3.post1/ace/tests/test_model.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2189 2016-02-15 20:19:18.000000 ace-0.3.post1/ace/tests/test_ace.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1401 2016-02-15 20:30:49.000000 ace-0.3.post1/ace/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13015 2014-11-01 23:30:56.000000 ace-0.3.post1/ace/smoother.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7192 2014-11-01 23:30:56.000000 ace-0.3.post1/ace/supersmoother.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ace-0.3.3/PKG-INFO` & `ace-0.3.post1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,180 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ace
-Version: 0.3.3
+Version: 0.3.post1
 Summary: Non-parametric multivariate regressions by Alternating Conditional Expectations
 Home-page: https://github.com/partofthething/ace
 Author: Nick Touran
 Author-email: ace@partofthething.com
 License: MIT
+Description: 
+        The ace Package
+        ===============
+        
+        ace is an implementation of the Alternating Conditional Expectation (ACE) algorithm [Breiman85]_,
+        which can be used to find otherwise difficult-to-find relationships between predictors
+        and responses and as a multivariate regression tool.
+        
+        The code for this project, as well as the issue tracker, etc. is
+        `hosted on GitHub <https://github.com/partofthething/ace>`_.
+        The documentation is hosted at http://partofthething.com/ace.
+        
+        What is it?
+        -----------
+        ACE can be used for a variety of purposes. With it, you can:
+        
+         - build easy-to-evaluate surrogate models of data. For example, if you are optimizing input
+           parameters to a complex and long-running simulation, you can feed the results of a parameter
+           sweep into ACE to get a model that will instantly give you predictions of results of any
+           combination of input within the parameter range.
+        
+         - expose interesting and meaningful relations between predictors and responses from complicated
+           data sets. For instance, if you have survey results from 1000 people and you and you want to
+           see how one answer is related to a bunch of others, ACE will help you.
+        
+        The fascinating thing about ACE is that it is a *non-parametric* multivariate regression
+        tool. This means that it doesn't make any assumptions about the functional form of the data.
+        You may be used to fitting polynomials or lines to data. Well, ACE doesn't do that. It
+        uses an iteration with a variable-span scatterplot smoother (implementing local least
+        squares estimates) to figure out the structure of your data. As you'll see, that
+        turns out to be a powerful difference.
+        
+        Installing it
+        -------------
+        ace is available in the `Python Package Index <https://pypi.python.org/pypi/ace/>`_,
+        and can be installed simply with the following.
+        
+        On Linux::
+        
+        	sudo pip install ace
+        
+        On Windows, use::
+        
+        	pip install ace
+        
+        or use the `GUI installer <http://partofthething.com/ace/builds/ace-0.2-1.win32.exe>`_.
+        
+        Directly from source::
+        
+        	git clone git@github.com:partofthething/ace.git
+        	cd ace
+        	python setup.py install
+        
+        .. note::
+        
+        	If you don't have git, you can just download the source directly from
+        	`here <https://github.com/partofthething/ace/archive/master.zip>`_.
+        
+        You can verify that the installation completed successfully by running the automated test
+        suite in the install directory::
+        
+        	python -m unittest discover -bv
+        
+        Using it
+        --------
+        To use, get some sample data:
+        
+        .. code:: python
+        
+            from ace.samples import wang04
+            x, y = wang04.build_sample_ace_problem_wang04(N=200)
+        
+        and run:
+        
+        .. code:: python
+        
+            from ace import model
+            myace = model.Model()
+            myace.build_model_from_xy(x, y)
+            myace.eval([0.1, 0.2, 0.5, 0.3, 0.5])
+        
+        For some plotting (matplotlib required), try:
+        
+        .. code:: python
+        
+            from ace import ace
+            ace.plot_transforms(myace.ace, fname = 'mytransforms.pdf')
+            myace.ace.write_transforms_to_file(fname = 'mytransforms.txt')
+        
+        Note that you could alternatively have loaded your data from a whitespace delimited
+        text file:
+        
+        .. code:: python
+        
+        	myace.build_model_from_txt(fname = 'myinput.txt')
+        
+        .. warning:: The more data points ACE is given as input, the better the results will be.
+        			 Be careful with less than 50 data points or so.
+        
+        Demo
+        ----
+        A clear demonstration of ace is available in the
+        `Sample ACE Problems <http://partofthething.com/ace/samples.html>`_ section.
+        
+        Other details
+        -------------
+        This implementation of ACE isn't as fast as the original FORTRAN version, but it can
+        still crunch through a problem with 5 independent variables having 1000 observations each
+        in on the order of 15 seconds. Not bad.
+        
+        ace also contains a pure-Python implementation of Friedman's SuperSmoother [Friedman82]_,
+        the variable-span smoother mentioned above. This can be useful on its own
+        for smoothing scatterplot data.
+        
+        History
+        -------
+        The ACE algorithm was published in 1985 by Breiman and Friedman [Breiman85]_, and the original
+        FORTRAN source code is available from `Friedman's webpage <http://statweb.stanford.edu/~jhf/>`_.
+        
+        Motivation
+        ----------
+        Before this package, the ACE algorithm has only been available in Python by using the rpy2 module
+        to load in the acepack package of the R statistical language. This package is a pure-Python
+        re-write of the ACE algorithm based on the original publication, using modern software practices.
+        This package is slower than the original FORTRAN code, but it is easier to understand. This package
+        should be suitable for medium-weight data and as a learning tool.
+        
+        For the record, it is also quite easy to run the original FORTRAN code in Python using f2py.
+        
+        About the Author
+        ----------------
+        This package was originated by Nick Touran, a nuclear engineer specializing in reactor physics.
+        He was exposed to ACE by his thesis advisor, Professor John Lee, and used it in his
+        Ph.D. dissertation to evaluate objective functions in a multidisciplinary
+        design optimization study of nuclear reactor cores [Touran12]_.
+        
+        License
+        -------
+        This package is released under the MIT License, reproduced
+        `here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
+        
+        References
+        ----------
+        .. [Breiman85] L. BREIMAN and J. H. FRIEDMAN, "Estimating optimal transformations for multiple regression and
+           correlation," Journal of the American Statistical Association, 80, 580 (1985).
+           `[Link1] <http://www.jstor.org/discover/10.2307/2288477?uid=2&uid=4&sid=21104902100507>`_
+        
+        .. [Friedman82] J. H. FRIEDMAN and W. STUETZLE, "Smoothing of scatterplots," ORION-003, Stanford
+           University, (1982). `[Link2] <http://www.slac.stanford.edu/cgi-wrap/getdoc/slac-pub-3013.pdf>`_
+        
+        .. [Wang04] D. WANG and M. MURPHY, "Estimating optimal transformations for multiple regression using the
+           ACE algorithm," Journal of Data Science, 2, 329 (2004).
+           `[Link3] <http://www.jds-online.com/files/JDS-156.pdf>`_
+        
+        .. [Touran12] N. TOURAN, "A Modal Expansion Equilibrium Cycle Perturbation Method for
+           Optimizing High Burnup Fast Reactors," Ph.D. dissertation, Univ. of Michigan, (2012).
+           `[The Thesis] <http://deepblue.lib.umich.edu/bitstream/handle/2027.42/95981/ntouran_1.pdf?sequence=1>`_
+        
+        
+        
 Keywords: regression ace multivariate statistics
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
-===============
-The ace Package
-===============
-
-.. image:: https://travis-ci.org/partofthething/ace.svg?branch=develop
-    :target: https://travis-ci.org/partofthething/ace
-    
-ace is an implementation of the Alternating Conditional Expectation (ACE) algorithm [Breiman85]_,
-which can be used to find otherwise difficult-to-find relationships between predictors
-and responses and as a multivariate regression tool.
-
-The code for this project, as well as the issue tracker, etc. is
-`hosted on GitHub <https://github.com/partofthething/ace>`_.
-The documentation is hosted at http://partofthething.com/ace.
-
-
-What is it?
------------
-ACE can be used for a variety of purposes. With it, you can:
-
- - build easy-to-evaluate surrogate models of data. For example, if you are optimizing input
-   parameters to a complex and long-running simulation, you can feed the results of a parameter
-   sweep into ACE to get a model that will instantly give you predictions of results of any
-   combination of input within the parameter range.
-
- - expose interesting and meaningful relations between predictors and responses from complicated
-   data sets. For instance, if you have survey results from 1000 people and you and you want to
-   see how one answer is related to a bunch of others, ACE will help you.
-
-The fascinating thing about ACE is that it is a *non-parametric* multivariate regression
-tool. This means that it doesn't make any assumptions about the functional form of the data.
-You may be used to fitting polynomials or lines to data. Well, ACE doesn't do that. It
-uses an iteration with a variable-span scatterplot smoother (implementing local least
-squares estimates) to figure out the structure of your data. As you'll see, that
-turns out to be a powerful difference.
-
-Installing it
--------------
-ace is available in the `Python Package Index <https://pypi.python.org/pypi/ace/>`_,
-and can be installed simply with the following.
-
-On Linux::
-
-	sudo pip install ace
-
-On Windows, use::
-
-	pip install ace
-
-Directly from source::
-
-	git clone git@github.com:partofthething/ace.git
-	cd ace
-	python setup.py install
-
-.. note::
-
-	If you don't have git, you can just download the source directly from
-	`here <https://github.com/partofthething/ace/archive/master.zip>`_.
-
-You can verify that the installation completed successfully by running the automated test
-suite in the install directory::
-
-	python -m unittest discover -bv
-
-Using it
---------
-To use, get some sample data:
-
-.. code:: python
-
-    from ace.samples import wang04
-    x, y = wang04.build_sample_ace_problem_wang04(N=200)
-
-and run:
-
-.. code:: python
-
-    from ace import model
-    myace = model.Model()
-    myace.build_model_from_xy(x, y)
-    myace.eval([0.1, 0.2, 0.5, 0.3, 0.5])
-
-For some plotting (matplotlib required), try:
-
-.. code:: python
-
-    from ace import ace
-    ace.plot_transforms(myace.ace, fname = 'mytransforms.pdf')
-    myace.ace.write_transforms_to_file(fname = 'mytransforms.txt')
-
-Note that you could alternatively have loaded your data from a whitespace delimited
-text file:
-
-.. code:: python
-
-	myace.build_model_from_txt(fname = 'myinput.txt')
-
-.. warning:: The more data points ACE is given as input, the better the results will be.
-			 Be careful with less than 50 data points or so.
-
-Demo
-----
-A combination of various functions with noise is shown below:
-
-.. have to use full path here to work in built docs and github-rendered README
-
-.. image:: https://partofthething.com/ace/_static/ace_input_wang04.png
-	   :alt: Plot of the input data, which is all over the place
-
-Given just those points and zero knowledge of the underlying functions, ACE comes back
-with this:
-
-.. image:: https://partofthething.com/ace/_static/ace_transforms_wang04.png
-	:alt: Plot of the output transforms, which clearly show the underlying structure
-
-
-A longer version of this demo is available in the
-`Sample ACE Problems <http://partofthething.com/ace/samples.html>`_ section.
-
-Other details
--------------
-This implementation of ACE isn't as fast as the original FORTRAN version, but it can
-still crunch through a problem with 5 independent variables having 1000 observations each
-in on the order of 15 seconds. Not bad.
-
-ace also contains a pure-Python implementation of Friedman's SuperSmoother [Friedman82]_,
-the variable-span smoother mentioned above. This can be useful on its own
-for smoothing scatterplot data.
-
-History
--------
-The ACE algorithm was published in 1985 by Breiman and Friedman [Breiman85]_, and the original
-FORTRAN source code is available from `Friedman's webpage <http://statweb.stanford.edu/~jhf/>`_.
-
-Motivation
-----------
-Before this package, the ACE algorithm has only been available in Python by using the rpy2 module
-to load in the acepack package of the R statistical language. This package is a pure-Python
-re-write of the ACE algorithm based on the original publication, using modern software practices.
-This package is slower than the original FORTRAN code, but it is easier to understand. This package
-should be suitable for medium-weight data and as a learning tool.
-
-For the record, it is also quite easy to run the original FORTRAN code in Python using f2py.
-
-About the Author
-----------------
-This package was originated by Nick Touran, a nuclear engineer specializing in reactor physics.
-He was exposed to ACE by his thesis advisor, Professor John Lee, and used it in his
-Ph.D. dissertation to evaluate objective functions in a multidisciplinary
-design optimization study of nuclear reactor cores [Touran12]_.
-
-License
--------
-This package is released under the MIT License, `reproduced
-here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
-
-References
-----------
-.. [Breiman85] L. BREIMAN and J. H. FRIEDMAN, "Estimating optimal transformations for multiple regression and
-   correlation," Journal of the American Statistical Association, 80, 580 (1985).
-   `[Link1] <http://www.jstor.org/discover/10.2307/2288477?uid=2&uid=4&sid=21104902100507>`_
-
-.. [Friedman82] J. H. FRIEDMAN and W. STUETZLE, "Smoothing of scatterplots," ORION-003, Stanford
-   University, (1982). `[Link2] <http://www.slac.stanford.edu/cgi-wrap/getdoc/slac-pub-3013.pdf>`_
-
-.. [Wang04] D. WANG and M. MURPHY, "Estimating optimal transformations for multiple regression using the
-   ACE algorithm," Journal of Data Science, 2, 329 (2004).
-   `[Link3] <http://www.jds-online.com/files/JDS-156.pdf>`_
-
-.. [Touran12] N. TOURAN, "A Modal Expansion Equilibrium Cycle Perturbation Method for
-   Optimizing High Burnup Fast Reactors," Ph.D. dissertation, Univ. of Michigan, (2012).
-   `[The Thesis] <http://deepblue.lib.umich.edu/bitstream/handle/2027.42/95981/ntouran_1.pdf?sequence=1>`_
-
-
```

### Comparing `ace-0.3.3/README.rst` & `ace-0.3.post1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-===============
+
 The ace Package
 ===============
 
-.. image:: https://travis-ci.org/partofthething/ace.svg?branch=develop
-    :target: https://travis-ci.org/partofthething/ace
-    
 ace is an implementation of the Alternating Conditional Expectation (ACE) algorithm [Breiman85]_,
 which can be used to find otherwise difficult-to-find relationships between predictors
 and responses and as a multivariate regression tool.
 
 The code for this project, as well as the issue tracker, etc. is
 `hosted on GitHub <https://github.com/partofthething/ace>`_.
 The documentation is hosted at http://partofthething.com/ace.
 
-
 What is it?
 -----------
 ACE can be used for a variety of purposes. With it, you can:
 
  - build easy-to-evaluate surrogate models of data. For example, if you are optimizing input
    parameters to a complex and long-running simulation, you can feed the results of a parameter
    sweep into ACE to get a model that will instantly give you predictions of results of any
@@ -43,14 +39,16 @@
 
 	sudo pip install ace
 
 On Windows, use::
 
 	pip install ace
 
+or use the `GUI installer <http://partofthething.com/ace/builds/ace-0.2-1.win32.exe>`_.
+
 Directly from source::
 
 	git clone git@github.com:partofthething/ace.git
 	cd ace
 	python setup.py install
 
 .. note::
@@ -97,29 +95,15 @@
 	myace.build_model_from_txt(fname = 'myinput.txt')
 
 .. warning:: The more data points ACE is given as input, the better the results will be.
 			 Be careful with less than 50 data points or so.
 
 Demo
 ----
-A combination of various functions with noise is shown below:
-
-.. have to use full path here to work in built docs and github-rendered README
-
-.. image:: https://partofthething.com/ace/_static/ace_input_wang04.png
-	   :alt: Plot of the input data, which is all over the place
-
-Given just those points and zero knowledge of the underlying functions, ACE comes back
-with this:
-
-.. image:: https://partofthething.com/ace/_static/ace_transforms_wang04.png
-	:alt: Plot of the output transforms, which clearly show the underlying structure
-
-
-A longer version of this demo is available in the
+A clear demonstration of ace is available in the
 `Sample ACE Problems <http://partofthething.com/ace/samples.html>`_ section.
 
 Other details
 -------------
 This implementation of ACE isn't as fast as the original FORTRAN version, but it can
 still crunch through a problem with 5 independent variables having 1000 observations each
 in on the order of 15 seconds. Not bad.
@@ -148,16 +132,16 @@
 This package was originated by Nick Touran, a nuclear engineer specializing in reactor physics.
 He was exposed to ACE by his thesis advisor, Professor John Lee, and used it in his
 Ph.D. dissertation to evaluate objective functions in a multidisciplinary
 design optimization study of nuclear reactor cores [Touran12]_.
 
 License
 -------
-This package is released under the MIT License, `reproduced
-here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
+This package is released under the MIT License, reproduced
+`here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
 
 References
 ----------
 .. [Breiman85] L. BREIMAN and J. H. FRIEDMAN, "Estimating optimal transformations for multiple regression and
    correlation," Journal of the American Statistical Association, 80, 580 (1985).
    `[Link1] <http://www.jstor.org/discover/10.2307/2288477?uid=2&uid=4&sid=21104902100507>`_
```

### Comparing `ace-0.3.3/ace/__init__.py` & `ace-0.3.post1/ace/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-ace is a multivariate regression tool that solves alternating conditional expectations.
+ace is a multivariate regression tool that solves alternating conditional expectations
 
 See full documentation at http://partofthething.com/ace
 
 To use, get some sample data::
 
     from ace.samples import wang04
     x, y = wang04.build_sample_ace_problem_wang04(N=200)
@@ -18,35 +18,35 @@
 For some plotting (matplotlib required), try::
 
     from ace import ace
     ace.plot_transforms(myace, fname = 'mytransforms.pdf')
     myace.ace.write_transforms_to_file(fname = 'mytransforms.txt')
 
 """
-
-import os.path
-from pkg_resources import get_distribution, DistributionNotFound
-
 def _get_version():
-    """
-    Groan single sourcing versions is a huge pain.
-
-    For now we have to manually sync it between here and setup.py (for doc build)
-
-    https://packaging.python.org/guides/single-sourcing-package-version/
-    """
+    from pkg_resources import get_distribution, DistributionNotFound
+    import os.path
     try:
         _dist = get_distribution('ace')
         # Normalize case for Windows systems
-        _dist_loc = os.path.normcase(_dist.location)  # pylint: disable=no-member
+        _dist_loc = os.path.normcase(_dist.location)
         _here = os.path.normcase(__file__)
         if not _here.startswith(os.path.join(_dist_loc, 'ace')):
             # not installed, but there is another version that *is*
             raise DistributionNotFound
     except DistributionNotFound:
-        version = '0.3.2'
+        version = 'Please install ace with setup.py'
     else:
-        version = _dist.version  # pylint: disable=no-member
+        version = _dist.version
 
     return version
 
 __version__ = _get_version()
+
+from . import ace
+from . import model
+from . import smoother
+from . import supersmoother
+from . import samples
+from . import tests
+
+
```

### Comparing `ace-0.3.3/ace/ace.py` & `ace-0.3.post1/ace/ace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-r"""
-The Alternating Condtional Expectation (ACE) algorithm.
+r'''
+The Alternating Condtional Expectation (ACE) algorithm
 
 ACE was invented by L. Breiman and J. Friedman [Breiman85]_. It is a powerful
 way to perform multidimensional regression without assuming
 any functional form of the model. Given a data set:
 
     :math:`y = f(X)`
 
@@ -11,81 +11,85 @@
 will tell you how :math:`y` varies vs. each of the individual independents :math:`xi`.
 This can be used to:
 
     * Understand the relative shape and magnitude of y's dependence on each xi
     * Produce a lightweight surrogate model of a more complex response
     * other stuff
 
-"""
+'''
 
 import numpy
 try:
     from matplotlib import pyplot as plt
 except ImportError:
     plt = None
 
 from .supersmoother import SuperSmoother
 from .smoother import perform_smooth
 
-
 MAX_OUTERS = 200
 
-
-class ACESolver(object):  # pylint: disable=too-many-instance-attributes
-    """The Alternating Conditional Expectation algorithm to perform regressions."""
+class ACESolver(object):
+    '''
+    Runs the Alternating Conditional Expectation algorithm to perform regressions
+    '''
 
     def __init__(self):
-        """Solver constructor."""
         self._last_inner_error = float('inf')
         self._last_outer_error = float('inf')
         self.x = []
         self.y = None
         self._xi_sorted = None
         self._yi_sorted = None
         self.x_transforms = None
         self.y_transform = None
         self._smoother_cls = SuperSmoother
         self._outer_iters = 0
         self._inner_iters = 0
+        self._N = None
 
     def specify_data_set(self, x_input, y_input):
         """
-        Define input to ACE.
+        Define input to ACE
 
         Parameters
         ----------
         x_input : list
             list of iterables, one for each independent variable
         y_input : array
             the dependent observations
-
         """
         self.x = x_input
         self.y = y_input
 
     def solve(self):
-        """Run the ACE calculational loop."""
+        """
+        Run the ACE calculational loop
+        """
         self._initialize()
         while self._outer_error_is_decreasing() and self._outer_iters < MAX_OUTERS:
             print('* Starting outer iteration {0:03d}. Current err = {1:12.5E}'
                   ''.format(self._outer_iters, self._last_outer_error))
             self._iterate_to_update_x_transforms()
             self._update_y_transform()
             self._outer_iters += 1
 
     def _initialize(self):
-        """Set up and normalize initial data once input data is specified."""
+        """
+        Set up and normalize initial data once input data is specified
+        """
+        self._N = len(self.y)
         self.y_transform = self.y - numpy.mean(self.y)
         self.y_transform /= numpy.std(self.y_transform)
-        self.x_transforms = [numpy.zeros(len(self.y)) for _xi in self.x]
+        self.x_transforms = [numpy.zeros(self._N) for xi in self.x]
         self._compute_sorted_indices()
 
     def _compute_sorted_indices(self):
         """
-        Sort data from the perspective of each column.
+        The smoothers need sorted data. This sorts it from the perspective of each column.
 
         if self._x[0][3] is the 9th-smallest value in self._x[0], then  _xi_sorted[3] = 8
 
         We only have to sort the data once.
         """
         sorted_indices = []
         for to_sort in [self.y] + self.x:
@@ -93,53 +97,66 @@
             data_w_indices.sort()
             sorted_indices.append([i for val, i in data_w_indices])
         # save in meaningful variable names
         self._yi_sorted = sorted_indices[0]  # list (like self.y)
         self._xi_sorted = sorted_indices[1:]  # list of lists (like self.x)
 
     def _outer_error_is_decreasing(self):
-        """Return True if outer iteration error is decreasing."""
+        """
+        True if outer iteration error is decreasing
+        """
         is_decreasing, self._last_outer_error = self._error_is_decreasing(self._last_outer_error)
         return is_decreasing
 
     def _error_is_decreasing(self, last_error):
-        """Return True if current error is less than last_error."""
+        """
+        True if current error is less than last_error
+        """
         current_error = self._compute_error()
-        is_decreasing = current_error < last_error
+        if current_error < last_error:
+            is_decreasing = True
+        else:
+            is_decreasing = False
         return is_decreasing, current_error
 
     def _compute_error(self):
-        """Compute unexplained error."""
+        """
+        Computes unexplained error
+        """
         sum_x = sum(self.x_transforms)
         err = sum((self.y_transform - sum_x) ** 2) / len(sum_x)
         return err
 
     def _iterate_to_update_x_transforms(self):
-        """Perform the inner iteration."""
+        """
+        Perform the inner iteration
+        """
         self._inner_iters = 0
         self._last_inner_error = float('inf')
         while self._inner_error_is_decreasing():
             print('  Starting inner iteration {0:03d}. Current err = {1:12.5E}'
                   ''.format(self._inner_iters, self._last_inner_error))
             self._update_x_transforms()
             self._inner_iters += 1
 
     def _inner_error_is_decreasing(self):
         is_decreasing, self._last_inner_error = self._error_is_decreasing(self._last_inner_error)
         return is_decreasing
 
     def _update_x_transforms(self):
         """
-        Compute a new set of x-transform functions phik.
+        Compute a new set of x-transform functions phik
 
         phik(xk) = theta(y) - sum of phii(xi) over i!=k
 
         This is the first of the eponymous conditional expectations. The conditional
         expectations are computed using the SuperSmoother.
+
         """
+
         # start by subtracting all transforms
         theta_minus_phis = self.y_transform - numpy.sum(self.x_transforms, axis=0)
 
         # add one transform at a time so as to exclude it from the subtracted sum
         for xtransform_index in range(len(self.x_transforms)):
             xtransform = self.x_transforms[xtransform_index]
             sorted_data_indices = self._xi_sorted[xtransform_index]
@@ -186,75 +203,86 @@
         sum_of_x_transformations_smooth -= numpy.mean(sum_of_x_transformations_smooth)
         sum_of_x_transformations_smooth /= numpy.std(sum_of_x_transformations_smooth)
 
         # unsort to save in the original data
         self.y_transform = unsort_vector(sum_of_x_transformations_smooth, sorted_data_indices)
 
     def write_input_to_file(self, fname='ace_input.txt'):
-        """Write y and x values used in this run to a space-delimited txt file."""
+        """
+        Write y and x values used in this run to a space-delimited txt file
+        """
         self._write_columns(fname, self.x, self.y)
 
     def write_transforms_to_file(self, fname='ace_transforms.txt'):
-        """Write y and x transforms used in this run to a space-delimited txt file."""
+        """
+        Write y and x transforms used in this run to a space-delimited txt file
+        """
         self._write_columns(fname, self.x_transforms, self.y_transform)
 
-    def _write_columns(self, fname, xvals, yvals):  # pylint: disable=no-self-use
-        with open(fname, 'w') as output_file:
-            alldata = [yvals] + xvals
-            for datai in zip(*alldata):
-                yline = '{0: 15.9E} '.format(datai[0])
-                xline = ' '.join(['{0: 15.9E}'.format(xii) for xii in datai[1:]])
-                output_file.write(''.join([yline, xline, '\n']))
-
+    def _write_columns(self, fname, xvals, yvals):
+        f = open(fname, 'w')
+        alldata = [yvals] + xvals
+        for datai in zip(*alldata):
+            yline = '{0: 15.9E} '.format(datai[0])
+            xline = ' '.join(['{0: 15.9E}'.format(xii) for xii in datai[1:]])
+            f.write(''.join([yline, xline, '\n']))
+        f.close()
 
 def sort_vector(data, indices_of_increasing):
-    """Permutate 1-d data using given indices."""
+    """
+    permutate 1-d data using given indices
+    """
     return numpy.array([data[i] for i in indices_of_increasing])
 
-
 def unsort_vector(data, indices_of_increasing):
-    """Upermutate 1-D data that is sorted by indices_of_increasing."""
+    """
+    unpermutate 1-D data that is sorted by indices_of_increasing
+    """
     return numpy.array([data[indices_of_increasing.index(i)] for i in range(len(data))])
 
-
 def plot_transforms(ace_model, fname='ace_transforms.png'):
-    """Plot the transforms."""
+    """
+    Plot the transforms
+    """
     if not plt:
         raise ImportError('Cannot plot without the matplotlib package')
     plt.rcParams.update({'font.size': 8})
     plt.figure()
-    num_cols = len(ace_model.x) // 2 + 1
+    numCols = len(ace_model.x) / 2 + 1
     for i in range(len(ace_model.x)):
-        plt.subplot(num_cols, 2, i + 1)
+        plt.subplot(numCols, 2, i + 1)
         plt.plot(ace_model.x[i], ace_model.x_transforms[i], '.', label='Phi {0}'.format(i))
         plt.xlabel('x{0}'.format(i))
         plt.ylabel('phi{0}'.format(i))
-    plt.subplot(num_cols, 2, i + 2)  # pylint: disable=undefined-loop-variable
+    plt.subplot(numCols, 2, i + 2)
     plt.plot(ace_model.y, ace_model.y_transform, '.', label='Theta')
     plt.xlabel('y')
     plt.ylabel('theta')
     plt.tight_layout()
 
     if fname:
         plt.savefig(fname)
-        return None
-    return plt
+    else:
+        plt.show()
 
 def plot_input(ace_model, fname='ace_input.png'):
-    """Plot the transforms."""
+    """
+    Plot the transforms
+    """
     if not plt:
         raise ImportError('Cannot plot without the matplotlib package')
     plt.rcParams.update({'font.size': 8})
     plt.figure()
-    num_cols = len(ace_model.x) // 2 + 1
+    numCols = len(ace_model.x) / 2 + 1
     for i in range(len(ace_model.x)):
-        plt.subplot(num_cols, 2, i + 1)
+        plt.subplot(numCols, 2, i + 1)
         plt.plot(ace_model.x[i], ace_model.y, '.')
         plt.xlabel('x{0}'.format(i))
-        plt.ylabel('y')
+        plt.ylabel('y'.format(i))
 
     plt.tight_layout()
 
     if fname:
         plt.savefig(fname)
     else:
         plt.show()
+
```

### Comparing `ace-0.3.3/ace/model.py` & `ace-0.3.post1/ace/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,111 @@
-"""
-The Model module is a front-end to the :py:mod:`ace.ace` module.
-
-ACE itself just gives transformations back as discontinuous data points.
-This module loads data, runs ACE, and then performs interpolations on the results,
+'''
+The Model module is a front-end to the :py:mod:`ace.ace` module. ACE itself
+just gives transformations back as discontinuous data points. This module
+loads data, runs ACE, and then performs interpolations on the results,
 giving the user continuous functions that may be evaluated at any point
 within the range trained.
 
 This is a convenience/frontend/demo module. If you want to control ACE yourself,
 you may want to just use the ace module manually.
-
-"""
+'''
 
 from scipy.interpolate import interp1d
 
 from . import ace
 
-
 def read_column_data_from_txt(fname):
     """
-    Read data from a simple text file.
+    reads data from a simple text file.
 
     Format should be just numbers.
     First column is the dependent variable. others are independent.
-    Whitespace delimited.
+    Whitespace deliminted.
 
     Returns
     -------
     x_values : list
         List of x columns
     y_values : list
         list of y values
-
     """
     datafile = open(fname)
     datarows = []
     for line in datafile:
         datarows.append([float(li) for li in line.split()])
-    datacols = list(zip(*datarows))
+    datacols = list(zip(*datarows))  # pylint: disable=star-args
     x_values = datacols[1:]
     y_values = datacols[0]
 
     return x_values, y_values
 
-
 class Model(object):
-    """A continuous model of data based on ACE regressions."""
-
+    """
+    A continuous model of data based on ACE regressions
+    """
     def __init__(self):
-        """Model constructor."""
         self.ace = ace.ACESolver()
         self.phi_continuous = None
         self.inverse_theta_continuous = None
 
     def build_model_from_txt(self, fname):
         """
         Construct the model and perform regressions based on data in a txt file.
 
         Parameters
         ----------
         fname : str
             The name of the file to load.
-
         """
         x_values, y_values = read_column_data_from_txt(fname)
         self.build_model_from_xy(x_values, y_values)
 
     def build_model_from_xy(self, x_values, y_values):
-        """Construct the model and perform regressions based on x, y data."""
+        """
+        Construct the model and perform regressions based on x, y data.
+        """
         self.init_ace(x_values, y_values)
         self.run_ace()
         self.build_interpolators()
 
     def init_ace(self, x_values, y_values):
-        """Specify data for the ACE solver object."""
+        """
+        Specify data for the ACE solver object
+        """
         self.ace.specify_data_set(x_values, y_values)
 
     def run_ace(self):
-        """Perform the ACE calculation."""
+        """
+        Perform the ACE calculation
+        """
         self.ace.solve()
 
     def build_interpolators(self):
-        """Compute 1-D interpolation functions for all the transforms so they're continuous.."""
+        """
+        Compute 1-D interpolation functions for all the transforms so they're continuous.
+        """
         self.phi_continuous = []
         for xi, phii in zip(self.ace.x, self.ace.x_transforms):
-            self.phi_continuous.append(
-                interp1d(
-                    x=xi,
-                    y=phii,
-                    bounds_error=False,
-                    fill_value=(min(phii), max(phii))))
-        self.inverse_theta_continuous = interp1d(
-            x=self.ace.y_transform,
-            y=self.ace.y,
-            bounds_error=False,
-            fill_value=(min(self.ace.y), max(self.ace.y)))
+            self.phi_continuous.append(interp1d(xi, phii))
+        self.inverse_theta_continuous = interp1d(self.ace.y_transform, self.ace.y)
 
     def eval(self, x_values):
         """
-        Evaluate the ACE regression at any combination of independent variable values.
+        evaluate the ACE regression at any combination of independent variable values
 
         Parameters
         ----------
         x_values : iterable
             a float x-value for each independent variable, e.g. (1.5, 2.5)
-
         """
         if len(x_values) != len(self.phi_continuous):
-            raise ValueError(
-                'x_values must have length equal to the number of independent variables '
-                '({0}) rather than {1}.'.format(
-                    len(self.phi_continuous), len(x_values)))
-
-        sum_phi = sum(
-            [phi(xi) for phi, xi in zip(self.phi_continuous, x_values)])
-        return self.inverse_theta_continuous(sum_phi)
+            raise ValueError('x_values must have length equal to the number of independent variables '
+                             '({0}) rather than {1}.'.format(len(self.phi_continuous),
+                                                             len(x_values)))
+
+        sum_phi = sum([phi(xi) for phi, xi in zip(self.phi_continuous, x_values)])
+        return float(self.inverse_theta_continuous(sum_phi))
+
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `ace-0.3.3/ace/samples/smoother_friedman82.py` & `ace-0.3.post1/ace/samples/smoother_friedman82.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-"""Problem demonstrating supersmoother from [Friedman82]_."""
+'''
+Problem demonstrating supersmoother from [Friedman82]_
+'''
 
 import math
 
+import numpy
 import numpy.random
 import matplotlib.pyplot as plt
 
 from ace import smoother
 
-
 def build_sample_smoother_problem_friedman82(N=200):
-    """Sample problem from supersmoother publication."""
+    """
+    Sample problem from supersmoother pub.
+    """
     x = numpy.random.uniform(size=N)
     err = numpy.random.standard_normal(N)
     y = numpy.sin(2 * math.pi * (1 - x) ** 2) + x * err
     return x, y
 
 def run_friedman82_basic():
-    """Run Friedman's test of fixed-span smoothers from Figure 2b."""
+    """
+    Runs Friedman's test of fixed-span smoothers from Figure 2b.
+    """
     x, y = build_sample_smoother_problem_friedman82()
     plt.figure()
     # plt.plot(x, y, '.', label='Data')
     for span in smoother.DEFAULT_SPANS:
         smooth = smoother.BasicFixedSpanSmoother()
         smooth.specify_data_set(x, y, sort_data=True)
         smooth.set_span(span)
```

### Comparing `ace-0.3.3/ace/samples/supersmoother_friedman82.py` & `ace-0.3.post1/ace/samples/supersmoother_friedman82.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-"""Problem demonstrating supersmoother from [Friedman82]_."""
+'''
+Problem demonstrating supersmoother from [Friedman82]_
+'''
 
 import matplotlib.pyplot as plt
 
-from ace.samples import smoother_friedman82
-from ace.supersmoother import SuperSmoother
+import smoother_friedman82
+from ..supersmoother import SuperSmoother
 
 def run_friedman82_super():
-    """Run Friedman's test of fixed-span smoothers from Figure 2b."""
+    """
+    Runs Friedman's test of fixed-span smoothers from Figure 2b.
+    """
     x, y = smoother_friedman82.build_sample_smoother_problem_friedman82()
     plt.figure()
     smooth = SuperSmoother()
     smooth.specify_data_set(x, y, sort_data=True)
     smooth.compute()
     plt.plot(x, y, '.', label='Data')
     plt.plot(smooth.x, smooth.smooth_result, 'o', label='Smooth')
```

### Comparing `ace-0.3.3/ace/smoother.py` & `ace-0.3.post1/ace/smoother.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-"""
-Scatterplot smoother with a fixed span.
-
-Takes x,y scattered data and returns a set of
+'''
+Scatterplot smoother with a fixed span. Takes x,y scattered data and returns a set of
 (x,s) points that form a smoother curve fitting the data with moving least squares estimates.
 Similar to a moving average, but with better characteristics. The fundamental issue
 with this smoother is that the choice of span (window size) is not known in advance.
 The SuperSmoother uses these smoothers to figure out which span is optimal.
 
 This is a Python port of J. Friedman's 1982 fixed-span Smoother [Friedman82]_
 
@@ -13,30 +11,32 @@
 
     s = Smoother()
     s.specify_data_set(x, y, sort_data = True)
     s.set_span(0.05)
     s.compute()
     smoothed_y = s.smooth_result
 
-"""
+
+'''
 
 import numpy
-import matplotlib.pyplot as plt
+import pylab
 
 TWEETER_SPAN = 0.05
 MID_SPAN = 0.2
 BASS_SPAN = 0.5
 
 DEFAULT_SPANS = (TWEETER_SPAN, MID_SPAN, BASS_SPAN)
 
-class Smoother(object):  # pylint: disable=too-many-instance-attributes
-    """Smoother that accepts data and produces smoother curves that fit the data."""
+class Smoother(object):
+    '''
+    Smoothers accept data and produce smoother curves that fit the data.
+    '''
 
     def __init__(self):
-        """Smoother constructor."""
         self.x = []
         self.y = []
 
         self._mean_x_in_window = 0.0
         self._mean_y_in_window = 0.0
         self._covariance_in_window = 0.0
         self._variance_in_window = 0.0
@@ -48,15 +48,17 @@
         self._original_index_of_xvalue = []  # for dealing w/ unsorted data
         self._window_bound_lower = 0
         self._x_in_window = []
         self._y_in_window = []
         self._neighbors_on_each_side = None
 
     def add_data_point_xy(self, x, y):
-        """Add a new data point to the data set to be smoothed."""
+        """
+        add a new data point to the data set to be smoothed
+        """
         self.x.append(x)
         self.y.append(y)
 
     def specify_data_set(self, x_input, y_input, sort_data=False):
         """
         Fully define data by lists of x values and y values.
 
@@ -66,68 +68,71 @@
         ----------
         x_input : iterable
             list of floats that represent x
         y_input : iterable
             list of floats that represent y(x) for each x
         sort_data : bool, optional
             If true, the data will be sorted by increasing x values.
-
         """
         if sort_data:
             xy = sorted(zip(x_input, y_input))
-            x, y = zip(*xy)
+            x, y = zip(*xy)  # pylint: disable=star-args
             x_input_list = list(x_input)
             self._original_index_of_xvalue = [x_input_list.index(xi) for xi in x]
             if len(set(self._original_index_of_xvalue)) != len(x):
                 raise RuntimeError('There are some non-unique x-values')
         else:
             x, y = x_input, y_input
 
         self.x = x
         self.y = y
 
     def set_span(self, span):
         """
-        Set the window-size for computing the least squares fit.
+        Set the window-size for computing the least squares fit
 
         Parameters
         ----------
         span : float
             Fraction on data length N to be considered in smoothing
-
         """
         self._span = span
 
     def compute(self):
-        """Perform the smoothing operations."""
+        """
+        Perform the smoothing operations
+        """
         raise NotImplementedError
 
     def plot(self, fname=None):
         """
-        Plot the input data and resulting smooth.
+        Plot the input data and resulting smooth
 
         Parameters
         ----------
         fname : str, optional
             name of file to produce. If none, will show interactively.
-
         """
-        plt.figure()
-        xy = sorted(zip(self.x, self.smooth_result))
-        x, y = zip(*xy)
-        plt.plot(x, y, '-')
-        plt.plot(self.x, self.y, '.')
+        pylab.figure()
+        xy = zip(self.x, self.smooth_result)
+        xy.sort()
+        x, y = zip(*xy)  # pylint: disable=star-args
+        pylab.plot(x, y, '-')
+        pylab.plot(self.x, self.y, '.')
         if fname:
-            plt.savefig(fname)
+            pylab.savefig(fname)
         else:
-            plt.show()
-        plt.close()
+            pylab.show()
+        pylab.close()
 
     def _store_unsorted_results(self, smooth, residual):
-        """Convert sorted smooth/residual back to as-input order."""
+        """
+        Convert sorted smooth/residual back to as-input order
+        """
+
         if self._original_index_of_xvalue:
             # data was sorted. Unsort it here.
             self.smooth_result = numpy.zeros(len(self.y))
             self.cross_validated_residual = numpy.zeros(len(residual))
             original_x = numpy.zeros(len(self.y))
             for i, (xval, smooth_val, residual_val) in enumerate(zip(self.x, smooth, residual)):
                 original_index = self._original_index_of_xvalue[i]
@@ -138,162 +143,177 @@
         else:
             # no sorting was done. just apply results
             self.smooth_result = smooth
             self.cross_validated_residual = residual
 
 
 
-class BasicFixedSpanSmoother(Smoother):  # pylint: disable=too-many-instance-attributes
+class BasicFixedSpanSmoother(Smoother):
     """
-    A basic fixed-span smoother.
+    A basic fixed-span smoother
 
     Simple least-squares linear local smoother.
 
     Uses fast updates of means, variances.
     """
 
     def compute(self):
-        """Perform the smoothing operations."""
+        """
+        Perform the smoothing operations
+        """
         self._compute_window_size()
         smooth = []
         residual = []
 
         x, y = self.x, self.y
 
         # step through x and y data with a window window_size wide.
         self._update_values_in_window()
         self._update_mean_in_window()
         self._update_variance_in_window()
         for i, (xi, yi) in enumerate(zip(x, y)):
             if ((i - self._neighbors_on_each_side) > 0.0 and
-                    (i + self._neighbors_on_each_side) < len(x)):
+                (i + self._neighbors_on_each_side) < len(x)):
                 self._advance_window()
             smooth_here = self._compute_smooth_during_construction(xi)
             residual_here = self._compute_cross_validated_residual_here(xi, yi, smooth_here)
             smooth.append(smooth_here)
             residual.append(residual_here)
 
         self._store_unsorted_results(smooth, residual)
 
     def _compute_window_size(self):
-        """Determine characteristics of symmetric neighborhood with J/2 values on each side."""
+        """
+        Determine characteristics of symmetric neighborhood with J/2 values on each side
+        """
         self._neighbors_on_each_side = int(len(self.x) * self._span) // 2
         self.window_size = self._neighbors_on_each_side * 2 + 1
         if self.window_size <= 1:
             # cannot do averaging with 1 point in window. Force >=2
             self.window_size = 2
 
     def _update_values_in_window(self):
-        """Update which values are in the current window."""
+        """
+        update which values are in the current window
+        """
         window_bound_upper = self._window_bound_lower + self.window_size
         self._x_in_window = self.x[self._window_bound_lower:window_bound_upper]
         self._y_in_window = self.y[self._window_bound_lower:window_bound_upper]
 
     def _update_mean_in_window(self):
         """
-        Compute mean in window the slow way. useful for first step.
+        Compute mean in window the slow way. useful for first step
 
         Considers all values in window
 
         See Also
         --------
         _add_observation_to_means : fast update of mean for single observation addition
         _remove_observation_from_means : fast update of mean for single observation removal
 
         """
         self._mean_x_in_window = numpy.mean(self._x_in_window)
         self._mean_y_in_window = numpy.mean(self._y_in_window)
 
     def _update_variance_in_window(self):
         """
-        Compute variance and covariance in window using all values in window (slow).
+        compute variance and covariance in window using all values in window (slow)
 
         See Also
         --------
         _add_observation_to_variances : fast update for single observation addition
         _remove_observation_from_variances : fast update for single observation removal
-
         """
         self._covariance_in_window = sum([(xj - self._mean_x_in_window) *
                                           (yj - self._mean_y_in_window)
                                           for xj, yj in zip(self._x_in_window, self._y_in_window)])
 
         self._variance_in_window = sum([(xj - self._mean_x_in_window) ** 2 for xj
                                         in self._x_in_window])
 
     def _advance_window(self):
-        """Update values in current window and the current window means and variances."""
+        """
+        Update values in current window and the current window means and variances.
+        """
         x_to_remove, y_to_remove = self._x_in_window[0], self._y_in_window[0]
 
         self._window_bound_lower += 1
         self._update_values_in_window()
         x_to_add, y_to_add = self._x_in_window[-1], self._y_in_window[-1]
 
         self._remove_observation(x_to_remove, y_to_remove)
         self._add_observation(x_to_add, y_to_add)
 
     def _remove_observation(self, x_to_remove, y_to_remove):
-        """Remove observation from window, updating means/variance efficiently."""
+        """
+        Removes observation from window, updating means/variance efficiently
+        """
         self._remove_observation_from_variances(x_to_remove, y_to_remove)
         self._remove_observation_from_means(x_to_remove, y_to_remove)
         self.window_size -= 1
 
     def _add_observation(self, x_to_add, y_to_add):
-        """Add observation to window, updating means/variance efficiently."""
+        """
+        Adds observation to window, updating means/variance efficiently
+        """
         self._add_observation_to_means(x_to_add, y_to_add)
         self._add_observation_to_variances(x_to_add, y_to_add)
         self.window_size += 1
 
     def _add_observation_to_means(self, xj, yj):
-        """Update the means without recalculating for the addition of one observation."""
+        """
+        Update the means without recalculating for the addition of one observation
+        """
         self._mean_x_in_window = ((self.window_size * self._mean_x_in_window + xj) /
                                   (self.window_size + 1.0))
         self._mean_y_in_window = ((self.window_size * self._mean_y_in_window + yj) /
                                   (self.window_size + 1.0))
 
     def _remove_observation_from_means(self, xj, yj):
-        """Update the means without recalculating for the deletion of one observation."""
+        """
+        Update the means without recalculating for the deletion of one observation
+        """
         self._mean_x_in_window = ((self.window_size * self._mean_x_in_window - xj) /
                                   (self.window_size - 1.0))
         self._mean_y_in_window = ((self.window_size * self._mean_y_in_window - yj) /
                                   (self.window_size - 1.0))
 
     def _add_observation_to_variances(self, xj, yj):
         """
-        Quickly update the variance and co-variance for the addition of one observation.
+        Quickly update the variance and co-variance for the addition of one observation
 
         See Also
         --------
         _update_variance_in_window : compute variance considering full window
-
         """
         term1 = (self.window_size + 1.0) / self.window_size * (xj - self._mean_x_in_window)
         self._covariance_in_window += term1 * (yj - self._mean_y_in_window)
         self._variance_in_window += term1 * (xj - self._mean_x_in_window)
 
     def _remove_observation_from_variances(self, xj, yj):
-        """Quickly update the variance and co-variance for the deletion of one observation."""
+        """
+        Quickly update the variance and co-variance for the deletion of one observation
+        """
         term1 = self.window_size / (self.window_size - 1.0) * (xj - self._mean_x_in_window)
         self._covariance_in_window -= term1 * (yj - self._mean_y_in_window)
         self._variance_in_window -= term1 * (xj - self._mean_x_in_window)
 
     def _compute_smooth_during_construction(self, xi):
         """
-        Evaluate value of smooth at x-value xi.
+        Evaluate value of smooth at x-value xi
 
         Parameters
         ----------
         xi : float
             Value of x where smooth value is desired
 
         Returns
         -------
         smooth_here : float
             Value of smooth s(xi)
-
         """
         if self._variance_in_window:
             beta = self._covariance_in_window / self._variance_in_window
             alpha = self._mean_y_in_window - beta * self._mean_x_in_window
             value_of_smooth_here = beta * (xi) + alpha
         else:
             value_of_smooth_here = 0.0
@@ -301,38 +321,36 @@
 
     def _compute_cross_validated_residual_here(self, xi, yi, smooth_here):
         """
         Compute cross validated residual.
 
         This is the absolute residual from Eq. 9. in [1]
         """
-        denom = (1.0 - 1.0 / self.window_size -
-                 (xi - self._mean_x_in_window) ** 2 /
-                 self._variance_in_window)
-        if denom == 0.0:
-            # can happen  with small data sets
-            return 1.0
-        return abs((yi - smooth_here) / denom)
+        residual = abs((yi - smooth_here) / (1.0 - 1.0 / self.window_size -
+                                             (xi - self._mean_x_in_window) ** 2 /
+                                             self._variance_in_window))
+        return residual
 
 class BasicFixedSpanSmootherSlowUpdate(BasicFixedSpanSmoother):
-    """Use slow means and variances at each step. Used to validate fast updates."""
+    """
+    Uses slow means and variances at each step. Used to validate fast updates
+    """
 
     def _advance_window(self):
         self._window_bound_lower += 1
         self._update_values_in_window()
         self._update_mean_in_window()
         self._update_variance_in_window()
 
 
-DEFAULT_BASIC_SMOOTHER = BasicFixedSpanSmoother  # pylint: disable=invalid-name
-
+DEFAULT_BASIC_SMOOTHER = BasicFixedSpanSmoother
 
 def perform_smooth(x_values, y_values, span=None, smoother_cls=None):
     """
-    Run the basic smoother (convenience function).
+    Convenience function to run the basic smoother
 
     Parameters
     ----------
     x_values : iterable
         List of x value observations
     y_ values : iterable
         list of y value observations
@@ -341,20 +359,18 @@
     smoother_cls : Class
         The class of smoother to use to smooth the data
 
     Returns
     -------
     smoother : object
         The smoother object with results stored on it.
-
     """
     if smoother_cls is None:
         smoother_cls = DEFAULT_BASIC_SMOOTHER
     smoother = smoother_cls()
     smoother.specify_data_set(x_values, y_values)
     smoother.set_span(span)
     smoother.compute()
     return smoother
 
-
 if __name__ == '__main__':
     pass
```

### Comparing `ace-0.3.3/ace/supersmoother.py` & `ace-0.3.post1/ace/supersmoother.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-"""
-A variable-span data smoother.
-
-This uses the fixed-span smoother to determine
+'''
+A variable-span data smoother. This uses the fixed-span smoother to determine
 a changing optimal span for the data based on cross-validated residuals. It
 is an adaptive smoother that requires several passes over the data.
 
 The SuperSmoother provides a mechanism to evaluate the conditional expectations
 in the ACE algorithm.
 
 Based on [Friedman82]_.
 
 Example::
 
     s = SuperSmoother()
     s.specify_data_set(x, y, sort_data = True)
     s.compute()
     smoothed_y = s.smooth_result
-"""
 
+'''
 import numpy
 from matplotlib import pyplot as plt
 
 from . import smoother
 from .smoother import DEFAULT_SPANS, MID_SPAN, BASS_SPAN, TWEETER_SPAN
 
-
 BASS_INDEX = DEFAULT_SPANS.index(BASS_SPAN)
 
-
 class SuperSmoother(smoother.Smoother):
-    """Variable-span smoother."""
+    '''
+    Variable-span smoother
+    '''
 
     def __init__(self):
-        """Construct a SuperSmoother."""
         super(SuperSmoother, self).__init__()
 
         self._primary_smooths = []
         self._residual_smooths = []
         self._best_span_at_each_point = []
-        self._smoothed_best_spans = None
+        self._smoothed_best_spans = []
         self._bass_enhancement = 0.0  # should be between 0 and 10.
 
     def set_bass_enhancement(self, alpha):
         """
-        Bass enhancement amplifies the bass span.
+        Bass enhancement amplifies the bass span
 
         This gives the resulting smooth a smoother look, which is sometimes desirable if
         the underlying mechanisms are known to be smooth.
         """
         self._bass_enhancement = alpha
 
     def compute(self):
-        """Run the SuperSmoother."""
+
         self._compute_primary_smooths()
         self._smooth_the_residuals()
         self._select_best_smooth_at_each_point()
         self._enhance_bass()
         self._smooth_best_span_estimates()
         self._apply_best_spans_to_primaries()
         self._smooth_interpolated_smooth()
         self._store_unsorted_results(self.smooth_result, numpy.zeros(len(self.smooth_result)))
 
     def _compute_primary_smooths(self):
-        """Compute fixed-span smooths with all of the default spans."""
+        """
+        Compute fixed-span smooths with all of the default spans.
+        """
         for span in DEFAULT_SPANS:
             smooth = smoother.perform_smooth(self.x, self.y, span)
             self._primary_smooths.append(smooth)
 
     def _smooth_the_residuals(self):
         """
         Apply the MID_SPAN to the residuals of the primary smooths.
@@ -78,79 +77,81 @@
             smooth = smoother.perform_smooth(self.x,
                                              primary_smooth.cross_validated_residual,
                                              MID_SPAN)
             self._residual_smooths.append(smooth.smooth_result)
 
     def _select_best_smooth_at_each_point(self):
         """
-        Solve Eq (10) to find the best span for each observation.
+        Solve Eq (10) to find the best span for each observation
 
         Stores index so we can easily grab the best residual smooth, primary smooth, etc.
         """
         for residuals_i in zip(*self._residual_smooths):
             index_of_best_span = residuals_i.index(min(residuals_i))
             self._best_span_at_each_point.append(DEFAULT_SPANS[index_of_best_span])
 
     def _enhance_bass(self):
-        """Update best span choices with bass enhancement as requested by user (Eq. 11)."""
+        """
+        Update best span choices with bass enhancement as requested by user
+        (Eq. 11)
+        """
         if not self._bass_enhancement:
             # like in supsmu, skip if alpha=0
             return
         bass_span = DEFAULT_SPANS[BASS_INDEX]
         enhanced_spans = []
         for i, best_span_here in enumerate(self._best_span_at_each_point):
             best_smooth_index = DEFAULT_SPANS.index(best_span_here)
             best_span = DEFAULT_SPANS[best_smooth_index]
             best_span_residual = self._residual_smooths[best_smooth_index][i]
             bass_span_residual = self._residual_smooths[BASS_INDEX][i]
-            if 0 < best_span_residual < bass_span_residual:
+            if best_span_residual < bass_span_residual and best_span_residual > 0:
                 ri = best_span_residual / bass_span_residual
                 bass_factor = ri ** (10.0 - self._bass_enhancement)
                 enhanced_spans.append(best_span + (bass_span - best_span) * bass_factor)
             else:
                 enhanced_spans.append(best_span)
         self._best_span_at_each_point = enhanced_spans
 
     def _smooth_best_span_estimates(self):
-        """Apply a MID_SPAN smooth to the best span estimates at each observation."""
+        """
+        Apply a MID_SPAN smooth to the best span estimates at each observation
+        """
         self._smoothed_best_spans = smoother.perform_smooth(self.x,
                                                             self._best_span_at_each_point,
                                                             MID_SPAN)
 
     def _apply_best_spans_to_primaries(self):
         """
-        Apply best spans.
-
-        Given the best span, interpolate to compute the best smoothed value
-        at each observation.
+        Given the best span, interpolate to compute the best smoothed value at each observation
         """
         self.smooth_result = []
         for xi, best_span in enumerate(self._smoothed_best_spans.smooth_result):
             primary_values = [s.smooth_result[xi] for s in self._primary_smooths]
-            # pylint: disable=no-member
             best_value = numpy.interp(best_span, DEFAULT_SPANS, primary_values)
             self.smooth_result.append(best_value)
 
     def _smooth_interpolated_smooth(self):
         """
-        Smooth interpolated results with tweeter span.
+        Smooth interpolated results with tweeter span
 
         A final step of the supersmoother is to smooth the interpolated values with
         the tweeter span. This is done in Breiman's supsmu.f but is not explicitly
         discussed in the publication. This step is necessary to match
         the FORTRAN version perfectly.
         """
         smoothed_results = smoother.perform_smooth(self.x,
                                                    self.smooth_result,
                                                    TWEETER_SPAN)
         self.smooth_result = smoothed_results.smooth_result
 
 class SuperSmootherWithPlots(SuperSmoother):
-    """Auxiliary subclass for researching/understanding the SuperSmoother."""
-
+    """
+    Auxiliary subclass for researching/understanding the SuperSmoother
+    """
     def _compute_primary_smooths(self):
         super(SuperSmootherWithPlots, self)._compute_primary_smooths()
         plt.figure()
         for smooth in self._primary_smooths:
             plt.plot(self.x, smooth.smooth_result)
         plt.plot(self.x, self.y, '.')
         plt.savefig('primary_smooths.png')
```

### Comparing `ace-0.3.3/ace/tests/test_ace.py` & `ace-0.3.post1/ace/tests/test_ace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-"""
+'''
 Unit tests for ACE methods.
 
 These implicitly cover the SuperSmoother as well, but they don't validate it.
-"""
+'''
 
 import unittest
 
 import ace.ace
 import ace.samples.breiman85
 
-# pylint: disable=protected-access, missing-docstring
-
 class TestAce(unittest.TestCase):
-    """Tests."""
 
     def setUp(self):
         self.ace = ace.ace.ACESolver()
         x, y = ace.samples.breiman85.build_sample_ace_problem_breiman85()
         self.ace.specify_data_set(x, y)
         self.ace._initialize()
```

### Comparing `ace-0.3.3/ace/tests/test_model.py` & `ace-0.3.post1/ace/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Unit tests for ace model."""
-
+'''
+Unit tests for ace model.
+'''
 import unittest
 import os
 
-from ace import model
-from ace.samples import breiman85
-from ace.samples import wang04
-
-# pylint: disable=protected-access, missing-docstring
+from .. import model
+from ..samples import breiman85
+from ..samples import wang04
 
 class TestModel(unittest.TestCase):
 
+
     def setUp(self):
         self.model = model.Model()
 
     def tearDown(self):
         pass
 
     def test_build_model_from_xy(self):
```

### Comparing `ace-0.3.3/ace/tests/test_smoother.py` & `ace-0.3.post1/ace/tests/test_smoother.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,84 @@
-"""Smoother unit tests"""
+'''
+Smoother unit tests
 
+'''
 import unittest
 
-from ace import smoother
-
-# pylint: disable=protected-access, missing-docstring
+from .. import smoother
 
 class TestSmoother(unittest.TestCase):
     def setUp(self):
         self.smoother = smoother.BasicFixedSpanSmoother()
-        self.x_data = [1.0, 2.0, 3.0, 4.0]
-        self.y_data = [4.0, 5.0, 6.0, 7.0]
-        self.smoother.specify_data_set(self.x_data, self.y_data)
+
+        self.xData = [1.0, 2.0, 3.0, 4.0]
+        self.yData = [4.0, 5.0, 6.0, 7.0]
+        self.smoother.specify_data_set(self.xData, self.yData)
         self.smoother.window_size = 3
         self.smoother._update_values_in_window()
         self.smoother._update_mean_in_window()
         self.smoother._update_variance_in_window()
 
 
     def test_mean(self):
-        size = self.smoother.window_size
+        ws = self.smoother.window_size
         self.assertAlmostEqual(self.smoother._mean_x_in_window,
-                               sum(self.x_data[:size]) / len(self.x_data[:size]))
+                               sum(self.xData[:ws]) / len(self.xData[:ws]))
 
         self.assertAlmostEqual(self.smoother._mean_y_in_window,
-                               sum(self.y_data[:size]) / len(self.y_data[:size]))
+                               sum(self.yData[:ws]) / len(self.yData[:ws]))
 
     def test_mean_on_addition_of_observation(self):
-        """Make sure things work when we add an observation."""
+        """
+        Make sure things work when we add an observation
+        """
         self.smoother._add_observation_to_means(7, 8)
-        size = self.smoother.window_size
+        ws = self.smoother.window_size
         self.assertAlmostEqual(self.smoother._mean_x_in_window,
-                               (sum(self.x_data[:size]) + 7.0) /
+                               (sum(self.xData[:ws]) + 7.0) /
                                (self.smoother.window_size + 1.0))
 
         self.assertAlmostEqual(self.smoother._mean_y_in_window,
-                               (sum(self.y_data[:size]) + 8.0) /
+                               (sum(self.yData[:ws]) + 8.0) /
                                (self.smoother.window_size + 1.0))
 
     def test_mean_on_removal_of_observation(self):
-        """Make sure things work when we remove an observation."""
+        """
+        Make sure things work when we remove an observation
+        """
         self.smoother._remove_observation_from_means(3, 6)
 
         self.assertAlmostEqual(self.smoother._mean_x_in_window,
-                               sum(self.x_data[:2]) /
+                               sum(self.xData[:2]) /
                                (self.smoother.window_size - 1.0))
 
         self.assertAlmostEqual(self.smoother._mean_y_in_window,
-                               (sum(self.y_data[:2])) /
+                               (sum(self.yData[:2])) /
                                (self.smoother.window_size - 1.0))
 
     def test_variance_on_removal_of_observation(self):
-        """Make sure variance and covariance work when we remove an observation quickly."""
+        """
+        Make sure variance and covariance work when we remove an observation quickly
+        """
         self.smoother._remove_observation(3, 6)
 
         cov_from_update = self.smoother._covariance_in_window
         var_from_update = self.smoother._variance_in_window
 
         self.smoother._update_values_in_window()
         self.smoother._update_mean_in_window()
         self.smoother._update_variance_in_window()
 
         self.assertAlmostEqual(cov_from_update, self.smoother._covariance_in_window)
         self.assertAlmostEqual(var_from_update, self.smoother._variance_in_window)
 
     def test_variance_on_addition_of_observation(self):
-        """Make sure variance and covariance work when we remove an observation quickly."""
+        """
+        Make sure variance and covariance work when we remove an observation quickly
+        """
         self.smoother._add_observation(4, 7)
         cov_from_update = self.smoother._covariance_in_window
         var_from_update = self.smoother._variance_in_window
 
         self.smoother._update_values_in_window()
         self.smoother._update_mean_in_window()
         self.smoother._update_variance_in_window()
@@ -88,13 +97,13 @@
     def test_compute_smooth_during_construction(self):
         # test data is linear, so we just make sure we're on the line
         val = self.smoother._compute_smooth_during_construction(2.5)
         self.assertAlmostEqual(val, 5.5)
 
     def test_compute_cross_validated_residual_here(self):
         # weak test. Hard to do analytically without just repeating the method
-        residual = self.smoother._compute_cross_validated_residual_here(2.5, 5.6, 5.5)
-        self.assertNotEqual(residual, 0.0)
+        r = self.smoother._compute_cross_validated_residual_here(2.5, 5.6, 5.5)
+        self.assertNotEqual(r, 0.0)
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `ace-0.3.3/ace/validation/validate_smoothers.py` & `ace-0.3.post1/ace/validation/validate_smoothers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,102 +1,107 @@
-"""
-A few validation problems to make sure the smoothers are working as expected.
+'''
+A few validation problems to make sure the smoothers are working as expected
 
 These depend on the supsmu module, which was created using f2py from Breiman's supsmu.f
-"""
+'''
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot as plt
 import numpy
 
 from ace.samples import smoother_friedman82
 import ace.smoother as smoother
 import ace.supersmoother as supersmoother
 
-# pylint: disable=protected-access, missing-docstring
-
 try:
     import mace
 except ImportError:
     print("WARNING: An F2Pyd version of Breiman's supsmu is not available. "
           "Validations will not work")
     raise
 
 def validate_basic_smoother():
-    """Run Friedman's test from Figure 2b."""
+    """
+    Runs Friedman's test from Figure 2b.
+    """
     x, y = sort_data(*smoother_friedman82.build_sample_smoother_problem_friedman82())
     plt.figure()
     # plt.plot(x, y, '.', label='Data')
     for span in smoother.DEFAULT_SPANS:
         my_smoother = smoother.perform_smooth(x, y, span)
-        friedman_smooth, _resids = run_friedman_smooth(x, y, span)
+        friedman_smooth, resids = run_friedman_smooth(x, y, span)
         plt.plot(x, my_smoother.smooth_result, '.-', label='pyace span = {0}'.format(span))
         plt.plot(x, friedman_smooth, '.-', label='Friedman span = {0}'.format(span))
     finish_plot()
 
 
 def validate_basic_smoother_resid():
-    """Compare residuals."""
+    """
+    compare residuals
+    """
     x, y = sort_data(*smoother_friedman82.build_sample_smoother_problem_friedman82())
     plt.figure()
     for span in smoother.DEFAULT_SPANS:
         my_smoother = smoother.perform_smooth(x, y, span)
-        _friedman_smooth, resids = run_friedman_smooth(x, y, span)  # pylint: disable=unused-variable
-        plt.plot(x, my_smoother.cross_validated_residual, '.-',
-                 label='pyace span = {0}'.format(span))
+        friedman_smooth, resids = run_friedman_smooth(x, y, span)
+        plt.plot(x, my_smoother.cross_validated_residual, '.-', label='pyace span = {0}'.format(span))
         plt.plot(x, resids, '.-', label='Friedman span = {0}'.format(span))
     finish_plot()
 
 def validate_supersmoother():
-    """Validate the supersmoother."""
     x, y = smoother_friedman82.build_sample_smoother_problem_friedman82()
     x, y = sort_data(x, y)
     my_smoother = smoother.perform_smooth(x, y, smoother_cls=supersmoother.SuperSmootherWithPlots)
     # smoother.DEFAULT_BASIC_SMOOTHER = BasicFixedSpanSmootherBreiman
     supsmu_result = run_freidman_supsmu(x, y, bass_enhancement=0.0)
     mace_result = run_mace_smothr(x, y, bass_enhancement=0.0)
     plt.plot(x, y, '.', label='Data')
     plt.plot(x, my_smoother.smooth_result, '-', label='pyace')
     plt.plot(x, supsmu_result, '--', label='SUPSMU')
     plt.plot(x, mace_result, ':', label='SMOOTH')
     plt.legend()
     plt.savefig('supersmoother_validation.png')
 
 def validate_supersmoother_bass():
-    """Validate the supersmoother with extra bass."""
     x, y = smoother_friedman82.build_sample_smoother_problem_friedman82()
     plt.figure()
     plt.plot(x, y, '.', label='Data')
     for bass in range(0, 10, 3):
-        smooth = supersmoother.SuperSmoother()
-        smooth.set_bass_enhancement(bass)
-        smooth.specify_data_set(x, y)
-        smooth.compute()
-        plt.plot(x, smooth.smooth_result, '.', label='Bass = {0}'.format(bass))
+        smoother = supersmoother.SuperSmoother()
+        smoother._bass_enhancement = bass
+        smoother.specify_data_set(x, y)
+        smoother.compute()
+        plt.plot(x,
+                   smoother.smooth_result,
+                   '.',
+                   label='Bass = {0}'.format(bass))
         # pylab.plot(self.x, smoother.smooth_result, label='Bass = {0}'.format(bass))
     finish_plot()
 
-def validate_average_best_span():
-    """Figure 2d? from Friedman."""
+
+def validate_average_best_span(self):
+    """
+    Figure 2d? from Friedman
+    """
     N = 200
     num_trials = 400
     avg = numpy.zeros(N)
     for i in range(num_trials):
         x, y = smoother_friedman82.build_sample_smoother_problem_friedman82(N=N)
         my_smoother = smoother.perform_smooth(
-            x, y, smoother_cls=supersmoother.SuperSmoother
-        )
+                             x, y,
+                             smoother_cls=supersmoother.SuperSmoother)
         avg += my_smoother._smoothed_best_spans.smooth_result
         if not (i + 1) % 20:
             print(i + 1)
     avg /= num_trials
     plt.plot(my_smoother.x, avg, '.', label='Average JCV')
     finish_plot()
 
-def validate_known_curve():
-    """Validate on a sin function."""
+
+def validate_known_curve(self):
     plt.figure()
     N = 100
     x = numpy.linspace(-1, 1, N)
     y = numpy.sin(4 * x)
     smoother.DEFAULT_BASIC_SMOOTHER = smoother.BasicFixedSpanSmootherSlowUpdate
     smooth = smoother.perform_smooth(x, y, smoother_cls=supersmoother.SuperSmoother)
     plt.plot(x, smooth.smooth_result, label='Slow')
@@ -104,68 +109,62 @@
     smooth = smoother.perform_smooth(x, y, smoother_cls=supersmoother.SuperSmoother)
     plt.plot(x, smooth.smooth_result, label='Fast')
     plt.plot(x, y, '.', label='data')
     plt.legend()
     plt.show()
 
 def finish_plot():
-    """Help with plotting."""
     plt.legend()
     plt.grid(color='0.7')
     plt.xlabel('x')
     plt.ylabel('y')
     plt.show()
 
 def run_freidman_supsmu(x, y, bass_enhancement=0.0):
-    """Run the FORTRAN supersmoother."""
     N = len(x)
     weight = numpy.ones(N)
     results = numpy.zeros(N)
-    flags = numpy.zeros((N, 7))
-    mace.supsmu(x, y, weight, 1, 0.0, bass_enhancement, results, flags)
+    sc = numpy.zeros((N, 7))
+    mace.supsmu(x, y, weight, 1, 0.0, bass_enhancement, results, sc)
     return results
 
 def run_friedman_smooth(x, y, span):
-    """Run the FORTRAN smoother."""
     N = len(x)
     weight = numpy.ones(N)
     results = numpy.zeros(N)
     residuals = numpy.zeros(N)
     mace.smooth(x, y, weight, span, 1, 1e-7, results, residuals)
     return results, residuals
 
-def run_mace_smothr(x, y, bass_enhancement=0.0):  # pylint: disable=unused-argument
-    """Run the FORTRAN SMOTHR."""
+def run_mace_smothr(x, y, bass_enhancement=0.0):
     N = len(x)
     weight = numpy.ones(N)
     results = numpy.zeros(N)
-    flags = numpy.zeros((N, 7))
-    mace.smothr(1, x, y, weight, results, flags)
+    sc = numpy.zeros((N, 7))
+    mace.smothr(1, x, y, weight, results, sc)
     return results
 
 class BasicFixedSpanSmootherBreiman(smoother.Smoother):
-    """Runs FORTRAN Smooth."""
-
+    """
+    Runs FORTRAN Smooth
+    """
     def compute(self):
-        """Run smoother."""
-        self.smooth_result, self.cross_validated_residual = run_friedman_smooth(
-            self.x, self.y, self._span
-        )
+        self.smooth_result, self.cross_validated_residual = run_friedman_smooth(self.x, self.y, self._span)
 
 class SuperSmootherBreiman(smoother.Smoother):
-    """Run FORTRAN Supersmoother."""
-
+    """
+    Runs FORTRAN Supersmoother
+    """
     def compute(self):
-        """Run SuperSmoother."""
         self.smooth_result = run_freidman_supsmu(self.x, self.y)
         self._store_unsorted_results(self.smooth_result, numpy.zeros(len(self.smooth_result)))
 
 def sort_data(x, y):
-    """Sort the data."""
-    xy = sorted(zip(x, y))
+    xy = zip(x, y)
+    xy.sort()
     x, y = zip(*xy)
     return x, y
 
 if __name__ == '__main__':
     validate_basic_smoother()
     # validate_basic_smoother_resid()
     #validate_supersmoother()
```

### Comparing `ace-0.3.3/ace.egg-info/PKG-INFO` & `ace-0.3.post1/ace.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,180 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ace
-Version: 0.3.3
+Version: 0.3.post1
 Summary: Non-parametric multivariate regressions by Alternating Conditional Expectations
 Home-page: https://github.com/partofthething/ace
 Author: Nick Touran
 Author-email: ace@partofthething.com
 License: MIT
+Description: 
+        The ace Package
+        ===============
+        
+        ace is an implementation of the Alternating Conditional Expectation (ACE) algorithm [Breiman85]_,
+        which can be used to find otherwise difficult-to-find relationships between predictors
+        and responses and as a multivariate regression tool.
+        
+        The code for this project, as well as the issue tracker, etc. is
+        `hosted on GitHub <https://github.com/partofthething/ace>`_.
+        The documentation is hosted at http://partofthething.com/ace.
+        
+        What is it?
+        -----------
+        ACE can be used for a variety of purposes. With it, you can:
+        
+         - build easy-to-evaluate surrogate models of data. For example, if you are optimizing input
+           parameters to a complex and long-running simulation, you can feed the results of a parameter
+           sweep into ACE to get a model that will instantly give you predictions of results of any
+           combination of input within the parameter range.
+        
+         - expose interesting and meaningful relations between predictors and responses from complicated
+           data sets. For instance, if you have survey results from 1000 people and you and you want to
+           see how one answer is related to a bunch of others, ACE will help you.
+        
+        The fascinating thing about ACE is that it is a *non-parametric* multivariate regression
+        tool. This means that it doesn't make any assumptions about the functional form of the data.
+        You may be used to fitting polynomials or lines to data. Well, ACE doesn't do that. It
+        uses an iteration with a variable-span scatterplot smoother (implementing local least
+        squares estimates) to figure out the structure of your data. As you'll see, that
+        turns out to be a powerful difference.
+        
+        Installing it
+        -------------
+        ace is available in the `Python Package Index <https://pypi.python.org/pypi/ace/>`_,
+        and can be installed simply with the following.
+        
+        On Linux::
+        
+        	sudo pip install ace
+        
+        On Windows, use::
+        
+        	pip install ace
+        
+        or use the `GUI installer <http://partofthething.com/ace/builds/ace-0.2-1.win32.exe>`_.
+        
+        Directly from source::
+        
+        	git clone git@github.com:partofthething/ace.git
+        	cd ace
+        	python setup.py install
+        
+        .. note::
+        
+        	If you don't have git, you can just download the source directly from
+        	`here <https://github.com/partofthething/ace/archive/master.zip>`_.
+        
+        You can verify that the installation completed successfully by running the automated test
+        suite in the install directory::
+        
+        	python -m unittest discover -bv
+        
+        Using it
+        --------
+        To use, get some sample data:
+        
+        .. code:: python
+        
+            from ace.samples import wang04
+            x, y = wang04.build_sample_ace_problem_wang04(N=200)
+        
+        and run:
+        
+        .. code:: python
+        
+            from ace import model
+            myace = model.Model()
+            myace.build_model_from_xy(x, y)
+            myace.eval([0.1, 0.2, 0.5, 0.3, 0.5])
+        
+        For some plotting (matplotlib required), try:
+        
+        .. code:: python
+        
+            from ace import ace
+            ace.plot_transforms(myace.ace, fname = 'mytransforms.pdf')
+            myace.ace.write_transforms_to_file(fname = 'mytransforms.txt')
+        
+        Note that you could alternatively have loaded your data from a whitespace delimited
+        text file:
+        
+        .. code:: python
+        
+        	myace.build_model_from_txt(fname = 'myinput.txt')
+        
+        .. warning:: The more data points ACE is given as input, the better the results will be.
+        			 Be careful with less than 50 data points or so.
+        
+        Demo
+        ----
+        A clear demonstration of ace is available in the
+        `Sample ACE Problems <http://partofthething.com/ace/samples.html>`_ section.
+        
+        Other details
+        -------------
+        This implementation of ACE isn't as fast as the original FORTRAN version, but it can
+        still crunch through a problem with 5 independent variables having 1000 observations each
+        in on the order of 15 seconds. Not bad.
+        
+        ace also contains a pure-Python implementation of Friedman's SuperSmoother [Friedman82]_,
+        the variable-span smoother mentioned above. This can be useful on its own
+        for smoothing scatterplot data.
+        
+        History
+        -------
+        The ACE algorithm was published in 1985 by Breiman and Friedman [Breiman85]_, and the original
+        FORTRAN source code is available from `Friedman's webpage <http://statweb.stanford.edu/~jhf/>`_.
+        
+        Motivation
+        ----------
+        Before this package, the ACE algorithm has only been available in Python by using the rpy2 module
+        to load in the acepack package of the R statistical language. This package is a pure-Python
+        re-write of the ACE algorithm based on the original publication, using modern software practices.
+        This package is slower than the original FORTRAN code, but it is easier to understand. This package
+        should be suitable for medium-weight data and as a learning tool.
+        
+        For the record, it is also quite easy to run the original FORTRAN code in Python using f2py.
+        
+        About the Author
+        ----------------
+        This package was originated by Nick Touran, a nuclear engineer specializing in reactor physics.
+        He was exposed to ACE by his thesis advisor, Professor John Lee, and used it in his
+        Ph.D. dissertation to evaluate objective functions in a multidisciplinary
+        design optimization study of nuclear reactor cores [Touran12]_.
+        
+        License
+        -------
+        This package is released under the MIT License, reproduced
+        `here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
+        
+        References
+        ----------
+        .. [Breiman85] L. BREIMAN and J. H. FRIEDMAN, "Estimating optimal transformations for multiple regression and
+           correlation," Journal of the American Statistical Association, 80, 580 (1985).
+           `[Link1] <http://www.jstor.org/discover/10.2307/2288477?uid=2&uid=4&sid=21104902100507>`_
+        
+        .. [Friedman82] J. H. FRIEDMAN and W. STUETZLE, "Smoothing of scatterplots," ORION-003, Stanford
+           University, (1982). `[Link2] <http://www.slac.stanford.edu/cgi-wrap/getdoc/slac-pub-3013.pdf>`_
+        
+        .. [Wang04] D. WANG and M. MURPHY, "Estimating optimal transformations for multiple regression using the
+           ACE algorithm," Journal of Data Science, 2, 329 (2004).
+           `[Link3] <http://www.jds-online.com/files/JDS-156.pdf>`_
+        
+        .. [Touran12] N. TOURAN, "A Modal Expansion Equilibrium Cycle Perturbation Method for
+           Optimizing High Burnup Fast Reactors," Ph.D. dissertation, Univ. of Michigan, (2012).
+           `[The Thesis] <http://deepblue.lib.umich.edu/bitstream/handle/2027.42/95981/ntouran_1.pdf?sequence=1>`_
+        
+        
+        
 Keywords: regression ace multivariate statistics
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
-===============
-The ace Package
-===============
-
-.. image:: https://travis-ci.org/partofthething/ace.svg?branch=develop
-    :target: https://travis-ci.org/partofthething/ace
-    
-ace is an implementation of the Alternating Conditional Expectation (ACE) algorithm [Breiman85]_,
-which can be used to find otherwise difficult-to-find relationships between predictors
-and responses and as a multivariate regression tool.
-
-The code for this project, as well as the issue tracker, etc. is
-`hosted on GitHub <https://github.com/partofthething/ace>`_.
-The documentation is hosted at http://partofthething.com/ace.
-
-
-What is it?
------------
-ACE can be used for a variety of purposes. With it, you can:
-
- - build easy-to-evaluate surrogate models of data. For example, if you are optimizing input
-   parameters to a complex and long-running simulation, you can feed the results of a parameter
-   sweep into ACE to get a model that will instantly give you predictions of results of any
-   combination of input within the parameter range.
-
- - expose interesting and meaningful relations between predictors and responses from complicated
-   data sets. For instance, if you have survey results from 1000 people and you and you want to
-   see how one answer is related to a bunch of others, ACE will help you.
-
-The fascinating thing about ACE is that it is a *non-parametric* multivariate regression
-tool. This means that it doesn't make any assumptions about the functional form of the data.
-You may be used to fitting polynomials or lines to data. Well, ACE doesn't do that. It
-uses an iteration with a variable-span scatterplot smoother (implementing local least
-squares estimates) to figure out the structure of your data. As you'll see, that
-turns out to be a powerful difference.
-
-Installing it
--------------
-ace is available in the `Python Package Index <https://pypi.python.org/pypi/ace/>`_,
-and can be installed simply with the following.
-
-On Linux::
-
-	sudo pip install ace
-
-On Windows, use::
-
-	pip install ace
-
-Directly from source::
-
-	git clone git@github.com:partofthething/ace.git
-	cd ace
-	python setup.py install
-
-.. note::
-
-	If you don't have git, you can just download the source directly from
-	`here <https://github.com/partofthething/ace/archive/master.zip>`_.
-
-You can verify that the installation completed successfully by running the automated test
-suite in the install directory::
-
-	python -m unittest discover -bv
-
-Using it
---------
-To use, get some sample data:
-
-.. code:: python
-
-    from ace.samples import wang04
-    x, y = wang04.build_sample_ace_problem_wang04(N=200)
-
-and run:
-
-.. code:: python
-
-    from ace import model
-    myace = model.Model()
-    myace.build_model_from_xy(x, y)
-    myace.eval([0.1, 0.2, 0.5, 0.3, 0.5])
-
-For some plotting (matplotlib required), try:
-
-.. code:: python
-
-    from ace import ace
-    ace.plot_transforms(myace.ace, fname = 'mytransforms.pdf')
-    myace.ace.write_transforms_to_file(fname = 'mytransforms.txt')
-
-Note that you could alternatively have loaded your data from a whitespace delimited
-text file:
-
-.. code:: python
-
-	myace.build_model_from_txt(fname = 'myinput.txt')
-
-.. warning:: The more data points ACE is given as input, the better the results will be.
-			 Be careful with less than 50 data points or so.
-
-Demo
-----
-A combination of various functions with noise is shown below:
-
-.. have to use full path here to work in built docs and github-rendered README
-
-.. image:: https://partofthething.com/ace/_static/ace_input_wang04.png
-	   :alt: Plot of the input data, which is all over the place
-
-Given just those points and zero knowledge of the underlying functions, ACE comes back
-with this:
-
-.. image:: https://partofthething.com/ace/_static/ace_transforms_wang04.png
-	:alt: Plot of the output transforms, which clearly show the underlying structure
-
-
-A longer version of this demo is available in the
-`Sample ACE Problems <http://partofthething.com/ace/samples.html>`_ section.
-
-Other details
--------------
-This implementation of ACE isn't as fast as the original FORTRAN version, but it can
-still crunch through a problem with 5 independent variables having 1000 observations each
-in on the order of 15 seconds. Not bad.
-
-ace also contains a pure-Python implementation of Friedman's SuperSmoother [Friedman82]_,
-the variable-span smoother mentioned above. This can be useful on its own
-for smoothing scatterplot data.
-
-History
--------
-The ACE algorithm was published in 1985 by Breiman and Friedman [Breiman85]_, and the original
-FORTRAN source code is available from `Friedman's webpage <http://statweb.stanford.edu/~jhf/>`_.
-
-Motivation
-----------
-Before this package, the ACE algorithm has only been available in Python by using the rpy2 module
-to load in the acepack package of the R statistical language. This package is a pure-Python
-re-write of the ACE algorithm based on the original publication, using modern software practices.
-This package is slower than the original FORTRAN code, but it is easier to understand. This package
-should be suitable for medium-weight data and as a learning tool.
-
-For the record, it is also quite easy to run the original FORTRAN code in Python using f2py.
-
-About the Author
-----------------
-This package was originated by Nick Touran, a nuclear engineer specializing in reactor physics.
-He was exposed to ACE by his thesis advisor, Professor John Lee, and used it in his
-Ph.D. dissertation to evaluate objective functions in a multidisciplinary
-design optimization study of nuclear reactor cores [Touran12]_.
-
-License
--------
-This package is released under the MIT License, `reproduced
-here <https://github.com/partofthething/ace/blob/master/LICENSE>`_.
-
-References
-----------
-.. [Breiman85] L. BREIMAN and J. H. FRIEDMAN, "Estimating optimal transformations for multiple regression and
-   correlation," Journal of the American Statistical Association, 80, 580 (1985).
-   `[Link1] <http://www.jstor.org/discover/10.2307/2288477?uid=2&uid=4&sid=21104902100507>`_
-
-.. [Friedman82] J. H. FRIEDMAN and W. STUETZLE, "Smoothing of scatterplots," ORION-003, Stanford
-   University, (1982). `[Link2] <http://www.slac.stanford.edu/cgi-wrap/getdoc/slac-pub-3013.pdf>`_
-
-.. [Wang04] D. WANG and M. MURPHY, "Estimating optimal transformations for multiple regression using the
-   ACE algorithm," Journal of Data Science, 2, 329 (2004).
-   `[Link3] <http://www.jds-online.com/files/JDS-156.pdf>`_
-
-.. [Touran12] N. TOURAN, "A Modal Expansion Equilibrium Cycle Perturbation Method for
-   Optimizing High Burnup Fast Reactors," Ph.D. dissertation, Univ. of Michigan, (2012).
-   `[The Thesis] <http://deepblue.lib.umich.edu/bitstream/handle/2027.42/95981/ntouran_1.pdf?sequence=1>`_
-
-
```

### Comparing `ace-0.3.3/ace.egg-info/SOURCES.txt` & `ace-0.3.post1/ace.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.rst
 setup.py
 ace/__init__.py
 ace/ace.py
 ace/model.py
 ace/smoother.py
 ace/supersmoother.py
@@ -17,8 +16,9 @@
 ace/samples/supersmoother_friedman82.py
 ace/samples/wang04.py
 ace/tests/__init__.py
 ace/tests/test_ace.py
 ace/tests/test_model.py
 ace/tests/test_smoother.py
 ace/validation/__init__.py
+ace/validation/run_supsmu.py
 ace/validation/validate_smoothers.py
```

### Comparing `ace-0.3.3/setup.py` & `ace-0.3.post1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     long_description = f.read()
 
-setup(
-    name='ace',
-    version='0.3.3',
-    description=
-    'Non-parametric multivariate regressions by Alternating Conditional Expectations',
+setup(name='ace',
+    version='0.3-1',
+    description='Non-parametric multivariate regressions by Alternating Conditional Expectations',
     author='Nick Touran',
     author_email='ace@partofthething.com',
     url='https://github.com/partofthething/ace',
     packages=find_packages(),
     license='MIT',
     long_description=long_description,
-    install_requires=['numpy', 'scipy>=0.17'],
+    install_requires=['numpy', 'scipy'],
     keywords='regression ace multivariate statistics',
+    use_2to3=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.2',
+        'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    test_suite='tests')
+        ],
+      test_suite='tests'
+
+     )
```

