# Comparing `tmp/ipam_pacman-1.0.0.tar.gz` & `tmp/ipam_pacman-1.0.0rc1.tar.gz`

## Comparing `ipam_pacman-1.0.0.tar` & `ipam_pacman-1.0.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/PACsettings.ini
--rw-r--r--   0        0        0    18318 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/PacMan.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/__init__.py
--rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/IRHM.py
--rw-r--r--   0        0        0   246110 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/PacMAN_LOGO_TRP.ico
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/PycroCom.py
--rw-r--r--   0        0        0    20888 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/SCM.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/StageCommunicator_Template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/__init__.py
--rw-r--r--   0        0        0    54410 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/pacmangui.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/sliceViewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/utils/__init__.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/utils/utils.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/PerPosScript.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pacman/managers/StartPosScript.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/.gitignore
--rw-r--r--   0        0        0    33021 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/LICENSE
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/README.md
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/PACsettings.ini
+-rw-r--r--   0        0        0    17543 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/PacMan.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/__init__.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/IRHM.py
+-rw-r--r--   0        0        0   246110 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/PacMAN_LOGO_TRP.ico
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/PycroCom.py
+-rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/SCM.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/StageCommunicator_Template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/__init__.py
+-rw-r--r--   0        0        0    54593 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/pacmangui.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/sliceViewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/utils/__init__.py
+-rw-r--r--   0        0        0    12605 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/utils/utils.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/PerPosScript.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pacman/managers/StartPosScript.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/.gitignore
+-rw-r--r--   0        0        0    33021 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 ipam_pacman-1.0.0rc1/PKG-INFO
```

### Comparing `ipam_pacman-1.0.0/pacman/PacMan.py` & `ipam_pacman-1.0.0rc1/pacman/PacMan.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,25 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 Contact: olle.ponten@gmail.com
 
 """
 
 from dataclasses import dataclass
 
-from utils import utils
-from managers import SCM
-from managers import IRHM
-from managers import pacmangui as pacmangui
+from .managers import SCM
+from .managers import IRHM
+from .managers import pacmangui as pacmangui
+from .utils import utils
 import tifffile
 import skimage
 import skimage.io
 import os, time, sys
 import matplotlib
 matplotlib.use("Qt5Agg")
 import numpy as np
-import psutil
-
 global gui_ptr
 
 global DEBUG
 DEBUG = False
 
 from enum import Enum
 class External_Components(Enum):
@@ -66,33 +64,18 @@
     def __init__(self, with_gui = False):           
         try:
             self.IPam = IRHM.AIPam()
         except ConnectionError as e:
             print("Error when starting IRHM. Double check ImagingWin is running. Aborting")
             cleanup()
             sys.exit()
-            
-        self.settings = utils.read_ini_file("PACSettings.ini")
-        if(self.settings['General']['imagingwininstalldir'] == "Default"):
-            processes = dict()
-            for proc in psutil.process_iter():
-                try:
-                    # Get process name & pid from process object.
-                    processName = proc.name()
-                    processID = proc.pid
-                    processes[processName] = processID
-                except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
-                    pass
-            if('ImagingWin.exe' in processes.keys()):
-                pid = processes['ImagingWin.exe']
-                self.settings['General']['imagingwininstalldir'] = psutil.Process(pid).exe()
-            utils.logmsg(f"Default install directory extracted from current exe: {self.settings['General']['imagingwininstalldir']}")
-        self.output_directory = self.settings['General']['outputdir']
+        self.settings = utils.read_ini_file("PACSettings")
+        self.output_directory = self.settings['General']['OutputDir']
         try: 
-            if(self.settings['General']['scmserial']):   
+            if(self.settings['General']['SCMSerial']):   
                 self.StageCom = SCM.SC()
             else:
                 self.StageCom = PycroCom.PCMCom()
         except:
             print("Cannot connect to StageManager, assuming debugging. SCM disabled.")
             DEBUG = True
             self.StageCom = 0
@@ -323,18 +306,18 @@
             DESCRIPTION.
 
         """
         #itr_imgs = []
         output_dir = self.output_directory
         lbls = self.StageCom.get_pos_lbls()
         for pos,data in enumerate(self.StageCom.Pos_List):
-            pos_fp = self.settings['General']['imagingwininstalldir'] + '\\Data_RGB\\' + self.IPam.Base_Filename.format(Exp = exp_name, lbl = lbls[pos]) + '.tif'
+            pos_fp = self.settings['General']['ImagingWinInstallDir'] + '\\Data_RGB\\' + self.IPam.Base_Filename.format(Exp = exp_name, lbl = lbls[pos]) + '.tif'
             #pos_coll = skimage.io.imread_collection(pos_fp,conserve_memory = True, plugin = 'tifffile')
             pos_img = skimage.io.imread(pos_fp,plugin = 'tifffile')
-            itr_fp = self.settings['General']['imagingwininstalldir'] + '\\Data_RGB\\' + self.IPam.Base_Filename.format(Exp = exp_name, lbl = lbls[pos]) + f"_T{itr_no}*.tif"
+            itr_fp = self.settings['General']['ImagingWinInstallDir'] + '\\Data_RGB\\' + self.IPam.Base_Filename.format(Exp = exp_name, lbl = lbls[pos]) + f"_T{itr_no}*.tif"
             itr_coll = skimage.io.imread_collection(itr_fp, conserve_memory = True, plugin = 'tifffile')
             pos_itr_imgs = itr_coll.concatenate()
             f_img = np.concatenate((pos_img, pos_itr_imgs), axis = 0)
             (PosX,PosY,PosZ) = data[0]
             #XPos_Tag = ["XPosition", 'I', 1, PosX]
             #YPos_Tag = ["YPosition", 'I', 1, PosY]
             tifffile.imwrite(pos_fp,f_img,imagej = True, resolution = (0.4,0.4),  metadata = {'unit': 'um',"XPosition":PosX, "YPosition":PosY})
@@ -443,11 +426,19 @@
             processes[processName] = processID
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
     if('ImagingWin.exe' in processes.keys()):
         os.kill(processes['ImagingWin.exe'],9)
     cv2.destroyAllWindows() 
 
+def get_file_path():
+    return output_dir
+
+
+
+    
+    
 if __name__ == '__main__':
-    PCM = PacMan(True)
-    #pacmangui.start(PCM)
+    from managers import pacmangui
+    pacmangui.start()
+    PCM = PacMan.PacMan()
     print("Exited")
```

### Comparing `ipam_pacman-1.0.0/pacman/managers/IRHM.py` & `ipam_pacman-1.0.0rc1/pacman/managers/IRHM.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 """
 
 from comtypes import client as ctClient 
 import comtypes
 import ctypes
 import collections
 import psutil
-import os
 
 DEBUG = False
 
 Command = collections.namedtuple('Command', ['cmd','param'])
 
 File_Specified_Commands = ["Export to Tiff File = ", "Save PIM File = ", "Save Tiff Image = ", "Save Jpeg Image = "] 
 Base_Filename = ''
@@ -200,16 +199,14 @@
                 if(strout):
                     ret.append(printstr)
             if(strout):
                 return ret
             
         def load_acquisition_script(self, fn = 'PerPosScript.txt'):
             self.Command_Queue.clear()
-            if("/" not in fn):
-                fn = os.path.join(os.path.split(__file__)[0],fn)
             with open(fn) as script_file:
                 for line in script_file:
                     read_cmd = line.split(",")
                     #If the parameter specified is a file name, we format this file name
                     #so that we get correct filenames that correspond to our repitition
                     self.add_command_to_queue(read_cmd[0], read_cmd[1].rstrip())
                     if(read_cmd[0] in str(File_Specified_Commands)):
@@ -217,16 +214,14 @@
                         
         def clear_queues(self):
             self.Command_Queue.clear()
             self.Start_Command_Queue.clear()
             
         def load_start_script(self, fn = 'StartPosScript.txt'):
             self.Start_Command_Queue.clear()
-            if("/" not in fn):
-                fn = os.path.join(os.path.split(__file__)[0],fn)
             with open(fn) as script_file:
                 for line in script_file:
                     read_cmd = line.split(",")
                     self.Start_Command_Queue.append(Command(read_cmd[0], read_cmd[1].rstrip()))
                     if(read_cmd[0] in str(File_Specified_Commands)):
                         self.Base_Filename = read_cmd[1].rstrip()
```

### Comparing `ipam_pacman-1.0.0/pacman/managers/PacMAN_LOGO_TRP.ico` & `ipam_pacman-1.0.0rc1/pacman/managers/PacMAN_LOGO_TRP.ico`

 * *Files identical despite different names*

### Comparing `ipam_pacman-1.0.0/pacman/managers/PycroCom.py` & `ipam_pacman-1.0.0rc1/pacman/managers/PycroCom.py`

 * *Files identical despite different names*

### Comparing `ipam_pacman-1.0.0/pacman/managers/SCM.py` & `ipam_pacman-1.0.0rc1/pacman/managers/SCM.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 
 import time
 import serial
 import sys
 import re
 
 #local imports
-if __name__ == '__main__':
-    from utils import utils
-else:    
-    from utils import utils
+from ..utils import utils
 
 global ser,COMPORT, resolution
 resolution = 0.1
 
 
 class SC:
```

### Comparing `ipam_pacman-1.0.0/pacman/managers/StageCommunicator_Template.py` & `ipam_pacman-1.0.0rc1/pacman/managers/StageCommunicator_Template.py`

 * *Files identical despite different names*

### Comparing `ipam_pacman-1.0.0/pacman/managers/pacmangui.py` & `ipam_pacman-1.0.0rc1/pacman/managers/pacmangui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 #! /usr/bin/env python
 #  -*- coding: utf-8 -*-
 #
 # GUI module generated by PAGE version 6.0.1
 #  in conjunction with Tcl version 8.6
 #    Mar 04, 2021 10:26:47 AM CET  platform: Windows NT
 
-
-import sys
-import os
-
 try:
     import Tkinter as tk
 except ImportError:
     import tkinter as tk
 
 try:
     import ttk
     py3 = False
 except ImportError:
     import tkinter.ttk as ttk
     py3 = True
+    
 import tkinter.filedialog
-import tkinter.messagebox
-
-
+import sys
+import os
 if __name__ == '__main__':
     import SCM
 else:
     from . import SCM
-import utils
-
-
-
+import tkinter.messagebox
 global ImagingWinPath
 ImagingWinPath = "C:/ImagingPamGigE/Data_RGB/"
 global int_var, rep_var, temp_sep_var, pos_var
 global val, root, top, PacManHndl
 
 
 def set_tk_var():
     global int_var, rep_var, temp_sep_var, pos_var
     int_var = tk.IntVar()
     rep_var = tk.IntVar()
     pos_var = tk.StringVar()
     temp_sep_var = tk.IntVar()
 
 def start(P_ptr = None):
-    global ImagingWinPath
     if(P_ptr is None):
         path = os.getcwd()+"..\\"
         sys.path.append(path)
         import PacMan
         PCM = PacMan.PacMan()
     else:
         PCM = P_ptr 
-    ImagingWinPath = PCM.settings['General']['imagingwininstalldir']
     vp_start_gui(PCM)
     PCM.IPam.load_acquisition_script()
     PCM.IPam.load_start_script()
     root.mainloop()  
 
 def debug_start():
     vp_start_gui(1)
@@ -80,15 +71,15 @@
 def load_AF():
     try:
         Threshold = float(window.dZMin_ent.get())
         Strength = float(window.AFStrength_ent.get())
         minCirc = float(window.minCirc_ent.get())
         minInert = float(window.minInert_ent.get())
         sizes = window.size_ent.get().split(',')
-        utils.logmsg(f"Autofocus parameters changed to: {[Threshold,Strength,minCirc,minInert,int(sizes[0]),int(sizes[1])]}")
+        PacMan.logmsg(f"Autofocus parameters changed to: {[Threshold,Strength,minCirc,minInert,int(sizes[0]),int(sizes[1])]}")
     except:
         print("One of the autofocus value was not correctly formmated")
     
 def save_pos_list():
     print("Save pos list pressed")
     
     try:
@@ -134,32 +125,32 @@
         exception_handler(e)
 
 def send_serial_command():
    msg = window.ser_com_ent.get()
    window.ser_com_var.set("")
    #w.ser_com_ent.set("")
    if("log:" in msg[0:5]):
-       utils.logmsg(msg)
+       PacMan.logmsg(msg)
    elif("Queue:" in msg[0:6]):
        timer_cmd = msg[6:]
        try:
-           utils.logmsg(f"Queing following command:{timer_cmd}")
+           PacMan.logmsg(f"Queing following command:{timer_cmd}")
            PacManHndl.queue_command(timer_cmd)
        except Exception as e:
            exception_handler(e)
    elif("IPAM:" in msg[0:6]):
        print(f"Sending Manual IPAM Command:{msg[5:]}")
        IPAM_Cmd = msg[5:].split(",")
 
        PacManHndl.IPam.send_Command(IPAM_Cmd[0],IPAM_Cmd[1])
    elif("Prior:" in msg[0:7]):      
        prior_cmd = msg[6:]
        print(f"Sending Manual Serial Command:{prior_cmd}")
        try:
-           utils.logmsg(PacManHndl.StageCom.msg_resp(prior_cmd))
+           PacMan.logmsg(PacManHndl.StageCom.msg_resp(prior_cmd))
        except Exception as e:
            exception_handler(e)
 
 def update_pos_list():
     if(PacManHndl.StageCom.get_pos_list_length()>0):
         try:
             window.pos_list.delete(0,tk.END)
@@ -277,15 +268,15 @@
         top.configure(highlightbackground="#d9d9d9")
         top.configure(highlightcolor="black")
 
         self.tabControl = ttk.Notebook(top)
         self.main_tab = ttk.Frame(self.tabControl)
         self.tabControl.add(self.main_tab,text="Main")
         self.autofocus_tab = ttk.Frame(self.tabControl)
-        #self.tabControl.add(self.autofocus_tab, text = "Autofocus",state="disabled")
+        self.tabControl.add(self.autofocus_tab, text = "Autofocus",state="disabled")
         self.positions_tab = ttk.Frame(self.tabControl)
         self.tabControl.add(self.positions_tab, text = "Positions")
         
         #Style for all frames
         s = ttk.Style(top)
         s.configure('TFrame', background="#d9d9d9", highlightbackground="#d9d9d9",highlightcolor="black")
         
@@ -318,14 +309,19 @@
         self.pos_list = tk.Listbox(self.positions_tab, selectmode='SINGLE')
         self.pos_list.place(relx = baserelx, rely = 0.08, relheight = 0.6, width = 300)
         
         self.pos_lbl = tk.Label(self.positions_tab, anchor = 'w')
         self.pos_lbl.place(relx=baserelx, rely=0, height=20, width=300)
         self.pos_lbl.configure(bg="#f9f9f9")
         self.pos_lbl.configure(fg="black")
+        # self.pos_lbl.configure(background="#d9d9d9")
+        # self.pos_lbl.configure(disabledforeground="#a3a3a3")
+        # self.pos_lbl.configure(foreground="#000000")
+        # self.pos_lbl.configure(highlightbackground="#d9d9d9")
+        # self.pos_lbl.configure(highlightcolor="black")
         self.pos_lbl.configure(text ="X:      Y:      Z:      Name: ")
         
         self.go_to_btn = tk.Button(self.positions_tab)
         self.go_to_btn.place(relx=0.25, rely=0.6, height=24, width=80)
         self.go_to_btn.configure(activebackground="#ececec")
         self.go_to_btn.configure(activeforeground="#000000")
         self.go_to_btn.configure(background="#d9d9d9")
```

### Comparing `ipam_pacman-1.0.0/pacman/managers/sliceViewer.py` & `ipam_pacman-1.0.0rc1/pacman/managers/sliceViewer.py`

 * *Files identical despite different names*

### Comparing `ipam_pacman-1.0.0/pacman/utils/utils.py` & `ipam_pacman-1.0.0rc1/pacman/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,27 @@
     -------
     None.
 
     """
     global msgbuffer, output_dir, experiment    
     if(toGUI):
         guibuffer.append(msg)
-    T = datetime.datetime.now().strftime("%d/%m (%H:%M:%S)")
+    T = datetime.now().strftime("%d/%m (%H:%M:%S)")
     frmstr = f"T:{T}: {msg}"
     if(toFile):
         msgbuffer.append(frmstr)
     print(frmstr)
     if(len(msgbuffer) > 10 or "Experiment Finished" in msg or "Experiment cancelled" in msg):
         fp = output_dir
         with open(fp + "\\" + f"{experiment}_log.txt", mode='a') as file_object:
             for msgiter in msgbuffer:
                 file_object.write('%s\n' % msgiter)   
         msgbuffer.clear()
 
 def read_ini_file(file_path):
-    file_path = os.path.join(os.path.split(__file__)[0],"PACsettings.ini")
     if not os.path.isfile(file_path):
         raise FileNotFoundError(f"The PACsettings {file_path} was not found.")
     config = configparser.ConfigParser()
     config.read(file_path)
     ini_dict = {}
     for section in config.sections():
         section_dict = {}
```

### Comparing `ipam_pacman-1.0.0/LICENSE` & `ipam_pacman-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipam_pacman-1.0.0/README.md` & `ipam_pacman-1.0.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,56 @@
 Confirmed to be compliant with V 2.51d of Imaging-Win
 Confirmed to be compliant with PRIOR ProScan III controller
 
 PACKAGE REQUIREMENTS:
 
 pyserial
 opencv
-pycromanager
 comtypes
 ctypes
 numpy
 matplotlib
 skimage
 tkinter/ttk
 
 # REQUIREMENTS
 - ImagingWin v2.51 (see Installing ImagingWin)
-- Python 3.8
+- Python 3.9
 - Pip
 - Windows 7/8/10
 
 
-# Installing ImagingWin 
+# Installation of ImagingWin 2.51
 - Windows 10:
 The remote control functionality is only enabled in specifically the v 2.51 exe version of the ImagingWin program. 
-Due to this and ImagingWin supporting Windows 10 only on version >=2.56 the following steps must be taken to allow for remote control on Windows 10 systems: Install ImagingWin =2.56 as usual from Walz IMAGING-PAM download site. After installation: Make copy of the ImagingWin.exe file located in the installation folder. Overwrite the ImagingWin.exe in the installation folder with the v 2.51 exe provided with PACMan. 
+Due to this and ImagingWin supporting Windows 10 only on version >=2.56 the following steps must be taken to allow for remote control on Windows 10 systems: Install ImagingWin =2.56 as usual from Walz IMAGING-PAM download site (https://www.walz.com/products/chl_p700/imaging-pam_ms/downloads.html). After installation: Make copy of the ImagingWin.exe file located in the installation folder. Overwrite the ImagingWin.exe in the installation folder with the v 2.51 exe provided with PACMan. 
 
-# To use
+# Installation and use of PACMan
+- Install correct version of ImagingWin as above
 - Install with pip: pip install IPAM-PACMan
+
+In your python IDE of choice:
 - import pacman
 - PacMan_instance = pacman.PacMan()
+This starts PacMan with the GUI turned on, in standard mode.
+To start PacMan in CLI mode:
+- PacMan_instance = pacman.PacMan(False)
+
+To start PacMan in Debug mode:
+- PacMan_instance = pacman.PacMan(True/False,True)
+
+To change PACsettings write pacman.open_settings()
 
 # Version history
 
+v 1.0rc 19/03/2023
+- Release Candidate
+- Test installation performed
+- Bug fixes
+
 v 0.9.7 27/02/2023
 - Technical Debt
 	- Cleaning upp and testing installation file structure
 	- Bug fixes
 - Features
 	- Added PACSettings.ini: A settings file to tell PACMan what features to use, pointing it to the local ImagingWin installation, default output dir etc.
 
@@ -96,8 +111,8 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
-Contact: olle.ponten@gmail.com
+Contact: olle.ponten@gmail.com
```

### Comparing `ipam_pacman-1.0.0/pyproject.toml` & `ipam_pacman-1.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "IPAM-PACMan"
-version = "1.0.0"
+version = "1.0.0rc1"
 
 authors = [{name = "Olle Pontén",email="olle.ponten@gmail.com"}]
 description = "PACMan: An chlorophyll-a fluorometry automation software designed for Walz (GMBH) Microscopy IPAM."
 readme = "README.md"
 license = "GPL-3.0-or-later"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ipam_pacman-1.0.0/PKG-INFO` & `ipam_pacman-1.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPAM-PACMan
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: PACMan: An chlorophyll-a fluorometry automation software designed for Walz (GMBH) Microscopy IPAM.
 Project-URL: Homepage, https://pypi.org/project/IPAM-PACMan
 Project-URL: Github, https://github.com/OllePonten/PACMan
 Project-URL: Bug Tracker, https://github.com/OllePonten/PACMan/issues
 Author-email: Olle Pontén <olle.ponten@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -31,41 +31,56 @@
 Confirmed to be compliant with V 2.51d of Imaging-Win
 Confirmed to be compliant with PRIOR ProScan III controller
 
 PACKAGE REQUIREMENTS:
 
 pyserial
 opencv
-pycromanager
 comtypes
 ctypes
 numpy
 matplotlib
 skimage
 tkinter/ttk
 
 # REQUIREMENTS
 - ImagingWin v2.51 (see Installing ImagingWin)
-- Python 3.8
+- Python 3.9
 - Pip
 - Windows 7/8/10
 
 
-# Installing ImagingWin 
+# Installation of ImagingWin 2.51
 - Windows 10:
 The remote control functionality is only enabled in specifically the v 2.51 exe version of the ImagingWin program. 
-Due to this and ImagingWin supporting Windows 10 only on version >=2.56 the following steps must be taken to allow for remote control on Windows 10 systems: Install ImagingWin =2.56 as usual from Walz IMAGING-PAM download site. After installation: Make copy of the ImagingWin.exe file located in the installation folder. Overwrite the ImagingWin.exe in the installation folder with the v 2.51 exe provided with PACMan. 
+Due to this and ImagingWin supporting Windows 10 only on version >=2.56 the following steps must be taken to allow for remote control on Windows 10 systems: Install ImagingWin =2.56 as usual from Walz IMAGING-PAM download site (https://www.walz.com/products/chl_p700/imaging-pam_ms/downloads.html). After installation: Make copy of the ImagingWin.exe file located in the installation folder. Overwrite the ImagingWin.exe in the installation folder with the v 2.51 exe provided with PACMan. 
 
-# To use
+# Installation and use of PACMan
+- Install correct version of ImagingWin as above
 - Install with pip: pip install IPAM-PACMan
+
+In your python IDE of choice:
 - import pacman
 - PacMan_instance = pacman.PacMan()
+This starts PacMan with the GUI turned on, in standard mode.
+To start PacMan in CLI mode:
+- PacMan_instance = pacman.PacMan(False)
+
+To start PacMan in Debug mode:
+- PacMan_instance = pacman.PacMan(True/False,True)
+
+To change PACsettings write pacman.open_settings()
 
 # Version history
 
+v 1.0rc 19/03/2023
+- Release Candidate
+- Test installation performed
+- Bug fixes
+
 v 0.9.7 27/02/2023
 - Technical Debt
 	- Cleaning upp and testing installation file structure
 	- Bug fixes
 - Features
 	- Added PACSettings.ini: A settings file to tell PACMan what features to use, pointing it to the local ImagingWin installation, default output dir etc.
 
@@ -123,8 +138,8 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
-Contact: olle.ponten@gmail.com
+Contact: olle.ponten@gmail.com
```

