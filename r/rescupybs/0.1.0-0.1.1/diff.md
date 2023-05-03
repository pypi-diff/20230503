# Comparing `tmp/rescupybs-0.1.0-py3-none-any.whl.zip` & `tmp/rescupybs-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9402 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       27 b- defN 23-May-01 05:23 rescupybs/__init__.py
--rw-rw-r--  2.0 unx    13813 b- defN 23-May-01 05:23 rescupybs/functions.py
--rw-rw-r--  2.0 unx     6786 b- defN 23-May-01 05:23 rescupybs/plots.py
--rw-rw-r--  2.0 unx    12499 b- defN 23-May-01 05:23 rescupybs/wrapper.py
--rwxrwxr-x  2.0 unx     1060 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2961 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       88 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      802 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/RECORD
-10 files, 38138 bytes uncompressed, 8036 bytes compressed:  78.9%
+Zip file size: 9526 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       27 b- defN 23-May-03 05:02 rescupybs/__init__.py
+-rw-rw-r--  2.0 unx    13813 b- defN 23-May-03 05:02 rescupybs/functions.py
+-rw-rw-r--  2.0 unx     7061 b- defN 23-May-03 05:02 rescupybs/plots.py
+-rw-rw-r--  2.0 unx    11652 b- defN 23-May-03 05:02 rescupybs/wrapper.py
+-rwxrwxr-x  2.0 unx     1060 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2961 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       88 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      802 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/RECORD
+10 files, 37566 bytes uncompressed, 8160 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/LICENSE
+Filename: rescupybs-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/METADATA
+Filename: rescupybs-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/WHEEL
+Filename: rescupybs-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/entry_points.txt
+Filename: rescupybs-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/top_level.txt
+Filename: rescupybs-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.1.0.dist-info/RECORD
+Filename: rescupybs-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## rescupybs/plots.py

```diff
@@ -1,109 +1,112 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
-def Nispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, location, color):
-    plt.figure(figsize=figsize)
-    if len(color) == 0:
-        color = ['r']
+def Nispin(eigenvalues, chpts, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     plt.plot(eigenvalues[0], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.xlim(chpts[0],chpts[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.tick_params(axis='y', which='minor', color='gray')
-    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=location)
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Mnispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, vbm_cbm, linestyle, linewidth):
-    plt.figure(figsize=figsize)
+def Mnispin(eigenvalues, chpts, labels, vbm_cbm, fig_p):
+    plt.figure(figsize=fig_p.size)
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
     VBM, CBM = vbm_cbm[0]
     org = plt.plot(eigenvalues[0], linewidth=linewidth[0], linestyle=linestyle[0])
     fig = plt.plot(eigenvalues[0,:,VBM-5:CBM+6], linewidth=linewidth[0]*1.5, linestyle=(0, (3, 1)))
     plt.xlim(chpts[0],chpts[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.tick_params(axis='y', which='minor', color='gray')
     plt.legend(fig, range(VBM-5, CBM+6), frameon=False, prop={'size':'medium'}, loc='center right')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Ispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, location, color):
-    plt.figure(figsize=figsize)
-    if len(color) == 0:
-        color = ['r', 'k']
-    elif len(color) == 1:
+def Ispin(eigenvalues, chpts, labels, legend, fig_p):
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
     p_up = plt.plot(eigenvalues[0], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     p_do = plt.plot(eigenvalues[1], color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     plt.xlim(chpts[0],chpts[-1])
-    plt.ylim(vertical)
+    plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.tick_params(axis='y', which='minor', color='gray')
-    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'medium'})
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.legend([p_up[0], p_do[0]], ['up', 'down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Dispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, location, color):
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
+def Dispin(eigenvalues, chpts, labels, legend, fig_p):
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
     ax1.plot(eigenvalues[0], color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax2.plot(eigenvalues[1], color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location, title=legend[0], title_fontproperties={'size':'medium'})
-    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=location)
+    ax1.legend(['up'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    ax2.legend(['down'], frameon=False, prop={'style':'italic', 'size':'medium'}, alignment='left', loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax1.set_xlim(chpts[0],chpts[-1])
-    ax1.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(chpts[0],chpts[-1])
-    ax2.set_ylim(vertical)
+    ax2.set_ylim(fig_p.vertical)
     ax1.set_ylabel('Energy (eV)')
     ax1.set_xticks(chpts,labels[:-1]+[''])
     ax2.set_xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def Mispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, vbm_cbm, linestyle, linewidth):
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
+def Mispin(eigenvalues, chpts, labels, vbm_cbm, fig_p):
+    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=fig_p.size)
+    linestyle = fig_p.linestyle or ['-', '-']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
     fig.subplots_adjust(wspace=0.0)
     if len(linestyle) == 1:
         linestyle = [linestyle[0], linestyle[0]]
     if len(linewidth) == 1:
         linewidth = [linewidth[0], linewidth[0]]
     VBM_up, CBM_up = vbm_cbm[0]
     VBM_do, CBM_do = vbm_cbm[1]
@@ -115,20 +118,20 @@
     ax2.legend(p_do_f, range(VBM_do-5, CBM_do+6), frameon=False, prop={'size':'medium'}, alignment='left', title="down", title_fontproperties={'style':'italic', 'size':'medium'}, loc='center right')
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax1.set_xlim(chpts[0],chpts[-1])
-    ax1.set_ylim(vertical)
+    ax1.set_ylim(fig_p.vertical)
     ax2.set_xlim(chpts[0],chpts[-1])
-    ax2.set_ylim(vertical)
+    ax2.set_ylim(fig_p.vertical)
     ax1.set_ylabel('Energy (eV)')
     ax1.set_xticks(chpts,labels[:-1]+[''])
     ax2.set_xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
-    plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
```

## rescupybs/wrapper.py

```diff
@@ -6,14 +6,22 @@
 from rescupybs import __version__
 
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
     parser = argparse.ArgumentParser(description='Plot the band structure from rescuplus calculation result *.json or *.dat file.',
                                      epilog='''
 Example:
 rescubs -y -0.5 0.5 -b
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
@@ -21,23 +29,24 @@
     parser.add_argument('-s', "--size",       type=float, nargs=2,   help='figure size: width, height')
     parser.add_argument('-b', "--divided",    action='store_true',   help="plot the up and down spin in divided subplot")
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,   help="vertical axis")
     parser.add_argument('-g', "--legend",     type=str,   nargs=1,   help="legend labels")
     parser.add_argument('-a', "--location",   type=str.lower,        default='best',
                                                                      choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                      help="arrange the legend location, default best")
-    parser.add_argument('-k', "--linestyle",  type=str, nargs='+',   default=['-'],
+    parser.add_argument('-k', "--linestyle",  type=str, nargs='+',   default=[],
                                                                      help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-w', "--linewidth",  type=str, nargs='+',   default=['0.8'], help="linewidth, default 0.8")
+    parser.add_argument('-w', "--linewidth",  type=str, nargs='+',   default=[], help="linewidth, default 0.8")
     parser.add_argument('-c', "--color",      type=str,              nargs='+', default=[],
-                                                                     help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
+                                                                     help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
     parser.add_argument('-m', "--modify",     type=int, nargs=2,     help='modify the bands overlap, the up or nonispin bands to exchange values')
     parser.add_argument('-n', "--nbands",     type=int, nargs=2,     help='the down bands to exchange values')
     parser.add_argument('-i', "--input",      type=str,              nargs='+', default=[], help="plot figure from .json or .dat file")
-    parser.add_argument('-o', "--output",     type=str,              default="BAND.png", help="plot figure filename")
+    parser.add_argument('-o', "--output",     type=str,              default="BAND.png", help="filename of the figure, default: BAND.png")
+    parser.add_argument('-q', "--dpi",        type=int,              default=500, help="dpi of the figure, default: 500")
     parser.add_argument('-l', "--labels",     type=str.upper,        nargs='+', default=[], help='labels for high-symmetry points')
     parser.add_argument('-f', "--font",       type=str,              default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels_f = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     linestyle = []
@@ -62,118 +71,107 @@
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
             color = color + [j[0]] * int(j[1])
         else:
             color.append(i)
 
-    if not args.vertical:
-        vertical = [-5.0, 5.0]
-    else:
-        vertical = args.vertical
+    vertical = args.vertical or [-5.0, 5.0]
 
     plt.rcParams['font.family'] = '%s'%args.font
+
     pltname = os.path.split(os.getcwd())[-1]
-    if not args.input:
-        input = ['nano_bs_out.json']
-        if not os.path.exists(input[0]):
-            raise Exception("The input file does not exist.")
-    else:
-        input = [f for i in args.input for f in glob.glob(i)]
-        input = [os.path.join(i,'nano_bs_out.json') if os.path.isdir(i) else i for i in input]
-        input = [i for i in input if os.path.exists(i)]
-        if not input:
-            raise Exception("The input file does not exist.")
 
+    input = args.input or ['nano_bs_out.json']
+    input = [f for i in input for f in glob.glob(i)]
+    input = [os.path.join(i,'nano_bs_out.json') if os.path.isdir(i) else i for i in input]
+    input = [i for i in input if os.path.exists(i)]
+    if not input:
+        raise Exception("The input file does not exist.")
+
+    fig_p = cla_fig(output=args.output, size=args.size, vertical=vertical,
+                    linestyle=linestyle, linewidth=linewidth, location=args.location, color=color, dpi=args.dpi)
     if len(input) == 1:
         if input[0].lower().endswith('.json'):
             if 'bs' in input[0].split('_'):
                 bs_file = input[0]
                 eigenvalues, chpts, labels = functions.bs_json_read(bs_file)
                 if labels_f:
                     labels = labels_f
-                legend = args.legend
-                if not legend:
-                    legend = [pltname]
+                legend = args.legend or [pltname]
                 if len(chpts) > len(labels):
                     labels = labels + [''] * (len(chpts) - len(labels))
                 elif len(chpts) < len(labels):
                     labels = labels[:len(chpts)]
                 if len(eigenvalues) == 1:
-                    plots.Nispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and not args.divided:
-                    plots.Ispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Ispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and args.divided:
-                    plots.Dispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Dispin(eigenvalues, chpts, labels, legend, fig_p)
 
         elif input[0].lower().endswith('.dat'):
             eigenvalues = functions.bs_dat_read(input)
             chpts, labels, vbm_cbm = functions.labels_read("LABELS")
             if labels_f:
                 labels = labels_f
-            legend = args.legend
-            if not legend:
-                legend = [pltname]
+            legend = args.legend or [pltname]
             if len(chpts) > len(labels):
                 labels = labels + [''] * (len(chpts) - len(labels))
             elif len(chpts) < len(labels):
                 labels = labels[:len(chpts)]
             if args.modify:
                 if args.modify[0] != args.modify[1]:
                     functions.exchange(eigenvalues[0,:,args.modify[0]], eigenvalues[0,:,args.modify[1]])
                     np.savetxt(input[0], eigenvalues[0])
-                plots.Mnispin(args.output, args.size, vertical, eigenvalues, chpts, labels, vbm_cbm, linestyle, linewidth)
+                plots.Mnispin(eigenvalues, chpts, labels, vbm_cbm, fig_p)
             else:
-                plots.Nispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
 
     else:
         Extension = [f.rsplit('.', 1)[-1].lower() for f in input]
         if all(x == Extension[0] for x in Extension):
             if len(input) == 2 and Extension[0] == 'dat':
                 eigenvalues = functions.bs_dat_read(input)
                 chpts, labels, vbm_cbm = functions.labels_read("LABELS")
                 if labels_f:
                     labels = labels_f
-                legend = args.legend
-                if not legend:
-                    legend = [pltname]
+                legend = args.legend or [pltname]
                 if len(chpts) > len(labels):
                     labels = labels + [''] * (len(chpts) - len(labels))
                 elif len(chpts) < len(labels):
                     labels = labels[:len(chpts)]
                 if args.modify or args.nbands:
                     if args.modify and args.modify[0] != args.modify[1]:
                         functions.exchange(eigenvalues[0,:,args.modify[0]], eigenvalues[0,:,args.modify[1]])
                         np.savetxt(input[0], eigenvalues[0])
                     if args.nbands and args.nbands[0] != args.nbands[1]:
                         functions.exchange(eigenvalues[0,:,args.nbands[0]], eigenvalues[0,:,args.nbands[1]])
                         np.savetxt(input[1], eigenvalues[1])
-                    plots.Mispin(args.output, args.size, vertical, eigenvalues, chpts, labels, vbm_cbm, linestyle, linewidth)
+                    plots.Mispin(eigenvalues, chpts, labels, vbm_cbm, fig_p)
                 else:
                     if len(eigenvalues) == 2 and not args.divided:
-                        plots.Ispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                        plots.Ispin(eigenvalues, chpts, labels, legend, fig_p)
                     elif len(eigenvalues) == 2 and args.divided:
-                        plots.Dispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                        plots.Dispin(eigenvalues, chpts, labels, legend, fig_p)
             elif Extension[0] == 'json' and all('bs' in f.split('_') for f in input):
                 eigenvalues, chpts, labels = functions.bs_json_read_all(input)
                 if labels_f:
                     labels = labels_f
-                legend = args.legend
-                if not legend:
-                    legend = [pltname]
+                legend = args.legend or [pltname]
                 if len(chpts) > len(labels):
                     labels = labels + [''] * (len(chpts) - len(labels))
                 elif len(chpts) < len(labels):
                     labels = labels[:len(chpts)]
                 if len(eigenvalues) == 1:
-                    plots.Nispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and not args.divided:
-                    plots.Ispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Ispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and args.divided:
-                    plots.Dispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
+                    plots.Dispin(eigenvalues, chpts, labels, legend, fig_p)
         else:
             raise Exception("The input files mismatch.")
 
 def surface():
     parser = argparse.ArgumentParser(description='Export the wavefunction isosurface for VESTA from rescuplus calculation result *.json and *.h5 files.',
                                      epilog='''
 Example:
@@ -185,30 +183,24 @@
     parser.add_argument('-o', "--output",  type=str,         help="wavefunction isosurface for VESTA format")
     parser.add_argument('-k', "--kpt",     type=int,         nargs='+', default=[0], help="The kpoint in wavefunctions")
     parser.add_argument('-b', "--band",    type=int,         nargs='+', default=[0], help="The band in wavefunctions")
     parser.add_argument('-s', "--spin",    type=int,         default=1, help="The up or down spin in wavefunctions")
 
     args = parser.parse_args()
 
-    if args.kpt[0] < 0:
+    if args.kpt[0] < 0 or args.band[0] < 0:
         raise Exception("Illegal input of kpt.")
-    if args.band[0] < 0:
-        raise Exception("Illegal input of band.")
 
-    if not args.input:
-        input = ['nano_wvf_out']
-        if not os.path.exists(input[0]+'.json') and not os.path.exists(input[0]+'.h5'):
-            raise Exception("The input file does not exist.")
-    else:
-        input = [f.rsplit('_in',1)[0]+'_out.json' if f.rsplit('.',1)[0].endswith('in') else f for i in args.input for f in glob.glob(i)]
-        input = [os.path.join(i,'nano_wvf_out.json') if os.path.isdir(i) else i for i in input]
-        input = [i.rsplit('.',1)[0] for i in input]
-        input = [i for i in input if os.path.exists(i+'.json') and os.path.exists(i+'.h5')]
-        if not input:
-            raise Exception("The input file does not exist.")
+    input = args.input or ['nano_wvf_out.json']
+    input = [f.rsplit('_in',1)[0]+'_out.json' if f.rsplit('.',1)[0].endswith('in') else f for i in input for f in glob.glob(i)]
+    input = [os.path.join(i,'nano_wvf_out.json') if os.path.isdir(i) else i for i in input]
+    input = [i.rsplit('.',1)[0] for i in input]
+    input = [i for i in input if os.path.exists(i+'.json') and os.path.exists(i+'.h5')]
+    if not input:
+        raise Exception("The input file does not exist.")
 
     if len(input) == 1:
         if 'wvf' in input[0].split('_'):
             functions.isosurfaces_wf(input[0], args.output, args.kpt, args.band, args.spin)
     else:
         if all('wvf' in f.split('_') for f in input):
             for i in range(len(input)):
```

## Comparing `rescupybs-0.1.0.dist-info/LICENSE` & `rescupybs-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rescupybs-0.1.0.dist-info/METADATA` & `rescupybs-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Band structure plot from rescuplus json file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT rescuplus band plot
 Platform: Unix
```

## Comparing `rescupybs-0.1.0.dist-info/RECORD` & `rescupybs-0.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-rescupybs/__init__.py,sha256=YmuAVovZuFz7KJoBCPmYu2fXceq6f2IPaWT9sayY_8w,27
+rescupybs/__init__.py,sha256=GThDTBxUYSx7Tbtuwxo2HyiVDw6EMvBnKJkJof2YsWQ,27
 rescupybs/functions.py,sha256=ywVvQ8WkiNb156SG4pUV1aGDQkYQlgBIFKWAkPgbNJw,13813
-rescupybs/plots.py,sha256=5_7__zep7lgbxNqw-UZ_Nm2h4uSbtjCbeqB9g3FHLoM,6786
-rescupybs/wrapper.py,sha256=v-aFTDSI4eO1meBJkME6y4HsfGpHo1yg_e7mR27aI98,12499
-rescupybs-0.1.0.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
-rescupybs-0.1.0.dist-info/METADATA,sha256=auaVArPyq42bNYOgbQYYlzD6yN9PQlJ8cUbv4_c8gv4,2961
-rescupybs-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.1.0.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
-rescupybs-0.1.0.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.1.0.dist-info/RECORD,,
+rescupybs/plots.py,sha256=Ql2VasG6SzXOgKRE43ROwiu15P8sPQHDukKwG1fuyUA,7061
+rescupybs/wrapper.py,sha256=mgGPiJKWW9U9Akvr-LV5-IFWf2fEopfO9d0IgxK7WSA,11652
+rescupybs-0.1.1.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
+rescupybs-0.1.1.dist-info/METADATA,sha256=L8iuuO6fZYDCNkIz6XtdjZyV0ygyackkBZn71WHveu8,2961
+rescupybs-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.1.1.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
+rescupybs-0.1.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.1.1.dist-info/RECORD,,
```

