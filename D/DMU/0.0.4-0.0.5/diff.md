# Comparing `tmp/DMU-0.0.4.tar.gz` & `tmp/DMU-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMU-0.0.4.tar", last modified: Thu Aug 25 10:07:57 2022, max compression
+gzip compressed data, was "DMU-0.0.5.tar", last modified: Wed May  3 13:08:37 2023, max compression
```

## Comparing `DMU-0.0.4.tar` & `DMU-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-25 10:07:57.746158 DMU-0.0.4/
-drwxrwxrwx   0        0        0        0 2022-08-25 10:07:57.730533 DMU-0.0.4/DMU/
--rw-rw-rw-   0        0        0        0 2022-08-25 10:07:31.000000 DMU-0.0.4/DMU/__init__.py
--rw-rw-rw-   0        0        0      713 2022-08-25 10:07:31.000000 DMU-0.0.4/DMU/graph_styles.py
--rw-rw-rw-   0        0        0    86473 2022-08-25 10:07:31.000000 DMU-0.0.4/DMU/utils.py
-drwxrwxrwx   0        0        0        0 2022-08-25 10:07:57.730533 DMU-0.0.4/DMU.egg-info/
--rw-rw-rw-   0        0        0    11119 2022-08-25 10:07:57.000000 DMU-0.0.4/DMU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2022-08-25 10:07:57.000000 DMU-0.0.4/DMU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-25 10:07:57.000000 DMU-0.0.4/DMU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-08-25 10:07:57.000000 DMU-0.0.4/DMU.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-08-25 10:07:57.000000 DMU-0.0.4/DMU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1102 2022-08-25 10:07:31.000000 DMU-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    11119 2022-08-25 10:07:57.746158 DMU-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10503 2022-08-25 10:07:31.000000 DMU-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2022-08-25 10:07:57.746158 DMU-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3608 2022-08-25 10:07:31.000000 DMU-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.620279 DMU-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.604689 DMU-0.0.5/DMU/
+-rw-rw-rw-   0        0        0        0 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/graph_styles.py
+-rw-rw-rw-   0        0        0    92377 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.620279 DMU-0.0.5/DMU.egg-info/
+-rw-rw-rw-   0        0        0    11119 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1102 2023-05-03 13:07:59.000000 DMU-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    11119 2023-05-03 13:08:37.620279 DMU-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10503 2023-05-03 13:07:59.000000 DMU-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:08:37.620279 DMU-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3608 2023-05-03 13:07:59.000000 DMU-0.0.5/setup.py
```

### Comparing `DMU-0.0.4/DMU/graph_styles.py` & `DMU-0.0.5/DMU/graph_styles.py`

 * *Files identical despite different names*

### Comparing `DMU-0.0.4/DMU/utils.py` & `DMU-0.0.5/DMU/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,24 +53,25 @@
 
 #%%
 
 def bias_plotter(data,ax,**kwargs): 
     keys = list(data.keys())
     kwargdict = {'fwd':'fwd','f':'fwd','forward':'fwd',
                  'bwd':'rev','rev':'rev','reverse':'rev',
-                 'title':'title','tit':'title'}
+                 'title':'title','tit':'title',
+                 'labels':'labels','lbl':'labels'}
     
     kuniq = np.unique(list(kwargdict.keys()))
     Pkwargs = {}
     #Filtering out the function kwargs from the plot kwargs
     for key in kwargs.keys():
         if key not in kuniq:
             kwargdict[key] = key
     #Collecting kwargs
-    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None)
+    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None, labels=[None,None])
     xkey = []; ykey = []; fwdbwd = []
     
     for k in keys:
         if "bias" in k.lower():
             xkey.append(k)
             
         if "bwd" not in k.lower() and "bias" not in k.lower():
@@ -80,37 +81,128 @@
         if "bwd" in k.lower() and "bias" not in k.lower():
             ykey.append(k)
             fwdbwd.append(1) #Note: 0  is forward, 1 is backwards
     
     for key,val in kwargs.items():
         if key not in kuniq:
             Pkwargs[key] = val
+
     for n,i in enumerate(fwdbwd):    
         plotkwargs = {}
         for k,v in Pkwargs.items():
             try: 
                 plotkwargs[k] = v[i]
             except:
                 plotkwargs[k] = v
     
         if kw.fwd == True and i == 0:
-
-            ax.plot(data[xkey[0]],data[ykey[i]],label='Forward',**plotkwargs)
+            if kw.labels[0] is None:
+                kw.labels[0] = "Forward"
+                
+            ax.plot(data[xkey[0]],data[ykey[i]],label=kw.labels[0],**plotkwargs)
             
         
         if kw.rev == True and i == 1:
-            ax.plot(data[xkey[0]],data[ykey[i]],label='Backward',**plotkwargs)        
+            if kw.labels[1] is None:
+                kw.labels[1] = "Backward"
+            ax.plot(data[xkey[0]],data[ykey[i]],label=kw.labels[1],**plotkwargs)        
     ax.set_xlabel(xkey[0])
     ax.set_ylabel(ykey[fwdbwd[0]])
     
     ax.legend()
     ax.set_title(kw.title)
 
 #%%
+def Single_NW_Diagram_Plotter(fig,ax,NanonisDat):
+    """
+    Parameters
+    ----------
+    ax : TYPE
+        DESCRIPTION.
+    labels : list: [port 1, port 2, port 3, port 4]
+    types : list: [bias, sweep, ground, ground]
+    plots a nanowire diagram
+    """ 
+    arrow_style = {
+    "head_width": 0.1,
+    "head_length": 0.2,
+    "color":"k"}
+    axobjs = []
+    Device = NanonisDat['device']
+    Portd =  [NanonisDat['Port'+n] for n in ['1','2','3','4']]
+    
+    if "Comment06" in list(NanonisDat.keys()):
+        comment = NanonisDat["Comment06"]
+    
+    dxW = 0.05
+    dyH = 0.05
+    
+    nwl = 0.065
+    nwh = 0.018
+    nwp = 0.003
+    c   = [0.825,0.175]
+    gctf = 1
+    
+    gcbl = gctf*nwl/3
+    gcbh = gctf*nwl/2
+    gcsl = nwh*gctf/3
+    gcsh = gctf*nwl
+    
+    ##Nanowire Creation
+    nw1 = ax.add_patch(ptc.Rectangle(
+    (c[0]-nwp-nwl, c[1]-nwh/2), # lower left point of rectangle
+    nwl, nwh,   # width/height of rectangle
+    facecolor="purple", edgecolor="darkorchid",alpha=1,zorder=2,transform=fig.transFigure
+    ))
+    labels = []
+    types  = []
+    
+    for i,port in enumerate(Portd):
+        if port['pos'] != None:
+            labels.append('Port'+str(i+1))
+            if port['current'] == True:
+                types.append('current')
+            
+            elif port['bias'] != False: 
+                types.append('bias')
+            
+            elif port['sweep'] != False:
+                types.append('sweep')
+            
+            elif port['ground'] == True:
+                types.append('ground')
+            
+            if "tip" in port['NW'] and port['pos'] == 2:
+                gp1_pos = (c[0]-nwp, c[1])
+            elif "tip" in port['NW'] and port['pos'] == 1:
+                gp1_pos = (c[0]-nwp-nwl, c[1])
 
+    gp1 = ax.add_patch(plt.Circle(gp1_pos, radius=nwh/2, facecolor="gold",edgecolor='orange',transform=fig.transFigure))
+    
+    axobjs = [nw1,gp1]
+    
+    portlocs      = [(c[0]-nwp-nwl-gcbl, c[1]),(c[0]+gcbl, c[1])]
+    porttextloc   = [(c[0]-nwp-nwl-4*gcbl, c[1]),(c[0]+gcbl, c[1])]
+    typetextloc   = [(c[0]-nwp-nwl-4*gcbl, c[1]-1.3*gcbl),(c[0]+gcbl, c[1]+1.3*gcbl)]
+    # porttextloc   = [(c[0]-nwp-nwl-4.8*gcbl, c[1]),(c[0]-nwp-nwh*gctf+1/2*gcsl, c+gcsh),(c[0]+nwp+nwh*gctf-1/2*gcsl, c[1]5-gcsh),(c[0]+nwp+nwl+2*gcbl, c[1])]
+    for i,lab in enumerate(labels):
+        axobjs.append(ax.annotate(labels[i],
+                  xy=portlocs[i],
+                  xytext=porttextloc[i], verticalalignment='center',
+                  xycoords = fig.transFigure, textcoords=fig.transFigure))
+        
+        typecolour = {'ground':"brown",'current':"blue",'bias':"green",'sweep':'red'}
+    
+        axobjs.append(ax.annotate(types[i],
+                  xy=portlocs[i],
+                  xytext=typetextloc[i], verticalalignment='center', color=typecolour[types[i].strip()],
+                  xycoords = fig.transFigure, textcoords=fig.transFigure))
+        #,arrowprops=dict(facecolor='black', shrink=0.05,width=1,headwidth=5,headlength=5)
+
+    
 def Nanowire_Diagram_Plotter(fig,ax,NanonisDat):
     """
     Parameters
     ----------
     ax : TYPE
         DESCRIPTION.
     labels : list: [port 1, port 2, port 3, port 4]
@@ -992,15 +1084,61 @@
     
     #Labelling and Gridding
     fig[0].ax[0].set_xlabel(xlab)
     fig[0].ax[0].set_ylabel(ylab)
     fig[0].ax[0].grid(True)
     return(fig)
     
-#%% 
+#%%
+class cmap_seq(object):
+    """
+    Goal of class: use for colourmapping profiles such that:
+        - cmap types can be selected
+        - The range of values before their full colour contents is selected
+        - Alternatively the increment between each cmap value can be selected
+        - Invoking the class allows the next value to be given (as to not rely on the for loop i)
+        - Allowing for the class to be reset
+    """
+    def __init__(self,**kwargs):
+        self.cmap = None
+        self.i    = 0
+
+        """
+        kwargs:
+            ==============
+            cmap:  the name of the colormap you wish to use
+            steps: the number of increments of the colormap between first and last values
+            custom: enables custom mode where colour 1 and colour 2 (and the interp between them) can be seleced
+            col1: colour 1
+            col2: colour 2
+            interp: value for interpolation speed (number of points between col1 and col2)
+        """
+        
+    def set_cmap(self,**kwargs):
+        import matplotlib.cm as mcm
+        kwargdict = {'cmap':'cmap','colormap':'cmap','colourmap':'cmap',
+                     'steps':'steps','step':'steps','N':'steps',
+                     'custom':'custom','cust':'custom',
+                     'col1':'col1','color1':'col1','colour1':'col1',
+                     'col2':'col2','color2':'col2','colour2':'col2',
+                     'interp':'interp','interpolation':'interp'}
+        kuniq = np.unique(list(kwargdict.keys()))
+        kw = KwargEval(kwargs, kwargdict, cmap='viridis',steps=100,custom=False,col1=None,col2=None,interp=None)
+
+        self.cmap = mcm.get_cmap(kw.cmap,kw.steps)
+        self.col  = self.cmap(self.i)
+        
+    def iter_cmap(self):
+        self.i += 1
+        self.col  = self.cmap(self.i)
+        
+    def reset(self):
+        self.i = 0
+        
+#%%
 class ezplot(object):
     """
     goal of testing:
     Plot.fig = plt.figure(num)
     Plot.add_subplot => fig.add_subplot => Plot.ax[ind] = ax_new
     """
     def __init__(self,**kwargs): #Initialise by assigning a figure, creating an axis, and selecting the axis
@@ -1263,15 +1401,15 @@
         DList = {}
         summary = ['\nSummary:']
         for ex in kw.ext:
             NList[ex] = [file for file in os.listdir(Dpath) if file.endswith(ex)]
             if kw.sort == 'numeric':
                 NList[ex] = natsort.natsorted(NList[ex], key=lambda y: y.lower())
                 cprint([ex, ' files were sorted numerically'],fg=['g','c'],ts='b')
-            DList[ex] = [Dpath+S_ESC+name for name in NList[ex]]
+            DList[ex] = [Dpath+name for name in NList[ex]]
             
         
             DSum = len(DList[ex])
             summary.append(str(DSum) + ' ' + ex + ' files')
                        
     else:
         NList = [file for file in os.listdir(Dpath)]
@@ -1910,14 +2048,15 @@
             if line.startswith('[') == True and line.endswith(']'):
                 topdict = line 
                 Raw[topdict] = {}
                 l2 = f.readline()
                 items = l2.split('\t')
                 for item in items:
                     Raw[topdict][item] = []
+                    
             else:
                 ld = line.split('\t')
                 
                 if topdict == '[Pre-Data]':
 
                     try:
                         Raw[topdict][ld[0]] = ld[1]
@@ -1926,33 +2065,46 @@
                             Raw[topdict][ld[0]] = None
                 else:
                     for num,item in enumerate(ld):
                         try:
                             Raw[topdict][items[num]].append(float(ld[num]))
                         except:
                             Raw[topdict][items[num]].append(ld[num])
-        
+            
+                
         if portF == True:
             keylist = []
             
             for key in Raw['[Pre-Data]'].keys():
                 if 'Comment' in key:
                     keylist.append(key)
+                    
             for key in keylist:
                 
                 cdata = Raw['[Pre-Data]'][key].split(' : ')
                 
                 cdstr = "".join(cdata).lower()
+                
                 if "device" in cdstr:
                     itlist = cdstr.split(' ; ')
                     Raw['[Pre-Data]'][itlist[0]] = itlist[1]
+                
+                if "light" in cdstr:
+                    itlist = cdstr.split(' ; ')
+                    if itlist[1].lower() in ['false','fal','off','none',None,'no']:
+                        itlist[1] = False
+                    
+                    elif itlist[1].lower() in ['true','tru','on','light','yes']:
+                        itlist[1] = True
+                        
+                    Raw['[Pre-Data]'][itlist[0]] = itlist[1]
+                    
                 else:
                     Raw['[Pre-Data]'][cdata[0]] = {'NW':None,'bias':False,'sweep':False,'current':False,'ground':False,'pos':None}
                 
-                print(cdata)
                 for item in cdata:
                     try:
                         itlist = item.split(' ; ')
                     except:
                         itlist = item
                         
                     if "NW" in item:   
@@ -1968,16 +2120,18 @@
                         Raw['[Pre-Data]'][cdata[0]][itlist[0]] = True
                         
                     if  'ground' in item:
                         Raw['[Pre-Data]'][cdata[0]][itlist[0]] = True
                         
                     if 'pos' in item:
                         Raw['[Pre-Data]'][cdata[0]][itlist[0]] = int(itlist[1])
-            
-                
+        Raw['info'] = {}
+        Raw['info']['filename'] = file.split('\\')[-1]
+        Raw['info']['path'] = file
+        
         return(Raw)
                 
    
    
 #%%
 def txtparse(**kwargs):
     kwargdict = {'file':'file','fn':'file','f':'file'}
```

### Comparing `DMU-0.0.4/DMU.egg-info/PKG-INFO` & `DMU-0.0.5/DMU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.4/LICENSE` & `DMU-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DMU-0.0.4/PKG-INFO` & `DMU-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.4/README.md` & `DMU-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `DMU-0.0.4/setup.py` & `DMU-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 
 setup(
     name="DMU",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     scripts=[TrgtScr],
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[module_filter(modules)+["docutils>=0.3"]],
```

