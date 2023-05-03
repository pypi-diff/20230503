# Comparing `tmp/bandplot-0.1.3.2-py3-none-any.whl.zip` & `tmp/bandplot-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9279 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       26 b- defN 23-May-02 18:19 bandplot/__init__.py
--rw-rw-r--  2.0 unx    27604 b- defN 23-May-02 18:19 bandplot/plots.py
--rw-rw-r--  2.0 unx     5809 b- defN 23-May-02 18:19 bandplot/readdata.py
--rw-rw-r--  2.0 unx    15274 b- defN 23-May-02 18:19 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2901 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      711 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/RECORD
-9 files, 52512 bytes uncompressed, 8055 bytes compressed:  84.7%
+Zip file size: 9430 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       24 b- defN 23-May-03 20:15 bandplot/__init__.py
+-rw-rw-r--  2.0 unx    28110 b- defN 23-May-03 20:15 bandplot/plots.py
+-rw-rw-r--  2.0 unx     5809 b- defN 23-May-03 20:15 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    15171 b- defN 23-May-03 20:15 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2899 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      701 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/RECORD
+9 files, 52901 bytes uncompressed, 8226 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.3.2.dist-info/METADATA
+Filename: bandplot-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.3.2.dist-info/WHEEL
+Filename: bandplot-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.3.2.dist-info/entry_points.txt
+Filename: bandplot-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.3.2.dist-info/top_level.txt
+Filename: bandplot-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.3.2.dist-info/RECORD
+Filename: bandplot-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.3.2"
+__version__ = "0.1.4"
```

## bandplot/plots.py

```diff
@@ -1,105 +1,100 @@
 import matplotlib.pyplot as plt
 
 # bandplot
 
-def Noneispin(EXPORT, figsize, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, location, color):
-    plt.figure(figsize=figsize)
-    if len(color) == 0:
-        color = ['r']
-
+def Noneispin(arr, bands, ticks, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     plt.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
-
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
-
     plt.xticks(ticks,labels)
-    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=location)
+    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xlim(arr[0], arr[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Ispin(EXPORT, figsize, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, location, color):
-    plt.figure(figsize=figsize)
-    if len(color) == 0:
-        color = ['r', 'k']
-    elif len(color) == 1:
+def Ispin(arr, bands, ticks, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
         color = [color[0], 'k']
-
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
-
     p_up = plt.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = plt.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'medium'})
+    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     plt.xlim(arr[0], arr[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.xticks(ticks,labels)
     plt.ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Dispin(EXPORT, figsize, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
+def Dispin(arr, bands, ticks, labels, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
-    if len(color) == 0:
-        color = ['r', 'k']
-    elif len(color) == 1:
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
         color = [color[0], 'k']
-
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
-
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'medium'})
-    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location)
+    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax1.set_xlim(arr[0], arr[-1])
-    ax1.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0], arr[-1])
-    ax2.set_ylim(vertical)
+    ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels[:-1]+[''])
     ax2.set_xticks(ticks,labels)
     ax1.set_ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def NoneispinWd(EXPORT, figsize, vertical, horizontal, arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=figsize)
+def NoneispinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
-    if len(color) == 0:
-        color = ['r']
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
 
     ax1.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = len(index_f)
     p_dos = []
     if num + 1 > len(color):
         color = color + [''] * (num + 1 - len(color))
 
@@ -115,54 +110,52 @@
             if fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=0.2)
         else:
             ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
 
-    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=location)
+    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.set_yticklabels([])
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=location, title="Density of states", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=fig_p.location, title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
 
     ax1.set_xlim(arr[0], arr[-1])
-    ax1.set_ylim(vertical)
-    ax2.set_xlim(horizontal)
-    ax2.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
+    ax2.set_xlim(fig_p.horizontal)
+    ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def IspinWd(EXPORT, figsize, vertical, horizontal, arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=figsize)
+def IspinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
-    if len(color) == 0:
-        color = ['r', 'k']
-    elif len(color) == 1:
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
         color = [color[0], 'k']
-
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
-
     p_up = ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = ax1.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'small'})
+    ax1.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'small'})
     num = len(index_f)
     p_dos = []
     if num + 2 > len(color):
         color = color + [''] * (num + 2 - len(color))
 
     if num + 2 > len(linestyle):
         linestyle = linestyle + ['-'] * (num + 2 - len(linestyle))
@@ -181,49 +174,47 @@
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
 
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=location, title="Density of states", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=fig_p.location, title="Density of states", title_fontproperties={'size':'small'})
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4, linestyle='-.', c='gray')
 
     ax1.set_xlim(arr[0], arr[-1])
-    ax1.set_ylim(vertical)
-    ax2.set_xlim(horizontal)
-    ax2.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
+    ax2.set_xlim(fig_p.horizontal)
+    ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def DispinWd(EXPORT, figsize, vertical, horizontal, arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.4*(1-width_ratios), 0.4*(1-width_ratios), width_ratios], figsize=figsize)
+def DispinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+    fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.4*(1-width_ratios), 0.4*(1-width_ratios), width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
-    if len(color) == 0:
-        color = ['r', 'k']
-    elif len(color) == 1:
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
         color = [color[0], 'k']
-
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
-
     if len(linewidth) == 1:
         linewidth = [linewidth[0], 0.8]
-
     ax1.plot(arr, bands[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, bands[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'small'})
-    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=location)
+    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'small'})
+    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'small'}, alignment='left', loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax3.minorticks_on()
     ax3.tick_params(axis='both', which='minor', color='gray')
     num = len(index_f)
     p_dos = []
     if num + 2 > len(color):
@@ -244,43 +235,46 @@
             p_dos = p_dos + ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
             if fill:
                 plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
 
     ax3.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax3.set_yticklabels([])
-    ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=location, title="Density of states", title_fontproperties={'size':'small'})
+    ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=fig_p.location, title="Density of states", title_fontproperties={'size':'small'})
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax3.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
             ax2.axvline(i,linewidth=0.4,linestyle='-.',c='gray')
 
     ax1.set_xlim(arr[0], arr[-1])
-    ax1.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(arr[0], arr[-1])
-    ax2.set_ylim(vertical)
-    ax3.set_xlim(horizontal)
-    ax3.set_ylim(vertical)
+    ax2.set_ylim(fig_p.vertical)
+    ax3.set_xlim(fig_p.horizontal)
+    ax3.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels[:-1]+[''])
     ax2.set_xticks(ticks,labels)
     ax3.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def pdosfiles(EXPORT, figsize, vertical, horizontal, darr, dele, fill, index_f, elements, linestyle, linewidth, legend, location, exchange, color):
-    plt.figure(figsize=figsize)
+def pdosfiles(darr, dele, fill, index_f, elements, legend, exchange, fig_p):
+    plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = len(index_f)
     p_dos = []
+    color = fig_p.color
+    linestyle = fig_p.linestyle
+    linewidth = fig_p.linewidth
     if num > len(color):
         color = color + [''] * (num - len(color))
 
     if num > len(linestyle):
         linestyle = linestyle + ['-'] * (num - len(linestyle))
 
     if num > len(linewidth):
@@ -294,54 +288,52 @@
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, color=color[i], alpha=0.2)
             else:
                 p_dos = p_dos + plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i])
                 if fill:
                     plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, alpha=0.2)
 
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
-        plt.xlim(vertical)
-        plt.ylim(horizontal)
+        plt.xlim(fig_p.vertical)
+        plt.ylim(fig_p.horizontal)
         plt.xlabel('Energy (eV)')
         plt.ylabel('Density of states, electrons/eV')
     else:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i], color=color[i])
                 if fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i], alpha=0.2)
             else:
                 p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i])
                 if fill:
                     plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
 
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
-        plt.ylim(vertical)
-        plt.xlim(horizontal)
+        plt.ylim(fig_p.vertical)
+        plt.xlim(fig_p.horizontal)
         plt.ylabel('Energy (eV)')
         plt.xlabel('Density of states, electrons/eV')
 
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=location, title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 # pbandplot
 
-def Broken(EXPORT,  figsize, vertical, arr, fre, ticks, labels, broken, height_ratio, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=figsize)
+def Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
-    if len(color) == 0:
-        color = ['r']
-
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.xlim(arr[0], arr[-1])
-    if vertical is None:
-        vertical = plt.ylim()
-
+    vertical = fig_p.vertical or plt.ylim()
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(vertical[0], broken[0])
     ax1.spines['bottom'].set_visible(False)
     ax2.spines['top'].set_visible(False)
     ax1.xaxis.set_ticks_position(position='none')
     ax1.tick_params(axis='y', which='minor', color='darkgray')
     ax1.tick_params(axis='y', labelsize='small', labelcolor='dimgray', labelrotation=-60)
@@ -349,49 +341,49 @@
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
-    ax2.legend(legend, frameon=False, prop={'size':'medium'}, loc=location)
+    ax2.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
-
-def Nobroken(EXPORT, figsize, vertical, arr, fre, ticks, labels, linestyle, linewidth, legend, location, color):
-    plt.figure(figsize=figsize)
-    if len(color) == 0:
-        color = ['r']
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
+def Nobroken(arr, fre, ticks, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     plt.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
-    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=location)
+    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xticks(ticks,labels)
     plt.xlim(arr[0], arr[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.ylabel('Frequency (THz)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def BrokenWd(EXPORT, figsize, vertical, horizontal, arr, fre, ticks, labels, broken, height_ratio, darr, dele, fill, elements, width_ratios, linestyle, linewidth, legend, location, color):
-    fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[height_ratio, 1-height_ratio], width_ratios=[1-width_ratios, width_ratios], figsize=figsize)
+def BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, fill, elements, width_ratios, legend, fig_p):
+    fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[height_ratio, 1-height_ratio], width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0, hspace=0.0)
-    if len(color) == 0:
-        color = ['r']
-
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax3.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
     p_dos = []
     if num + 1 > len(color):
         color = color + [''] * (num - len(color) + 1)
 
@@ -411,23 +403,22 @@
             ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fill:
                 plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
 
     ax1.set_xlim(arr[0], arr[-1])
     ax3.set_xlim(arr[0], arr[-1])
-    if vertical is None:
-        vertical = ax1.get_ylim()
+    vertical = fig_p.vertical or ax1.get_ylim()
 
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(broken[1], vertical[1])
     ax3.set_ylim(vertical[0], broken[0])
     ax4.set_ylim(vertical[0], broken[0])
-    ax2.set_xlim(horizontal)
-    ax4.set_xlim(horizontal)
+    ax2.set_xlim(fig_p.horizontal)
+    ax4.set_xlim(fig_p.horizontal)
     ax1.spines['bottom'].set_visible(False)
     ax2.spines['bottom'].set_visible(False)
     ax3.spines['top'].set_visible(False)
     ax4.spines['top'].set_visible(False)
     ax1.xaxis.set_ticks_position('none')
     ax2.xaxis.set_ticks_position('none')
     ax1.tick_params(axis='y', which='minor', color='darkgray')
@@ -449,38 +440,38 @@
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
-    ax3.legend(legend, frameon=False, prop={'size':'small'}, loc=location)
-    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=location, title="Phonon DOS", title_fontproperties={'size':'small'})
+    ax3.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
+    ax4.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=fig_p.location, title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax3.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax3.set_xticks(ticks,labels)
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax3.plot([0, 1], [0.98, 0.98], transform=ax3.transAxes, **kwargs)
     ax2.plot(1, 0.02, transform=ax2.transAxes, **kwargs)
     ax4.plot(1, 0.98, transform=ax4.transAxes, **kwargs)
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def NobrokenWd(EXPORT, figsize, vertical, horizontal, arr, fre, ticks, labels, darr, dele, fill, elements, width_ratios, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=figsize)
+def NobrokenWd(arr, fre, ticks, labels, darr, dele, fill, elements, width_ratios, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
-    if len(color) == 0:
-        color = ['r']
-
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
     p_dos = []
     if num + 1 > len(color):
         color = color + [''] * (num - len(color) + 1)
 
     if num + 1 > len(linestyle):
@@ -496,20 +487,19 @@
                 plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=0.2)
         else:
             p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             if fill:
                 plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
 
     ax1.set_xlim(arr[0], arr[-1])
-    if vertical is None:
-        vertical = ax1.get_ylim()
+    vertical = fig_p.vertical or ax1.get_ylim()
 
     ax1.set_ylim(vertical)
     ax2.set_ylim(vertical)
-    ax2.set_xlim(horizontal)
+    ax2.set_xlim(fig_p.horizontal)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='x', labelsize='small', labelcolor='dimgray', labelrotation=-90, pad=3)
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.set_yticklabels([])
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
@@ -517,31 +507,34 @@
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
-    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=location)
+    ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax2.axvline(linewidth=0.4,linestyle='-.',c='dimgray')
-    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=location, title="Phonon DOS", title_fontproperties={'size':'small'})
+    ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, alignment='left', loc=fig_p.location, title="Phonon DOS", title_fontproperties={'size':'small'})
     if len(ticks) > 2:
         ticks[0],ticks[-1] = arr[0],arr[-1]
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax1.set_xticks(ticks,labels)
     ax1.set_ylabel('Frequency (THz)')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def dosfile(EXPORT, figsize, vertical, horizontal, darr, dele, fill, elements, linestyle, linewidth, legend, location, exchange, color):
-    plt.figure(figsize=figsize)
+def dosfile(darr, dele, fill, elements, legend, exchange, fig_p):
+    plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = dele.shape[-1]
+    color = fig_p.color
+    linestyle = fig_p.linestyle
+    linewidth = fig_p.linewidth
     p_dos = []
     if num > len(color):
         color = color + [''] * (num - len(color))
 
     if num > len(linestyle):
         linestyle = linestyle + ['-'] * (num - len(linestyle))
 
@@ -555,42 +548,42 @@
                 if fill:
                     plt.fill_between(darr, dele[:,i], 0, color=color[i], alpha=0.2)
             else:
                 p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i])
                 if fill:
                     plt.fill_between(darr, dele[:,i], 0, alpha=0.2)
 
-        plt.xlim(vertical)
-        plt.ylim(horizontal)
+        plt.xlim(fig_p.vertical)
+        plt.ylim(fig_p.horizontal)
         plt.xlabel('Frequency (THz)')
         plt.ylabel('Phonon DOS')
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
     else:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
                 if fill:
                     plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=0.2)
             else:
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i])
                 if fill:
                     plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
 
-        plt.ylim(vertical)
-        plt.xlim(horizontal)
+        plt.ylim(fig_p.vertical)
+        plt.xlim(fig_p.horizontal)
         plt.ylabel('Frequency (THz)')
         plt.xlabel('Phonon DOS')
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
 
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     if num > len(elements):
         elements = elements + [''] * (num - len(elements))
     elif num < len(elements):
         if num == 1:
             elements = ['$tdos$']
         else:
             elements = elements[:num]
 
-    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## bandplot/wrapper.py

```diff
@@ -4,52 +4,70 @@
 from bandplot import __version__
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['ytick.minor.visible'] = True
 plt.rcParams["mathtext.fontset"] = 'cm'
 
+class cla_fig:
+    def __init__(self, **kwargs):
+        for key, value in kwargs.items():
+            if isinstance(value, str):
+                exec('self.%s = "%s"' %(key, value))
+            else:
+                exec('self.%s = %s' %(key, value))
+
 def main():
     parser = argparse.ArgumentParser(description='Plot the band structure or DOS from vaspkit result.',
                                      epilog='''
 Example:
 bandplot -i band.dat -o pband.png -l g m k g -d PDOS* -z
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-s', "--size",       type=int, nargs=2)
+    parser.add_argument('-s', "--size",       type=int,   nargs=2,  help='figure size: width, height')
     parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
-    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range")
-    parser.add_argument('-g', "--legend",     type=str, nargs=1,    help="legend labels")
-    parser.add_argument('-a', "--location",   type=str.lower,       default='best',
-                                                                    choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
-                                                                    help="arrange the legend location, default best")
-    parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', default=['-'],
-                                                                    help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
-    parser.add_argument('-c', "--color",      type=str,             nargs='+', default=[],
-                                                                    help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
-    parser.add_argument('-i', "--input",      type=str,             default="BAND.dat", help="plot figure from .dat file, default BAND.dat")
-    parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="plot figure filename, default BAND.png")
-    parser.add_argument('-j', "--klabels",    type=str,             default="KLABELS",  help="the filename of KLABELS")
+    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range, default: [-5.0, 5.0]")
+    parser.add_argument('-g', "--legend",     type=str,   nargs=1,  help="legend labels")
+    parser.add_argument('-a', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
+                                                                             'center left', 'center right', 'lower center', 'upper center', 'center'],
+                                                                    help="arrange the legend location, default: best", default='best')
+    parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
+                                                                                    "k, black; w, white", default=[])
+    parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
+                                                                                    default=[])
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
+    parser.add_argument('-i', "--input",      type=str,             help="plot figure from .dat file, default: BAND.dat", default="BAND.dat")
+    parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
+    parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
+    parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
-    parser.add_argument('-x', "--horizontal", type=float,           nargs=2, help="Density of states, electrons/eV range")
+    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-r', "--wratios",    type=float,           help='width ratio for DOS subplot')
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
-    parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
+    parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     dosfiles = [f for i in args.dos for f in glob.glob(i)]
+
+    color = []
+    for i in args.color:
+        j = i.split('*')
+        if len(j) == 2:
+            color = color + [j[0]] * int(j[1])
+        else:
+            color.append(i)
+
     linestyle = []
     for i in args.linestyle:
         if len(i) > 2 and i[0] == '(' and i[-1] == ')':
             linestyle.append(eval(i))
         elif len(i.split('*')) == 2:
             j = i.split('*')
             linestyle = linestyle + [j[0]] * int(j[1])
@@ -61,47 +79,34 @@
         if len(i.split('*')) == 2:
             j = i.split('*')
             linewidth = linewidth + [float(j[0])] * int(j[1])
         else:
             linewidth.append(float(i))
 
     plt.rcParams['font.family'] = '%s'%args.font
+
     pltname = os.path.split(os.getcwd())[-1]
     formula = ''
     if os.path.exists('POSCAR'):
         symbol, factor = readdata.symbols('POSCAR')
         for i in range(len(symbol)):
             if factor[i] > 1:
                 formula = formula + symbol[i]
                 for j in str(factor[i]):
                     formula = formula + '$_'+ j + '$'
             else:
                 formula = formula + symbol[i]
 
-    legend = args.legend
-    if not legend:
-        if formula:
-            legend = [formula]
-        else:
-            legend = [pltname]
-
-    color = []
-    for i in args.color:
-        j = i.split('*')
-        if len(j) == 2:
-            color = color + [j[0]] * int(j[1])
-        else:
-            color.append(i)
+    legend = args.legend or [formula] or [pltname]
 
+    fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
     if os.path.exists(args.input):
-        if not args.vertical:
-            vertical = [-5.0, 5.0]
-        else:
-            vertical = args.vertical
-
+        if not fig_p.vertical:
+            fig_p.vertical = [-5.0, 5.0]
         arr, bands, ispin = readdata.bands(args.input)
         ticks   = []
         klabels = []
         if os.path.exists(args.klabels):
             ticks, klabels = readdata.klabels(args.klabels)
 
         if len(labels) == 0:
@@ -110,86 +115,95 @@
         if len(ticks) > len(labels):
             labels = labels + [''] * (len(ticks) - len(labels))
         elif len(ticks) < len(labels):
             labels = labels[:len(ticks)]
 
         if not dosfiles:
             if ispin == "Noneispin":
-                plots.Noneispin(args.output, args.size, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, args.location, color)
+                plots.Noneispin(arr, bands, ticks, labels, legend, fig_p)
             elif ispin == "Ispin" and not args.divided:
-                plots.Ispin(args.output, args.size, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, args.location, color)
+                plots.Ispin(arr, bands, ticks, labels, legend, fig_p)
             elif ispin == "Ispin" and args.divided:
-                plots.Dispin(args.output, args.size, vertical, arr, bands, ticks, labels, linestyle, linewidth, legend, args.location, color)
+                plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
         else:
             darr, dele, s_elements = readdata.dos(args.dos)
             index_f, labels_elements = readdata.select(s_elements, args.partial)
             if not elements:
                 elements = labels_elements
             if not args.wratios:
                 if not args.divided:
                     width_ratios = 0.5
                 else:
                     width_ratios = 0.3
             else:
                 width_ratios = args.wratios
 
             if ispin == "Noneispin":
-                plots.NoneispinWd(args.output, args.size, vertical, args.horizontal, arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, linestyle, linewidth, legend, args.location, color)
+                plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
             elif ispin == "Ispin" and not args.divided:
-                plots.IspinWd(args.output, args.size, vertical, args.horizontal, arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, linestyle, linewidth, legend, args.location, color)
+                plots.IspinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
             elif ispin == "Ispin" and args.divided:
-                plots.DispinWd(args.output, args.size, vertical, args.horizontal, arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, linestyle, linewidth, legend, args.location, color)
+                plots.DispinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
 
     else:
         if dosfiles:
             darr, dele, s_elements = readdata.dos(dosfiles)
             index_f, labels_elements = readdata.select(s_elements, args.partial)
             if not elements:
                 elements = labels_elements
 
-            plots.pdosfiles(args.output, args.size, args.vertical, args.horizontal, darr, dele, args.fill, index_f, elements, linestyle, linewidth, legend, args.location, args.exchange, color)
+            plots.pdosfiles(darr, dele, args.fill, index_f, elements, legend, args.exchange, fig_p)
         else:
             print('No .dat file!')
 
 def pmain():
     parser = argparse.ArgumentParser(description='Plot the phonon band structure or DOS from phonopy results.',
                                      epilog='''
 Example:
 pbandplot -i band.dat -o pband.png -l g m k g -d projected_dos.dat -g "$\pi^2_4$" -e Si C O
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-s', "--size",       type=float,           nargs=2, help='figure size: width, height')
-    parser.add_argument('-b', "--broken",     type=float,           nargs=2, help='broken axis: start, end')
-    parser.add_argument('-r', "--hratios",    type=float,           default=0.2, help='height ratio for broken axis, default 0.2')
-    parser.add_argument('-y', "--vertical",   type=float,           nargs=2, help="frequency (THz) range")
-    parser.add_argument('-g', "--legend",     type=str,             nargs=1, help="legend labels")
-    parser.add_argument('-a', "--location",   type=str.lower,       default='best',
-                                                                    choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
-                                                                    help="arrange the legend location, default best")
-    parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', default=['-'],
-                                                                    help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
-    parser.add_argument('-c', "--color",      type=str,             nargs='+', default=[],
-                                                                    help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
-    parser.add_argument('-i', "--input",      type=str,             default="BAND.dat", help="plot figure from .dat file, default BAND.dat")
-    parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="plot figure filename, default BAND.png")
+    parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height')
+    parser.add_argument('-b', "--broken",     type=float, nargs=2,  help='broken axis: start, end')
+    parser.add_argument('-r', "--hratios",    type=float,           help='height ratio for broken axis, default: 0.2', default=0.2)
+    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="frequency (THz) range")
+    parser.add_argument('-g', "--legend",     type=str,   nargs=1,  help="legend labels")
+    parser.add_argument('-a', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
+                                                                             'center left', 'center right', 'lower center', 'upper center', 'center'],
+                                                                    help="arrange the legend location, default: best", default='best')
+    parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
+                                                                                    "k, black; w, white", default=[])
+    parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
+                                                                                    default=[])
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
+    parser.add_argument('-i', "--input",      type=str,             help="plot figure from .dat file, default: BAND.dat", default="BAND.dat")
+    parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
+    parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
-    parser.add_argument('-x', "--horizontal", type=float,           nargs=2, help="Phonon density of states range")
+    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-p', "--wratios",    type=float,           default=0.5, help='width ratio for DOS subplot, default 0.5')
+    parser.add_argument('-p', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
-    parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
+    parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
+    color  = []
+    for i in args.color:
+        j = i.split('*')
+        if len(j) == 2:
+            color = color + [j[0]] * int(j[1])
+        else:
+            color.append(i)
+
     linestyle = []
     for i in args.linestyle:
         if len(i) > 2 and i[0] == '(' and i[-1] == ')':
             linestyle.append(eval(i))
         elif len(i.split('*')) == 2:
             j = i.split('*')
             linestyle = linestyle + [j[0]] * int(j[1])
@@ -208,65 +222,56 @@
     pltname = os.path.split(os.getcwd())[-1]
     s_ele = []
     formula = ''
     if os.path.exists('POSCAR-unitcell'):
         symbol, factor = readdata.symbols('POSCAR-unitcell')
         for i in range(len(symbol)):
             if factor[i] > 1:
+                s_ele = s_ele + [symbol[i]] * factor[i]
                 formula = formula + symbol[i]
                 for j in str(factor[i]):
                     formula = formula + '$_'+ j + '$'
             else:
+                s_ele = s_ele + [symbol[i]]
                 formula = formula + symbol[i]
 
     if not elements and s_ele:
         elements = s_ele
 
-    legend = args.legend
-    if not legend:
-        if formula:
-            legend = [formula]
-        else:
-            legend = [pltname]
-
-    color  = []
-    for i in args.color:
-        j = i.split('*')
-        if len(j) == 2:
-            color = color + [j[0]] * int(j[1])
-        else:
-            color.append(i)
+    legend = args.legend or [formula] or [pltname]
 
     broken = args.broken
     height_ratio = args.hratios
     if height_ratio >= 1 or height_ratio <= 0:
         height_ratio = 0.2
 
     width_ratios = args.wratios
     if width_ratios >= 1 or width_ratios <= 0:
         width_ratios = 0.5
 
+    fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
     if os.path.exists(args.input):
         arr, fre, ticks = readdata.pbands(args.input)
         if len(ticks) > len(labels):
             labels = labels + [''] * (len(ticks) - len(labels))
         elif len(ticks) < len(labels):
             labels = labels[:len(ticks)]
         if args.dos is None:
             if args.broken is None:
-                plots.Nobroken(args.output, args.size, args.vertical, arr, fre, ticks, labels, linestyle, linewidth, legend, args.location, color)
+                plots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
             else:
-                plots.Broken(args.output, args.size, args.vertical, arr, fre, ticks, labels, broken, height_ratio, linestyle, linewidth, legend, args.location, color)
+                plots.Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p)
         elif os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
             if args.broken is None:
-                plots.NobrokenWd(args.output, args.size, args.vertical, args.horizontal, arr, fre, ticks, labels, darr, dele, args.fill, elements, width_ratios, linestyle, linewidth, legend, args.location, color)
+                plots.NobrokenWd(arr, fre, ticks, labels, darr, dele, args.fill, elements, width_ratios, legend, fig_p)
             else:
-                plots.BrokenWd(args.output, args.size, args.vertical, args.horizontal, arr, fre, ticks, labels, broken, height_ratio, darr, dele, args.fill, elements, width_ratios, linestyle, linewidth, legend, args.location, color)
+                plots.BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, args.fill, elements, width_ratios, legend, fig_p)
 
     else:
         if args.dos and os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
-            plots.dosfile(args.output, args.size, args.vertical, args.horizontal, darr, dele, args.fill, elements, linestyle, linewidth, legend, args.location, args.exchange, color)
+            plots.dosfile(darr, dele, args.fill, elements, legend, args.exchange, fig_p)
         else:
             print('No .dat file!')
```

## Comparing `bandplot-0.1.3.2.dist-info/METADATA` & `bandplot-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.3.2
+Version: 0.1.4
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

