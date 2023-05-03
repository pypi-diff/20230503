# Comparing `tmp/sigProfilerPlotting-1.3.8.tar.gz` & `tmp/sigProfilerPlotting-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigProfilerPlotting-1.3.8.tar", last modified: Wed Dec 14 23:57:49 2022, max compression
+gzip compressed data, was "sigProfilerPlotting-1.3.9.tar", last modified: Tue Jan 10 21:07:44 2023, max compression
```

## Comparing `sigProfilerPlotting-1.3.8.tar` & `sigProfilerPlotting-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-12-14 23:57:49.813445 sigProfilerPlotting-1.3.8/
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     1341 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/LICENSE
--rw-r--r--   0 mbarnes    (501) staff       (20)       15 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/MANIFEST.in
--rw-r--r--   0 mbarnes    (501) staff       (20)     6835 2022-12-14 23:57:49.813146 sigProfilerPlotting-1.3.8/PKG-INFO
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     6517 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/README.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-12-14 23:57:49.798868 sigProfilerPlotting-1.3.8/fonts/
--rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Arial Bold.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   773236 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Arial.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   691796 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Courier New Bold.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   684624 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Courier New.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   842168 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Times New Roman Bold.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   834452 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/Times New Roman.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)        0 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/fonts/__init__.py
--rw-r--r--   0 mbarnes    (501) staff       (20)       38 2022-12-14 23:57:49.813552 sigProfilerPlotting-1.3.8/setup.cfg
--rw-r--r--   0 mbarnes    (501) staff       (20)     3211 2022-12-14 23:55:12.000000 sigProfilerPlotting-1.3.8/setup.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-12-14 23:57:49.809944 sigProfilerPlotting-1.3.8/sigProfilerPlotting/
--rw-r--r--   0 mbarnes    (501) staff       (20)       84 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/__init__.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     6283 2022-11-28 17:26:57.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/plotActivity.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    99392 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/sample_portrait.py
--rw-r--r--   0 mbarnes    (501) staff       (20)   227233 2022-12-14 23:55:00.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/sigProfilerPlotting.py
--rw-r--r--   0 mbarnes    (501) staff       (20)   182559 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/sigProfilerPlotting_old.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     4669 2022-11-28 04:05:10.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/tmbplot.py
--rw-r--r--   0 mbarnes    (501) staff       (20)      111 2022-12-14 23:57:48.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting/version.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-12-14 23:57:49.812663 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/
--rw-r--r--   0 mbarnes    (501) staff       (20)     6835 2022-12-14 23:57:49.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)      714 2022-12-14 23:57:49.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/SOURCES.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-12-14 23:57:49.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/dependency_links.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-11-28 04:06:45.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/not-zip-safe
--rw-r--r--   0 mbarnes    (501) staff       (20)       60 2022-12-14 23:57:49.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/requires.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       20 2022-12-14 23:57:49.000000 sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/top_level.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2023-01-10 21:07:44.813016 sigProfilerPlotting-1.3.9/
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     1341 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/LICENSE
+-rw-r--r--   0 mbarnes    (501) staff       (20)       15 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/MANIFEST.in
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6835 2023-01-10 21:07:44.812193 sigProfilerPlotting-1.3.9/PKG-INFO
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     6517 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/README.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2023-01-10 21:07:44.799913 sigProfilerPlotting-1.3.9/fonts/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Arial Bold.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   773236 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Arial.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   691796 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Courier New Bold.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   684624 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Courier New.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   842168 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Times New Roman Bold.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   834452 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/Times New Roman.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)        0 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/fonts/__init__.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)       38 2023-01-10 21:07:44.813249 sigProfilerPlotting-1.3.9/setup.cfg
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3203 2023-01-10 21:07:33.000000 sigProfilerPlotting-1.3.9/setup.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2023-01-10 21:07:44.806705 sigProfilerPlotting-1.3.9/sigProfilerPlotting/
+-rw-r--r--   0 mbarnes    (501) staff       (20)       84 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/__init__.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6283 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/plotActivity.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    99392 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/sample_portrait.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)   225244 2023-01-10 21:07:33.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/sigProfilerPlotting.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)   182559 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/sigProfilerPlotting_old.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4669 2023-01-10 20:59:42.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/tmbplot.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)      111 2023-01-10 21:07:43.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting/version.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2023-01-10 21:07:44.811437 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6835 2023-01-10 21:07:43.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)      714 2023-01-10 21:07:44.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2023-01-10 21:07:43.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2023-01-10 21:07:43.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/not-zip-safe
+-rw-r--r--   0 mbarnes    (501) staff       (20)       52 2023-01-10 21:07:44.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/requires.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       20 2023-01-10 21:07:44.000000 sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/top_level.txt
```

### Comparing `sigProfilerPlotting-1.3.8/LICENSE` & `sigProfilerPlotting-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/PKG-INFO` & `sigProfilerPlotting-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigProfilerPlotting
-Version: 1.3.8
+Version: 1.3.9
 Summary: SigProfiler plotting tool
 Home-page: https://github.com/alexandrovlab/SigProfilerPlotting
 Author: Erik Bergstrom
 Author-email: ebergstr@eng.ucsd.edu
 License: UCSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sigProfilerPlotting-1.3.8/README.md` & `sigProfilerPlotting-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Arial Bold.ttf` & `sigProfilerPlotting-1.3.9/fonts/Arial Bold.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Arial.ttf` & `sigProfilerPlotting-1.3.9/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Courier New Bold.ttf` & `sigProfilerPlotting-1.3.9/fonts/Courier New Bold.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Courier New.ttf` & `sigProfilerPlotting-1.3.9/fonts/Courier New.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Times New Roman Bold.ttf` & `sigProfilerPlotting-1.3.9/fonts/Times New Roman Bold.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/fonts/Times New Roman.ttf` & `sigProfilerPlotting-1.3.9/fonts/Times New Roman.ttf`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/setup.py` & `sigProfilerPlotting-1.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if os.path.exists("dist"):
     shutil.rmtree("dist")
 
 def readme():
 	with open('README.rst') as f:
 		return(f.read())
 
-VERSION = '1.3.8'
+VERSION = '1.3.9'
 
 def write_version_py(filename='sigProfilerPlotting/version.py'):
     # Copied from numpy setup.py
     cnt = """
 # THIS FILE IS GENERATED FROM SIGPROFILERPLOTTING SETUP.PY
 short_version = '%(version)s'
 version = '%(version)s'
@@ -81,14 +81,14 @@
         long_description_content_type="text/markdown",
 		url='https://github.com/alexandrovlab/SigProfilerPlotting',
 		author='Erik Bergstrom',
 		author_email='ebergstr@eng.ucsd.edu',
 		license='UCSD',
 		packages=['sigProfilerPlotting'],
 		install_requires =[
-			"matplotlib>=3.3.0,<=3.4.3", "pandas>=1.2.4", "scikit-learn>=1.1.3"],
+			"matplotlib>=3.4.3", "pandas>=1.2.4", "scikit-learn>=1.1.3"],
         package_data={'':['fonts/*.ttf']},
 		include_package_data=True,
 	    #Specify the custom install class
 	    cmdclass={'install' : move_ttf},
 		zip_safe=False)
```

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting/plotActivity.py` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting/plotActivity.py`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting/sample_portrait.py` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting/sample_portrait.py`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting/sigProfilerPlotting.py` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting/sigProfilerPlotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,35 @@
 import copy
 import errno
 
 MUTTYPE="MutationType"
 
 warnings.filterwarnings("ignore")
 
+def process_input(matrix_path):
+	# input data is a DataFrame
+	if isinstance(matrix_path, pd.DataFrame):
+		data = matrix_path
+		if MUTTYPE in data.columns:
+			data = data.set_index(MUTTYPE, drop=True)
+		else:
+			data.rename(columns={data.columns[0]:MUTTYPE}, inplace=True)
+			data = data.set_index(MUTTYPE, drop=True)
+	# input data is a path to a file
+	elif isinstance(matrix_path, str):
+		data=pd.read_csv(matrix_path,sep='\t',index_col=0)
+		data=data.dropna(axis=1, how='all')
+	else:
+		raise ValueError("ERROR: matrix_path requires path to file or DataFrame.")
+
+	if data.isnull().values.any():
+		raise ValueError("Input data contains Nans.")
+
+	return data
+
 def temp_plotsave(output_path,project,figs_orig):
     pp = PdfPages(output_path + 'SBS_288_testst_plots_' + project + '.pdf')
     figs_orig.savefig(pp, format='pdf')
     pp.close()
 
 def get_default_96labels():
     first=['A','C','G','T']
@@ -985,42 +1006,19 @@
 	"""
 	plot_custom_text = False
 	sig_probs = False
 	pcawg = False
 
 	if plot_type == '96':
 		try:
-			# input data is a DataFrame
-			if isinstance(matrix_path, pd.DataFrame):
-				data = matrix_path
-				if MUTTYPE in data.columns:
-					data = data.set_index(MUTTYPE, drop=True)
-				else:
-					data.rename(columns={data.columns[0]:MUTTYPE}, inplace=True)
-					data = data.set_index(MUTTYPE, drop=True)
-
-			# input data is a path to a file
-			elif isinstance(matrix_path, str):
-				data=pd.read_csv(matrix_path,sep='\t',index_col=0)
-				data=data.dropna(axis=1, how='all')
-			else:
-				raise ValueError("ERROR: plotSBS requires path to file or DataFrame.")
-
-			if data.isnull().values.any():
-				raise ValueError("Input data contains Nans.")
-			
-			data= reindex_sbs96(data)
+			data = process_input(matrix_path)
+			data = reindex_sbs96(data)
 			sample_count = 0
 
-
 			buf= io.BytesIO()
-			# try:
-			# 	fig_orig=pickle.load(open(spplt.__path__[0]+'/templates/SBS96.pkl','rb'))
-			# 	pickle.dump(fig_orig, buf)
-			# except:
 			fig_orig=make_pickle_file(context='SBS96',path='SBS96.pkl', return_plot_template=True)
 			pickle.dump(fig_orig, buf)
 
 			figs={}
 			buff_list={}
 			ctx = data.index #[seq[0]+seq[2]+seq[6] for seq in data.index]
 			colors = [[3/256,189/256,239/256], [1/256,1/256,1/256],[228/256,41/256,38/256], [203/256,202/256,202/256], [162/256,207/256,99/256], [236/256,199/256,197/256]]
@@ -3388,20 +3386,15 @@
 
 	elif plot_type == '288':
 		try:
 			plot_custom_text = False
 			sig_probs = False
 			pcawg = False
 
-			if not isinstance(matrix_path, pd.DataFrame):
-				data=pd.read_csv(matrix_path,sep='\t',index_col=0)
-				data=data.dropna(axis=1, how='all')
-
-			if data.isnull().values.any():
-				raise ValueError("Input data contains Nans.")
+			data = process_input(matrix_path)
 		
 			sample_count = 0
 
 			data,tsb_mats = reindex_sbs288(data)
 			buf= io.BytesIO()
 			# try:
 			# 	fig_orig=pickle.load(open(spplt.__path__[0]+'/templates/SBS288.pkl','rb'))
@@ -3932,46 +3925,22 @@
 	#   del matplotlib.font_manager.weight_dict['roman']
 	#   matplotlib.font_manager._rebuild()
 	plot_custom_text = False
 	sig_probs = False
 	pcawg = False
 	if plot_type == '94' or plot_type == 'ID94' or plot_type == '94ID' or plot_type == '83':
 
-		# input data is a DataFrame
-		if isinstance(matrix_path, pd.DataFrame):
-			data = matrix_path
-			if MUTTYPE in data.columns:
-				data = data.set_index(MUTTYPE, drop=True)
-			else:
-				data.rename(columns={data.columns[0]:MUTTYPE}, inplace=True)
-				data = data.set_index(MUTTYPE, drop=True)
-
-		# input data is a path to a file
-		elif isinstance(matrix_path, str):
-			data=pd.read_csv(matrix_path,sep='\t',index_col=0)
-			data=data.dropna(axis=1, how='all')
-		else:
-			raise ValueError("ERROR: plotSBS requires path to file or DataFrame.")
-
-		if data.isnull().values.any():
-			raise ValueError("Input data contains Nans.")
+		data = process_input(matrix_path)
 		
 		try:
 			sample_count = 0
 			buf= io.BytesIO()
-			# try:
-			# 	fig_orig=pickle.load(open(spplt.__path__[0]+'/templates/ID83.pkl','rb'))
-			# 	pickle.dump(fig_orig, buf)
-			# except:
 			fig_orig=make_pickle_file(context='ID83',path='ID83.pkl', return_plot_template=True)
 			pickle.dump(fig_orig, buf)
-
-
 			figs={}
-
 			colors = [[253/256,190/256,111/256], [255/256,128/256,2/256], [176/256,221/256,139/256], [54/256,161/256,46/256],
 							[253/256,202/256,181/256], [252/256,138/256,106/256], [241/256,68/256,50/256], [188/256,25/256,26/256],
 							[208/256,225/256,242/256], [148/256,196/256,223/256], [74/256,152/256,201/256], [23/256,100/256,171/256],
 							[226/256,226/256,239/256], [182/256,182/256,216/256], [134/256,131/256,189/256], [98/256,64/256,155/256]]
 			ctx = data.index
 			xlabels= [i.split(":")[0]+i.split(":")[1]+i.split(":")[2] for i in ctx.to_list()]
 			xlables_set= ['1DelC', '1DelT', '1InsC', '1InsT', '2DelR', '3DelR', '4DelR', '5DelR', '2InsR','3InsR','4InsR','5InsR', '2DelM', '3DelM','4DelM','5DelM']
@@ -4741,43 +4710,19 @@
 
 
 	else:
 		print("The provided plot_type:", plot_type, "is not supported by this plotting function")
 
 def plotDBS(matrix_path, output_path, project, plot_type, percentage=False, custom_text_upper=None, custom_text_middle=None, custom_text_bottom=None,savefig_format='pdf'):
 
-
-    # context ='DBS78'
-    # package_path = spplt.__path__[0]
-    # install_path =os.path.join(package_path,'templates/')
-    # if not os.path.exists(install_path):
-    #     os.mkdir(install_path)
-
-    # filename= os.path.join(install_path,context+'.pkl')
-    # getdbstemp(context,path=filename)
 	plot_custom_text = False
 	pcawg = False
 	sig_probs = False
 	if plot_type == '78' or plot_type == '78DBS' or plot_type == 'DBS78':
-		if not isinstance(matrix_path, pd.DataFrame):
-			data=pd.read_csv(matrix_path,sep='\t',index_col=0)
-			data=data.dropna(axis=1, how='all')
-
-		if data.isnull().values.any():
-			raise ValueError("Input data contains Nans.")
-		# with open(matrix_path) as f:
-		#     next(f)
-		#     first_line = f.readline()
-		#     first_line = first_line.strip().split()
-		#     mutation_type = first_line[0]
-		#     if first_line[0][2] != ">":
-		#         pcawg = True
-		#     if len(mutation_type) != 5 and first_line[0][2] == ">":
-		#         sys.exit("The matrix does not match the correct DBS96 format. Please check you formatting and rerun this plotting function.")
-		# pp = PdfPages(output_path + 'DBS_78_plots_' + project + '.pdf')
+		data = process_input(matrix_path)
 
 		dinucs = ['TT>GG','TT>CG','TT>AG','TT>GC','TT>CC','TT>AC','TT>GA','TT>CA','TT>AA','AC>CA','AC>CG','AC>CT','AC>GA',
 					'AC>GG','AC>GT','AC>TA','AC>TG','AC>TT','CT>AA','CT>AC','CT>AG','CT>GA','CT>GC','CT>GG','CT>TG','CT>TC',
 					'CT>TA','AT>CA','AT>CC','AT>CG','AT>GA','AT>GC','AT>TA','TG>GT','TG>CT','TG>AT','TG>GC','TG>CC','TG>AC',
 					'TG>GA','TG>CA','TG>AA','CC>AA','CC>AG','CC>AT','CC>GA','CC>GG','CC>GT','CC>TA','CC>TG','CC>TT','CG>AT',
 					'CG>GC','CG>GT','CG>TC','CG>TA','CG>TT','TC>GT','TC>CT','TC>AT','TC>GG','TC>CG','TC>AG','TC>GA','TC>CA',
 					'TC>AA','GC>AA','GC>AG','GC>AT','GC>CA','GC>CG','GC>TA','TA>GT','TA>CT','TA>AT','TA>GG','TA>CG','TA>GC']
```

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting/sigProfilerPlotting_old.py` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting/sigProfilerPlotting_old.py`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting/tmbplot.py` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting/tmbplot.py`

 * *Files identical despite different names*

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/PKG-INFO` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigProfilerPlotting
-Version: 1.3.8
+Version: 1.3.9
 Summary: SigProfiler plotting tool
 Home-page: https://github.com/alexandrovlab/SigProfilerPlotting
 Author: Erik Bergstrom
 Author-email: ebergstr@eng.ucsd.edu
 License: UCSD
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `sigProfilerPlotting-1.3.8/sigProfilerPlotting.egg-info/SOURCES.txt` & `sigProfilerPlotting-1.3.9/sigProfilerPlotting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

