# Comparing `tmp/dextrusion-0.0.6.tar.gz` & `tmp/dextrusion-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dextrusion-0.0.6.tar", last modified: Thu Feb  9 12:30:03 2023, max compression
+gzip compressed data, was "dextrusion-0.0.7.tar", last modified: Wed May  3 09:24:12 2023, max compression
```

## Comparing `dextrusion-0.0.6.tar` & `dextrusion-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-02-09 12:30:03.345062 dextrusion-0.0.6/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    16798 2023-02-09 12:30:03.345062 dextrusion-0.0.6/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    14918 2023-02-09 12:29:34.000000 dextrusion-0.0.6/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       81 2023-02-01 13:06:55.000000 dextrusion-0.0.6/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       38 2023-02-09 12:30:03.345062 dextrusion-0.0.6/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      860 2023-02-09 12:29:43.000000 dextrusion-0.0.6/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-02-09 12:30:03.345062 dextrusion-0.0.6/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-02-09 12:30:03.345062 dextrusion-0.0.6/src/dextrusion/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    32410 2023-02-09 10:18:27.000000 dextrusion-0.0.6/src/dextrusion/DeXtrusion.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9883 2023-02-09 09:20:51.000000 dextrusion-0.0.6/src/dextrusion/DialogDeXtrusion.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     2505 2023-02-01 13:06:55.000000 dextrusion-0.0.6/src/dextrusion/DialogParameters.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    17382 2023-02-01 13:06:55.000000 dextrusion-0.0.6/src/dextrusion/MovieGeneratorFromROI.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9928 2023-02-01 13:06:55.000000 dextrusion-0.0.6/src/dextrusion/Network.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     6879 2023-02-01 13:06:55.000000 dextrusion-0.0.6/src/dextrusion/RoiUtils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        0 2023-02-01 13:06:55.000000 dextrusion-0.0.6/src/dextrusion/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4663 2023-02-09 09:20:36.000000 dextrusion-0.0.6/src/dextrusion/__main__.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-02-09 12:30:03.345062 dextrusion-0.0.6/src/dextrusion.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    16798 2023-02-09 12:30:03.000000 dextrusion-0.0.6/src/dextrusion.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      468 2023-02-09 12:30:03.000000 dextrusion-0.0.6/src/dextrusion.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-02-09 12:30:03.000000 dextrusion-0.0.6/src/dextrusion.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      129 2023-02-09 12:30:03.000000 dextrusion-0.0.6/src/dextrusion.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       11 2023-02-09 12:30:03.000000 dextrusion-0.0.6/src/dextrusion.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-05-03 09:24:12.527809 dextrusion-0.0.7/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1542 2023-02-01 13:06:55.000000 dextrusion-0.0.7/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    15212 2023-05-03 09:24:12.527809 dextrusion-0.0.7/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    14918 2023-02-09 12:29:34.000000 dextrusion-0.0.7/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       81 2023-02-01 13:06:55.000000 dextrusion-0.0.7/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       38 2023-05-03 09:24:12.527809 dextrusion-0.0.7/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      860 2023-05-03 09:18:17.000000 dextrusion-0.0.7/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-05-03 09:24:12.527809 dextrusion-0.0.7/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-05-03 09:24:12.527809 dextrusion-0.0.7/src/dextrusion/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    32678 2023-05-03 09:17:57.000000 dextrusion-0.0.7/src/dextrusion/DeXtrusion.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9883 2023-02-09 09:20:51.000000 dextrusion-0.0.7/src/dextrusion/DialogDeXtrusion.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     2505 2023-02-01 13:06:55.000000 dextrusion-0.0.7/src/dextrusion/DialogParameters.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    17382 2023-02-01 13:06:55.000000 dextrusion-0.0.7/src/dextrusion/MovieGeneratorFromROI.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9928 2023-02-01 13:06:55.000000 dextrusion-0.0.7/src/dextrusion/Network.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     6879 2023-02-01 13:06:55.000000 dextrusion-0.0.7/src/dextrusion/RoiUtils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        0 2023-02-01 13:06:55.000000 dextrusion-0.0.7/src/dextrusion/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4663 2023-02-09 09:20:36.000000 dextrusion-0.0.7/src/dextrusion/__main__.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-05-03 09:24:12.527809 dextrusion-0.0.7/src/dextrusion.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    15212 2023-05-03 09:24:12.000000 dextrusion-0.0.7/src/dextrusion.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      476 2023-05-03 09:24:12.000000 dextrusion-0.0.7/src/dextrusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-05-03 09:24:12.000000 dextrusion-0.0.7/src/dextrusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      129 2023-05-03 09:24:12.000000 dextrusion-0.0.7/src/dextrusion.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       11 2023-05-03 09:24:12.000000 dextrusion-0.0.7/src/dextrusion.egg-info/top_level.txt
```

### Comparing `dextrusion-0.0.6/PKG-INFO` & `dextrusion-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,205 +1,195 @@
-Metadata-Version: 2.1
-Name: dextrusion
-Version: 0.0.6
-Summary: DeXtrusion: automatic detection of cell extrusion in epithelial tissu
-Home-page: https://gitlab.pasteur.fr/gletort/dextrusion
-Author: Gaëlle Letort and Alexis Villars
-License: UNKNOWN
-Description: # ![DeXtrusion](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/DeX.png "DeXtrusion") DeXtrusion
-        
-        DeXtrusion is  a machine learning based python pipeline to detect cell extrusions in epithelial tissues movies. It can also detect cell divisions and SOPs, and can easily be trained to detect other dynamic events. 
-        
-        This repository contains the code source of the python DeXtrusion library, the trained neural networks (ready to use) with Jupyter notebooks to run, train or retrain DeXtrusion networks, and Fiji macros for visualization/analysis of the results.
-        
-        * [Presentation](#presentation)
-        * [Installation](#installation)
-        * [Usage](#usage)
-        * [Data](#data)
-        * [DeXtrusion networks](#dexnets-dextrusion-neural-networks)
-        * [Fiji macros](#fiji-macros)
-        * [Jupyter notebooks](#jupyter-notebooks)
-        * [References](#references)
-        
-        ## Presentation
-        DeXtrusion takes as input a movie of an epithelium and outputs the **spatio-temporal location of cell extrusion events** or other event as cell divisions. 
-        The movie is discretized into small overlapping rolling windows which are individually [classified for event detection](#event-classification) by a trained [neural network](#deXNets-deXtrusion-neural-networks). Results are then put together in event [probability map](#event-probability-map) for the whole movie or as [spatio-temporal points](#event-spot-localization) indicating each event. 
-        
-        <p align="center">
-        ![Example extrusion detection](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/SequenceExtrusion.png "Extrusion detection example") 
-        Example of the detection of an extrusion event (probability map, red).
-        </p>
-        
-        
-        ### Event classification
-        The movie is discretized into small windows that span all the movie in a rolling windows fashion with overlap between the different windows. 
-        Each window is classified by a trained neural network as containing or not a cellular event as cell extrusion. The different classes available in the main DeXtrusion network are:
-        - No event
-        - Cell extrusion/cell death
-        - Cell division
-        - SOPs
-        
-        It is easy to add or remove a cellular event to this list, but necessitates to train new neural networks for this. Jupyter notebook is available in this repository to do it.
-        
-        ### Event probability map
-        Each window is associated an event probability which allow to generate an events probability map on the whole movie. This probability maps can be refined to precise spatio-temporal spots for each event.
-        The results can be visualized by overlaying the initial movie and all the probability maps saved by DeXtrusion in Fiji with the saved by DeXtrusion with the [`deXtrusion_overlayProbabilityMaps.ijm`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) macro.
-        
-        <p align="center">
-        ![Example probability maps](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/images/SequenceProbamaps.png?raw=True "Probability map example") 
-        </p>
-        
-        Example of probability maps (green: division, red: extrusion, blue: SOP
-        
-        ### Event spot localization
-        An event is visible in the probability map as a volume of connected pixels of high probability. To convert the probability map to a list of event, we place the event localization at the center of each of these high probability volumes.
-        Moreover, to reduce false positive detections, the volumes can be thresholded to keep only big enough volume of high enough probability values. 
-        The list of spots obtained in this way are saved in ROIS `.zip` file that can be open in Fiji through the `ROIManager` tool. The macro [`deXtrusion_showROIs.ijm`](#https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) allows to directly visualize with Fiji the results saved by DeXtrusion. 
-        
-        
-        ## Installation
-        DeXtrusion is distributed as a python module, compatible with `python3`. 
-        You can install it in a virtual environment to be sure to have the required versions.
-        **DeXtrusion** can be installed either manually through the setup file or with pip:
-        
-        * DeXtrusion can be directly installed via pip. In your python virtual environment, enter: `pip install dextrusion` to install it.
-        You should also download the trained neural network [DeXNet](#dexnets-dextrusion-neural-networks) that you want to use from this repository.
-        
-        * To install manually **DeXtrusion**, clone this github repository, and inside this repository type: `python setup.py install`. 
-        If you want to install it in a virtual environment, you should have activated it before.
-        It will install all the necessary dependencies.
-        
-        
-        ### Detailled installation on Linux (Ubuntu)
-        Here's a step by step command lines to run in a Terminal to install DeXtrusion on Linux from scratch. It is creating a new virtual environment on which DeXtrusion will be installed (not necessary but recommended). Tested with `python 3.8`.
-        
-        * Installation with `pip`
-        ```sh
-        python3 -m venv dextrusenv               ## create a virtual environment with python 3 called dextrusenv (you can choose the name)
-        source dextrusenv/bin/activate           ## activate the virtual environment: now python commands will be runned in that environment
-        pip install dextrusion                  ## install DeXtrusion, download all the necessary dependencies, can take time
-        ```
-        DeXtrusion is installed and can be runned with:
-        
-        ```sh
-        python -m dextrusion 	                  ## run DeXtrusion. Next time to run it again with the same networks, you only have to do this line
-        ```
-        
-        DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the DeXNets repository), you have to download and uncompress it. From the command line:
-        
-        ```sh
-        mkdir DeXNets							## create directory on which neural networks will be put
-        mkdir DeXNets/notum_ExtSOPDiv			## create directory for the neural networks traind with 4 events available in this repository
-        cd DeXNets/notum_ExtSOPDiv               ## go inside the desired neural networks directory (here the network trained with 4 events)
-        wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv0.zip   ## download the first neural network
-        wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv1.zip   ## download the second neural network
-        unzip notumExtSOPDiv0.zip                ## uncompress it. It is now ready to be used
-        unzip notumExtSOPDiv1.zip
-        cd ../..                                 ## go back to main DeXtrusion directory
-        ```
-         
-        * You can also clone this repository and install DeXtrusion from the source code `python setup.py install` instead of using pip installation.
-        
-        
-        ### Detailled installation on Windows
-        You need to have anaconda installed to run python and create a new virtual environment. On the command prompt, write:
-        ```cmd
-        $ C:\ProgramData\Anaconda3\Scripts\Activate     ## activate conda (should be the path of your anaconda installation)
-        $ conda create --name dextrusionenv python=3.8  ## to create virtual environment called dextrusionenv
-        $ conda activate dextrusionenv                  ## activate the virtual environment that you juste created
-        $ pip install dextrusion                        ## install DeXtrusion in it
-        $ python -m dextrusion                          ## Run it
-        ```
-        
-        ### Choose the neural network DeXNets to use
-        DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the [DeXNets repository](./DeXNets)), you have to download and uncompress it. 
-        From DeXtrusion user interface, to select a network to run, you have to go inside its uncompressed directory (click on `Browse` and go there). If you want to use several networks together for the detection for better results (see our paper), the networks folders should be placed within the same directory. Go inside that directy with the interface, and it will use all the networks presents in that directory.
-        
-        ## Usage
-        
-        DeXtrusion can be used directly within python. 
-        To run an already trained network and detect cell events, run `python3 -m dextrusion` in your virtual environment. It will open a graphical interface to perform the detection.
-        
-        We also propose [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks) in this repository, to use dextrusion options. 
-        You can find a notebook to perform the detection, train a new neural network, retrain a network or evaluate the performance of the network compared to a manual detection.
-        
-        
-        ## Data
-        Data used for the training of our neural networks (raw movies with manual anotation of events) are freely available on Zenodo. 
-        
-        
-        ## DeXNets: deXtrusion neural networks
-        DeXtrusion was trained on E-cadherin tagged drosophilia notum but can be easily adapted to other markers/biological conditions. Retraining of DeXtrusion network may be necessary when images are quite different.
-        
-        In the `deXNets` folder of this repository, we proposed several trained networks:
-        - `notum_Ext`: trained on drosophilia notum movies with only extrusion events
-        - `notum_ExtSOP`: trained on drosophilia notum movies with extrusion and SOP events
-        - `notum_ExtSOPDiv`: trained on drosophilia notum movies with extrusion, division and SOP events
-        - `notum_all`: trained on drosophilia notum movies with extrusion, division and SOP events, on all our annotated data (training and test). Networks to use by default.
-        
-        Download them and unzip to be ready to use in DeXtrusion.
-        
-        ### Train/retrain a new DeXNet
-        If you want to train/retrain a neural network, to add a new event to detect or to improve its performance on new datasets, Jupyter notebooks are proposed in this repository: [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks). You can just follow step by step the notebook.
-        
-        If you want to change the architecture of DeXNet, you will have to change it in the `src/dextrusion/Network.py` file. The architecture is defined in the `action_model` function.
-        
-        
-        ## Fiji macros
-        
-        Fiji macros to prepare data for DeXtrusion neural network training or to handle DeXtrusion results are available in the [`Fiji macros`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/) folder of this repository.
-        
-        * [deXtrusion_checkAndClearROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_checkAndClearROIs.ijm) allows to check manually all the detected ROIs and to keep only the correct ones. 
-        It shows each event (point ROI) detected by deXtrusion as a pop-up window centered temporally and spatially around the event.
-        The user is asked wether the detection is correct (if there is an event in the current window) by pressing `y` or `n`.
-        If yes, the ROI is kept, else it will be removed from the list of ROIs.
-        
-        
-        * [deXtrusion_scoreROIs_Random.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_scoreROIs_Random.ijm) allows to score manually the precision of the detected events.
-        The macro will open randomly a given number of ROIs, and show a window centered temporally and spatially around the event.
-        The user is asked wether the detection is correct (if it contains the event) by pressing `y` or `n`.
-        The macro will output the count of correct and false detections and the precision. 
-        The ROIs file will not be edited and the ROIs left after running this macro should not be saved as it deletes all the ROIs explored to be sure not to draw them twice.
-        
-        * [deXtrusion_overlayProbabilityMaps.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) allows to visualize the probability maps together with the original image.
-        The user is asked for the original image to visualize and will open the probability maps in the `results` folder where they should be saved by default.
-        The directory to look in can be changed in the macro. 
-        
-        * [deXtrusion_showROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) displays the original movie (chosen by the user) and the ROI file found in the `results` folder. 
-        The location of the ROI file can be changed in the macro by changing the `resfold` parameter and the event to show (by default extrusion) can be changed in the `type` parameter.
-        
-        * [deXtrusion_subsetMovieAndRois.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_subsetMovieAndRois.ijm) save a temporal subset of a movie, and keep only the corresponding ROIs. 
-        
-        
-        ## Jupyter notebooks
-        We provide in this repository several jupyter notebooks to run, train/retrain, evaluate DeXtrusion. 
-        * [detectEventsOnMovie.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/detectEventsOnMovie.ipynb) allows you to run DeXtrusion with the graphical interaface to choose the parameters. 
-        * [deXtrusion_TrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_TrainNetwork.ipynb) to train a new DeXNet network with your own data (or using our data publicly available, see [data section](#Data)).
-        * [deXtrusion_RetrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_RetrainNetwork.ipynb) to retrain an already trained neural network with new data.
-        * [deXtrusion_CompareRois.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_CompareRois.ipynb) to compare two ROIs files (manual detection vs DeXtrusion detection) and gives the score. It can also generate ROIs files of the false detection (false positives and/or false negatives).
-        * [deXtrusion_testClassification_OnWindows.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_testClassification_OnWindows.ipynb): run the trained neural network (DeXNet) on test data on generated windows, and print the resulting confusion matrix of the classification (DeXtrusion classification compared to the manual classification).
-        
-        #### Notebooks usage
-        * If you have Jupyter installed on your computer, to add your virtual environment to the environment Jupyter can see:
-        ```
-        ipython kernel install --user --name=dextrusionenv
-        ```
-        You can refer to this [tutorial](https://www.geeksforgeeks.org/using-jupyter-notebook-in-virtual-environment/) for instructions on creating virtual environment and using it with jupyter.
-        
-        * You can also install Jupyter Lab or Jupyter notebook in your virtual environment if you don't have it installed in your computer:
-        ```sh
-        pip install jupyterlab
-        jupyter-lab
-        ```
-        Refer to [Jupyter](https://jupyter.org/) webpage for more information.
-        
-        ## References
-        To know more about DeXtrusion, refer to our paper: Villars, Letort et al. 2023.
-        
-        ## License
-        DeXtrusion is distributed open-source under the BSD-3 license, see the license file in this repository.
-        
-        When you use DeXtrusion source code, neural networks or data for your projects, please cite our paper. 
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# ![DeXtrusion](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/DeX.png "DeXtrusion") DeXtrusion
+
+DeXtrusion is  a machine learning based python pipeline to detect cell extrusions in epithelial tissues movies. It can also detect cell divisions and SOPs, and can easily be trained to detect other dynamic events. 
+
+This repository contains the code source of the python DeXtrusion library, the trained neural networks (ready to use) with Jupyter notebooks to run, train or retrain DeXtrusion networks, and Fiji macros for visualization/analysis of the results.
+
+* [Presentation](#presentation)
+* [Installation](#installation)
+* [Usage](#usage)
+* [Data](#data)
+* [DeXtrusion networks](#dexnets-dextrusion-neural-networks)
+* [Fiji macros](#fiji-macros)
+* [Jupyter notebooks](#jupyter-notebooks)
+* [References](#references)
+
+## Presentation
+DeXtrusion takes as input a movie of an epithelium and outputs the **spatio-temporal location of cell extrusion events** or other event as cell divisions. 
+The movie is discretized into small overlapping rolling windows which are individually [classified for event detection](#event-classification) by a trained [neural network](#deXNets-deXtrusion-neural-networks). Results are then put together in event [probability map](#event-probability-map) for the whole movie or as [spatio-temporal points](#event-spot-localization) indicating each event. 
+
+<p align="center">
+![Example extrusion detection](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/SequenceExtrusion.png "Extrusion detection example") 
+Example of the detection of an extrusion event (probability map, red).
+</p>
+
+
+### Event classification
+The movie is discretized into small windows that span all the movie in a rolling windows fashion with overlap between the different windows. 
+Each window is classified by a trained neural network as containing or not a cellular event as cell extrusion. The different classes available in the main DeXtrusion network are:
+- No event
+- Cell extrusion/cell death
+- Cell division
+- SOPs
+
+It is easy to add or remove a cellular event to this list, but necessitates to train new neural networks for this. Jupyter notebook is available in this repository to do it.
+
+### Event probability map
+Each window is associated an event probability which allow to generate an events probability map on the whole movie. This probability maps can be refined to precise spatio-temporal spots for each event.
+The results can be visualized by overlaying the initial movie and all the probability maps saved by DeXtrusion in Fiji with the saved by DeXtrusion with the [`deXtrusion_overlayProbabilityMaps.ijm`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) macro.
+
+<p align="center">
+![Example probability maps](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/images/SequenceProbamaps.png?raw=True "Probability map example") 
+</p>
+
+Example of probability maps (green: division, red: extrusion, blue: SOP
+
+### Event spot localization
+An event is visible in the probability map as a volume of connected pixels of high probability. To convert the probability map to a list of event, we place the event localization at the center of each of these high probability volumes.
+Moreover, to reduce false positive detections, the volumes can be thresholded to keep only big enough volume of high enough probability values. 
+The list of spots obtained in this way are saved in ROIS `.zip` file that can be open in Fiji through the `ROIManager` tool. The macro [`deXtrusion_showROIs.ijm`](#https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) allows to directly visualize with Fiji the results saved by DeXtrusion. 
+
+
+## Installation
+DeXtrusion is distributed as a python module, compatible with `python3`. 
+You can install it in a virtual environment to be sure to have the required versions.
+**DeXtrusion** can be installed either manually through the setup file or with pip:
+
+* DeXtrusion can be directly installed via pip. In your python virtual environment, enter: `pip install dextrusion` to install it.
+You should also download the trained neural network [DeXNet](#dexnets-dextrusion-neural-networks) that you want to use from this repository.
+
+* To install manually **DeXtrusion**, clone this github repository, and inside this repository type: `python setup.py install`. 
+If you want to install it in a virtual environment, you should have activated it before.
+It will install all the necessary dependencies.
+
+
+### Detailled installation on Linux (Ubuntu)
+Here's a step by step command lines to run in a Terminal to install DeXtrusion on Linux from scratch. It is creating a new virtual environment on which DeXtrusion will be installed (not necessary but recommended). Tested with `python 3.8`.
+
+* Installation with `pip`
+```sh
+python3 -m venv dextrusenv               ## create a virtual environment with python 3 called dextrusenv (you can choose the name)
+source dextrusenv/bin/activate           ## activate the virtual environment: now python commands will be runned in that environment
+pip install dextrusion                  ## install DeXtrusion, download all the necessary dependencies, can take time
+```
+DeXtrusion is installed and can be runned with:
+
+```sh
+python -m dextrusion 	                  ## run DeXtrusion. Next time to run it again with the same networks, you only have to do this line
+```
+
+DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the DeXNets repository), you have to download and uncompress it. From the command line:
+
+```sh
+mkdir DeXNets							## create directory on which neural networks will be put
+mkdir DeXNets/notum_ExtSOPDiv			## create directory for the neural networks traind with 4 events available in this repository
+cd DeXNets/notum_ExtSOPDiv               ## go inside the desired neural networks directory (here the network trained with 4 events)
+wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv0.zip   ## download the first neural network
+wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv1.zip   ## download the second neural network
+unzip notumExtSOPDiv0.zip                ## uncompress it. It is now ready to be used
+unzip notumExtSOPDiv1.zip
+cd ../..                                 ## go back to main DeXtrusion directory
+```
+ 
+* You can also clone this repository and install DeXtrusion from the source code `python setup.py install` instead of using pip installation.
+
+
+### Detailled installation on Windows
+You need to have anaconda installed to run python and create a new virtual environment. On the command prompt, write:
+```cmd
+$ C:\ProgramData\Anaconda3\Scripts\Activate     ## activate conda (should be the path of your anaconda installation)
+$ conda create --name dextrusionenv python=3.8  ## to create virtual environment called dextrusionenv
+$ conda activate dextrusionenv                  ## activate the virtual environment that you juste created
+$ pip install dextrusion                        ## install DeXtrusion in it
+$ python -m dextrusion                          ## Run it
+```
+
+### Choose the neural network DeXNets to use
+DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the [DeXNets repository](./DeXNets)), you have to download and uncompress it. 
+From DeXtrusion user interface, to select a network to run, you have to go inside its uncompressed directory (click on `Browse` and go there). If you want to use several networks together for the detection for better results (see our paper), the networks folders should be placed within the same directory. Go inside that directy with the interface, and it will use all the networks presents in that directory.
+
+## Usage
+
+DeXtrusion can be used directly within python. 
+To run an already trained network and detect cell events, run `python3 -m dextrusion` in your virtual environment. It will open a graphical interface to perform the detection.
+
+We also propose [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks) in this repository, to use dextrusion options. 
+You can find a notebook to perform the detection, train a new neural network, retrain a network or evaluate the performance of the network compared to a manual detection.
+
+
+## Data
+Data used for the training of our neural networks (raw movies with manual anotation of events) are freely available on Zenodo. 
+
+
+## DeXNets: deXtrusion neural networks
+DeXtrusion was trained on E-cadherin tagged drosophilia notum but can be easily adapted to other markers/biological conditions. Retraining of DeXtrusion network may be necessary when images are quite different.
+
+In the `deXNets` folder of this repository, we proposed several trained networks:
+- `notum_Ext`: trained on drosophilia notum movies with only extrusion events
+- `notum_ExtSOP`: trained on drosophilia notum movies with extrusion and SOP events
+- `notum_ExtSOPDiv`: trained on drosophilia notum movies with extrusion, division and SOP events
+- `notum_all`: trained on drosophilia notum movies with extrusion, division and SOP events, on all our annotated data (training and test). Networks to use by default.
+
+Download them and unzip to be ready to use in DeXtrusion.
+
+### Train/retrain a new DeXNet
+If you want to train/retrain a neural network, to add a new event to detect or to improve its performance on new datasets, Jupyter notebooks are proposed in this repository: [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks). You can just follow step by step the notebook.
+
+If you want to change the architecture of DeXNet, you will have to change it in the `src/dextrusion/Network.py` file. The architecture is defined in the `action_model` function.
+
+
+## Fiji macros
+
+Fiji macros to prepare data for DeXtrusion neural network training or to handle DeXtrusion results are available in the [`Fiji macros`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/) folder of this repository.
+
+* [deXtrusion_checkAndClearROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_checkAndClearROIs.ijm) allows to check manually all the detected ROIs and to keep only the correct ones. 
+It shows each event (point ROI) detected by deXtrusion as a pop-up window centered temporally and spatially around the event.
+The user is asked wether the detection is correct (if there is an event in the current window) by pressing `y` or `n`.
+If yes, the ROI is kept, else it will be removed from the list of ROIs.
+
+
+* [deXtrusion_scoreROIs_Random.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_scoreROIs_Random.ijm) allows to score manually the precision of the detected events.
+The macro will open randomly a given number of ROIs, and show a window centered temporally and spatially around the event.
+The user is asked wether the detection is correct (if it contains the event) by pressing `y` or `n`.
+The macro will output the count of correct and false detections and the precision. 
+The ROIs file will not be edited and the ROIs left after running this macro should not be saved as it deletes all the ROIs explored to be sure not to draw them twice.
+
+* [deXtrusion_overlayProbabilityMaps.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) allows to visualize the probability maps together with the original image.
+The user is asked for the original image to visualize and will open the probability maps in the `results` folder where they should be saved by default.
+The directory to look in can be changed in the macro. 
+
+* [deXtrusion_showROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) displays the original movie (chosen by the user) and the ROI file found in the `results` folder. 
+The location of the ROI file can be changed in the macro by changing the `resfold` parameter and the event to show (by default extrusion) can be changed in the `type` parameter.
+
+* [deXtrusion_subsetMovieAndRois.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_subsetMovieAndRois.ijm) save a temporal subset of a movie, and keep only the corresponding ROIs. 
+
+
+## Jupyter notebooks
+We provide in this repository several jupyter notebooks to run, train/retrain, evaluate DeXtrusion. 
+* [detectEventsOnMovie.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/detectEventsOnMovie.ipynb) allows you to run DeXtrusion with the graphical interaface to choose the parameters. 
+* [deXtrusion_TrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_TrainNetwork.ipynb) to train a new DeXNet network with your own data (or using our data publicly available, see [data section](#Data)).
+* [deXtrusion_RetrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_RetrainNetwork.ipynb) to retrain an already trained neural network with new data.
+* [deXtrusion_CompareRois.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_CompareRois.ipynb) to compare two ROIs files (manual detection vs DeXtrusion detection) and gives the score. It can also generate ROIs files of the false detection (false positives and/or false negatives).
+* [deXtrusion_testClassification_OnWindows.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_testClassification_OnWindows.ipynb): run the trained neural network (DeXNet) on test data on generated windows, and print the resulting confusion matrix of the classification (DeXtrusion classification compared to the manual classification).
+
+#### Notebooks usage
+* If you have Jupyter installed on your computer, to add your virtual environment to the environment Jupyter can see:
+```
+ipython kernel install --user --name=dextrusionenv
+```
+You can refer to this [tutorial](https://www.geeksforgeeks.org/using-jupyter-notebook-in-virtual-environment/) for instructions on creating virtual environment and using it with jupyter.
+
+* You can also install Jupyter Lab or Jupyter notebook in your virtual environment if you don't have it installed in your computer:
+```sh
+pip install jupyterlab
+jupyter-lab
+```
+Refer to [Jupyter](https://jupyter.org/) webpage for more information.
+
+## References
+To know more about DeXtrusion, refer to our paper: Villars, Letort et al. 2023.
+
+## License
+DeXtrusion is distributed open-source under the BSD-3 license, see the license file in this repository.
+
+When you use DeXtrusion source code, neural networks or data for your projects, please cite our paper. 
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dextrusion-0.0.6/README.md` & `dextrusion-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: dextrusion
+Version: 0.0.7
+Summary: DeXtrusion: automatic detection of cell extrusion in epithelial tissu
+Home-page: https://gitlab.pasteur.fr/gletort/dextrusion
+Author: Gaëlle Letort and Alexis Villars
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ![DeXtrusion](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/DeX.png "DeXtrusion") DeXtrusion
 
 DeXtrusion is  a machine learning based python pipeline to detect cell extrusions in epithelial tissues movies. It can also detect cell divisions and SOPs, and can easily be trained to detect other dynamic events. 
 
 This repository contains the code source of the python DeXtrusion library, the trained neural networks (ready to use) with Jupyter notebooks to run, train or retrain DeXtrusion networks, and Fiji macros for visualization/analysis of the results.
 
 * [Presentation](#presentation)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dextrusion-0.0.6/setup.py` & `dextrusion-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='dextrusion',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.6',
+    version='0.0.7',
     description='DeXtrusion: automatic detection of cell extrusion in epithelial tissu',
       author='Gaëlle Letort and Alexis Villars',
       url='https://gitlab.pasteur.fr/gletort/dextrusion',
       package_dir={'':'src'},
       packages=find_packages('src'),
     install_requires=[
         "matplotlib",
```

### Comparing `dextrusion-0.0.6/src/dextrusion/DeXtrusion.py` & `dextrusion-0.0.7/src/dextrusion/DeXtrusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         try:
             if self.probamap is not None:
                 del self.probamap
                 gc.collect()
                 self.probamap = None
         except:
             self.probamap = None
-        self.probamap = zeros((3,)+self.scaled_shape, dtype="uint8")
+        self.probamap = zeros((self.ncat-1,)+self.scaled_shape, dtype="uint8")
         for c in range(self.ncat-1):
             self.probamap[c,:,:,:] = uint8(res[c,(self.nframes[0]):(res.shape[1]-self.nframes[1]),:,:]/nres[(self.nframes[0]):(res.shape[1]-self.nframes[1]),:,:]*255)
 
     def do_one_group(self, img, pred_channels, npred, group):
         """ Categorize one batch of windows (one group), put the results in pred_channels """
         if self.verbose:
             print("     - Do one group: "+str(group))
@@ -437,17 +437,21 @@
         self.divide(pred_channels, npred)
         del pred_channels
         del npred
   
     ##################################################################################################
     ####### Postprocess results: probability maps, Fiji ROIs
     
-    def rescale_position(self, z, y, x):
-        ratioxy = self.init_shape[1]/self.probamap.shape[2]
-        ratioz = self.init_shape[0]/self.probamap.shape[1]
+    def rescale_position(self, z, y, x, probshape=None):
+        if probshape is not None:
+            probashape = probshape
+        else:
+            probashape = self.probamap.shape
+        ratioxy = self.init_shape[1]/probashape[2]
+        ratioz = self.init_shape[0]/probashape[1]
         z = floor(z*ratioz)
         y = floor(y*ratioxy)
         x = floor(x*ratioxy)
         return z, y, x
 
     def resize_probamap(self, cat=1):
         ''' resize to initial size proba map '''
@@ -597,26 +601,28 @@
     
         return binimg, labels, listlabels, vols, vals
 
     
     def get_rois_fromrawproba_path(self, imagepath=None, cat=1, volume_threshold=800, proba_threshold=180, disxy=10, dist=4, outfile=None):
         """ 
            Clean the raw probamap, get rois and rescale to original image size 
+           Read the raw probamap in the results folder.
         """
-        if imgpath is None:
+        if imagepath is None:
             img = self.probamap[cat-1]
         else:
-            img = self.get_rawproba_frompath( imgpath, cat=cat)
+            img = self.get_rawproba_frompath( imagepath, cat=cat)
 
-        bimg, labels, llabels, vols, vals = self.rawproba_to_volumes( img, threshold=125, mindxy=mindxy, mindt=mindt )
+        bimg, labels, llabels, vols, vals = self.rawproba_to_volumes( img, threshold=125, mindxy=disxy, mindt=dist )
         coords = measurements.center_of_mass(bimg, labels=labels, index=llabels)
         rois = []
         for (pt, vol, val) in zip(coords, vols, vals):
             if not isnan(pt[0]) and (vol>volume_threshold) and (val>proba_threshold):
-                rois.append(ru.create_roi((floor(pt[0]), floor(pt[1]), floor(pt[2])), cat=cat))
+                roiz, roiy, roix = self.rescale_position( pt[0], pt[1], pt[2], ((1,))+img.shape )
+                rois.append(ru.create_roi((roiz, roiy, roix), cat=cat))
             
         if outfile is None:
             outfile = self.outname+self.catnames[cat]
         ru.write_rois(outfile, rois, verbose=self.verbose)
 
     def compare_rois(self, cat, gtroisfile, resroisfile=None, distance_xy=15, distance_t=4):
         """ Compare two ROIs files and measure accuracy metrics (precision, recall)
```

### Comparing `dextrusion-0.0.6/src/dextrusion/DialogDeXtrusion.py` & `dextrusion-0.0.7/src/dextrusion/DialogDeXtrusion.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion/DialogParameters.py` & `dextrusion-0.0.7/src/dextrusion/DialogParameters.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion/MovieGeneratorFromROI.py` & `dextrusion-0.0.7/src/dextrusion/MovieGeneratorFromROI.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion/Network.py` & `dextrusion-0.0.7/src/dextrusion/Network.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion/RoiUtils.py` & `dextrusion-0.0.7/src/dextrusion/RoiUtils.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion/__main__.py` & `dextrusion-0.0.7/src/dextrusion/__main__.py`

 * *Files identical despite different names*

### Comparing `dextrusion-0.0.6/src/dextrusion.egg-info/PKG-INFO` & `dextrusion-0.0.7/src/dextrusion.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,205 +1,204 @@
 Metadata-Version: 2.1
 Name: dextrusion
-Version: 0.0.6
+Version: 0.0.7
 Summary: DeXtrusion: automatic detection of cell extrusion in epithelial tissu
 Home-page: https://gitlab.pasteur.fr/gletort/dextrusion
 Author: Gaëlle Letort and Alexis Villars
-License: UNKNOWN
-Description: # ![DeXtrusion](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/DeX.png "DeXtrusion") DeXtrusion
-        
-        DeXtrusion is  a machine learning based python pipeline to detect cell extrusions in epithelial tissues movies. It can also detect cell divisions and SOPs, and can easily be trained to detect other dynamic events. 
-        
-        This repository contains the code source of the python DeXtrusion library, the trained neural networks (ready to use) with Jupyter notebooks to run, train or retrain DeXtrusion networks, and Fiji macros for visualization/analysis of the results.
-        
-        * [Presentation](#presentation)
-        * [Installation](#installation)
-        * [Usage](#usage)
-        * [Data](#data)
-        * [DeXtrusion networks](#dexnets-dextrusion-neural-networks)
-        * [Fiji macros](#fiji-macros)
-        * [Jupyter notebooks](#jupyter-notebooks)
-        * [References](#references)
-        
-        ## Presentation
-        DeXtrusion takes as input a movie of an epithelium and outputs the **spatio-temporal location of cell extrusion events** or other event as cell divisions. 
-        The movie is discretized into small overlapping rolling windows which are individually [classified for event detection](#event-classification) by a trained [neural network](#deXNets-deXtrusion-neural-networks). Results are then put together in event [probability map](#event-probability-map) for the whole movie or as [spatio-temporal points](#event-spot-localization) indicating each event. 
-        
-        <p align="center">
-        ![Example extrusion detection](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/SequenceExtrusion.png "Extrusion detection example") 
-        Example of the detection of an extrusion event (probability map, red).
-        </p>
-        
-        
-        ### Event classification
-        The movie is discretized into small windows that span all the movie in a rolling windows fashion with overlap between the different windows. 
-        Each window is classified by a trained neural network as containing or not a cellular event as cell extrusion. The different classes available in the main DeXtrusion network are:
-        - No event
-        - Cell extrusion/cell death
-        - Cell division
-        - SOPs
-        
-        It is easy to add or remove a cellular event to this list, but necessitates to train new neural networks for this. Jupyter notebook is available in this repository to do it.
-        
-        ### Event probability map
-        Each window is associated an event probability which allow to generate an events probability map on the whole movie. This probability maps can be refined to precise spatio-temporal spots for each event.
-        The results can be visualized by overlaying the initial movie and all the probability maps saved by DeXtrusion in Fiji with the saved by DeXtrusion with the [`deXtrusion_overlayProbabilityMaps.ijm`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) macro.
-        
-        <p align="center">
-        ![Example probability maps](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/images/SequenceProbamaps.png?raw=True "Probability map example") 
-        </p>
-        
-        Example of probability maps (green: division, red: extrusion, blue: SOP
-        
-        ### Event spot localization
-        An event is visible in the probability map as a volume of connected pixels of high probability. To convert the probability map to a list of event, we place the event localization at the center of each of these high probability volumes.
-        Moreover, to reduce false positive detections, the volumes can be thresholded to keep only big enough volume of high enough probability values. 
-        The list of spots obtained in this way are saved in ROIS `.zip` file that can be open in Fiji through the `ROIManager` tool. The macro [`deXtrusion_showROIs.ijm`](#https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) allows to directly visualize with Fiji the results saved by DeXtrusion. 
-        
-        
-        ## Installation
-        DeXtrusion is distributed as a python module, compatible with `python3`. 
-        You can install it in a virtual environment to be sure to have the required versions.
-        **DeXtrusion** can be installed either manually through the setup file or with pip:
-        
-        * DeXtrusion can be directly installed via pip. In your python virtual environment, enter: `pip install dextrusion` to install it.
-        You should also download the trained neural network [DeXNet](#dexnets-dextrusion-neural-networks) that you want to use from this repository.
-        
-        * To install manually **DeXtrusion**, clone this github repository, and inside this repository type: `python setup.py install`. 
-        If you want to install it in a virtual environment, you should have activated it before.
-        It will install all the necessary dependencies.
-        
-        
-        ### Detailled installation on Linux (Ubuntu)
-        Here's a step by step command lines to run in a Terminal to install DeXtrusion on Linux from scratch. It is creating a new virtual environment on which DeXtrusion will be installed (not necessary but recommended). Tested with `python 3.8`.
-        
-        * Installation with `pip`
-        ```sh
-        python3 -m venv dextrusenv               ## create a virtual environment with python 3 called dextrusenv (you can choose the name)
-        source dextrusenv/bin/activate           ## activate the virtual environment: now python commands will be runned in that environment
-        pip install dextrusion                  ## install DeXtrusion, download all the necessary dependencies, can take time
-        ```
-        DeXtrusion is installed and can be runned with:
-        
-        ```sh
-        python -m dextrusion 	                  ## run DeXtrusion. Next time to run it again with the same networks, you only have to do this line
-        ```
-        
-        DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the DeXNets repository), you have to download and uncompress it. From the command line:
-        
-        ```sh
-        mkdir DeXNets							## create directory on which neural networks will be put
-        mkdir DeXNets/notum_ExtSOPDiv			## create directory for the neural networks traind with 4 events available in this repository
-        cd DeXNets/notum_ExtSOPDiv               ## go inside the desired neural networks directory (here the network trained with 4 events)
-        wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv0.zip   ## download the first neural network
-        wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv1.zip   ## download the second neural network
-        unzip notumExtSOPDiv0.zip                ## uncompress it. It is now ready to be used
-        unzip notumExtSOPDiv1.zip
-        cd ../..                                 ## go back to main DeXtrusion directory
-        ```
-         
-        * You can also clone this repository and install DeXtrusion from the source code `python setup.py install` instead of using pip installation.
-        
-        
-        ### Detailled installation on Windows
-        You need to have anaconda installed to run python and create a new virtual environment. On the command prompt, write:
-        ```cmd
-        $ C:\ProgramData\Anaconda3\Scripts\Activate     ## activate conda (should be the path of your anaconda installation)
-        $ conda create --name dextrusionenv python=3.8  ## to create virtual environment called dextrusionenv
-        $ conda activate dextrusionenv                  ## activate the virtual environment that you juste created
-        $ pip install dextrusion                        ## install DeXtrusion in it
-        $ python -m dextrusion                          ## Run it
-        ```
-        
-        ### Choose the neural network DeXNets to use
-        DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the [DeXNets repository](./DeXNets)), you have to download and uncompress it. 
-        From DeXtrusion user interface, to select a network to run, you have to go inside its uncompressed directory (click on `Browse` and go there). If you want to use several networks together for the detection for better results (see our paper), the networks folders should be placed within the same directory. Go inside that directy with the interface, and it will use all the networks presents in that directory.
-        
-        ## Usage
-        
-        DeXtrusion can be used directly within python. 
-        To run an already trained network and detect cell events, run `python3 -m dextrusion` in your virtual environment. It will open a graphical interface to perform the detection.
-        
-        We also propose [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks) in this repository, to use dextrusion options. 
-        You can find a notebook to perform the detection, train a new neural network, retrain a network or evaluate the performance of the network compared to a manual detection.
-        
-        
-        ## Data
-        Data used for the training of our neural networks (raw movies with manual anotation of events) are freely available on Zenodo. 
-        
-        
-        ## DeXNets: deXtrusion neural networks
-        DeXtrusion was trained on E-cadherin tagged drosophilia notum but can be easily adapted to other markers/biological conditions. Retraining of DeXtrusion network may be necessary when images are quite different.
-        
-        In the `deXNets` folder of this repository, we proposed several trained networks:
-        - `notum_Ext`: trained on drosophilia notum movies with only extrusion events
-        - `notum_ExtSOP`: trained on drosophilia notum movies with extrusion and SOP events
-        - `notum_ExtSOPDiv`: trained on drosophilia notum movies with extrusion, division and SOP events
-        - `notum_all`: trained on drosophilia notum movies with extrusion, division and SOP events, on all our annotated data (training and test). Networks to use by default.
-        
-        Download them and unzip to be ready to use in DeXtrusion.
-        
-        ### Train/retrain a new DeXNet
-        If you want to train/retrain a neural network, to add a new event to detect or to improve its performance on new datasets, Jupyter notebooks are proposed in this repository: [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks). You can just follow step by step the notebook.
-        
-        If you want to change the architecture of DeXNet, you will have to change it in the `src/dextrusion/Network.py` file. The architecture is defined in the `action_model` function.
-        
-        
-        ## Fiji macros
-        
-        Fiji macros to prepare data for DeXtrusion neural network training or to handle DeXtrusion results are available in the [`Fiji macros`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/) folder of this repository.
-        
-        * [deXtrusion_checkAndClearROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_checkAndClearROIs.ijm) allows to check manually all the detected ROIs and to keep only the correct ones. 
-        It shows each event (point ROI) detected by deXtrusion as a pop-up window centered temporally and spatially around the event.
-        The user is asked wether the detection is correct (if there is an event in the current window) by pressing `y` or `n`.
-        If yes, the ROI is kept, else it will be removed from the list of ROIs.
-        
-        
-        * [deXtrusion_scoreROIs_Random.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_scoreROIs_Random.ijm) allows to score manually the precision of the detected events.
-        The macro will open randomly a given number of ROIs, and show a window centered temporally and spatially around the event.
-        The user is asked wether the detection is correct (if it contains the event) by pressing `y` or `n`.
-        The macro will output the count of correct and false detections and the precision. 
-        The ROIs file will not be edited and the ROIs left after running this macro should not be saved as it deletes all the ROIs explored to be sure not to draw them twice.
-        
-        * [deXtrusion_overlayProbabilityMaps.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) allows to visualize the probability maps together with the original image.
-        The user is asked for the original image to visualize and will open the probability maps in the `results` folder where they should be saved by default.
-        The directory to look in can be changed in the macro. 
-        
-        * [deXtrusion_showROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) displays the original movie (chosen by the user) and the ROI file found in the `results` folder. 
-        The location of the ROI file can be changed in the macro by changing the `resfold` parameter and the event to show (by default extrusion) can be changed in the `type` parameter.
-        
-        * [deXtrusion_subsetMovieAndRois.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_subsetMovieAndRois.ijm) save a temporal subset of a movie, and keep only the corresponding ROIs. 
-        
-        
-        ## Jupyter notebooks
-        We provide in this repository several jupyter notebooks to run, train/retrain, evaluate DeXtrusion. 
-        * [detectEventsOnMovie.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/detectEventsOnMovie.ipynb) allows you to run DeXtrusion with the graphical interaface to choose the parameters. 
-        * [deXtrusion_TrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_TrainNetwork.ipynb) to train a new DeXNet network with your own data (or using our data publicly available, see [data section](#Data)).
-        * [deXtrusion_RetrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_RetrainNetwork.ipynb) to retrain an already trained neural network with new data.
-        * [deXtrusion_CompareRois.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_CompareRois.ipynb) to compare two ROIs files (manual detection vs DeXtrusion detection) and gives the score. It can also generate ROIs files of the false detection (false positives and/or false negatives).
-        * [deXtrusion_testClassification_OnWindows.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_testClassification_OnWindows.ipynb): run the trained neural network (DeXNet) on test data on generated windows, and print the resulting confusion matrix of the classification (DeXtrusion classification compared to the manual classification).
-        
-        #### Notebooks usage
-        * If you have Jupyter installed on your computer, to add your virtual environment to the environment Jupyter can see:
-        ```
-        ipython kernel install --user --name=dextrusionenv
-        ```
-        You can refer to this [tutorial](https://www.geeksforgeeks.org/using-jupyter-notebook-in-virtual-environment/) for instructions on creating virtual environment and using it with jupyter.
-        
-        * You can also install Jupyter Lab or Jupyter notebook in your virtual environment if you don't have it installed in your computer:
-        ```sh
-        pip install jupyterlab
-        jupyter-lab
-        ```
-        Refer to [Jupyter](https://jupyter.org/) webpage for more information.
-        
-        ## References
-        To know more about DeXtrusion, refer to our paper: Villars, Letort et al. 2023.
-        
-        ## License
-        DeXtrusion is distributed open-source under the BSD-3 license, see the license file in this repository.
-        
-        When you use DeXtrusion source code, neural networks or data for your projects, please cite our paper. 
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ![DeXtrusion](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/DeX.png "DeXtrusion") DeXtrusion
+
+DeXtrusion is  a machine learning based python pipeline to detect cell extrusions in epithelial tissues movies. It can also detect cell divisions and SOPs, and can easily be trained to detect other dynamic events. 
+
+This repository contains the code source of the python DeXtrusion library, the trained neural networks (ready to use) with Jupyter notebooks to run, train or retrain DeXtrusion networks, and Fiji macros for visualization/analysis of the results.
+
+* [Presentation](#presentation)
+* [Installation](#installation)
+* [Usage](#usage)
+* [Data](#data)
+* [DeXtrusion networks](#dexnets-dextrusion-neural-networks)
+* [Fiji macros](#fiji-macros)
+* [Jupyter notebooks](#jupyter-notebooks)
+* [References](#references)
+
+## Presentation
+DeXtrusion takes as input a movie of an epithelium and outputs the **spatio-temporal location of cell extrusion events** or other event as cell divisions. 
+The movie is discretized into small overlapping rolling windows which are individually [classified for event detection](#event-classification) by a trained [neural network](#deXNets-deXtrusion-neural-networks). Results are then put together in event [probability map](#event-probability-map) for the whole movie or as [spatio-temporal points](#event-spot-localization) indicating each event. 
+
+<p align="center">
+![Example extrusion detection](https://gitlab.pasteur.fr/gletort/dextrusion/-/raw/main/images/SequenceExtrusion.png "Extrusion detection example") 
+Example of the detection of an extrusion event (probability map, red).
+</p>
+
+
+### Event classification
+The movie is discretized into small windows that span all the movie in a rolling windows fashion with overlap between the different windows. 
+Each window is classified by a trained neural network as containing or not a cellular event as cell extrusion. The different classes available in the main DeXtrusion network are:
+- No event
+- Cell extrusion/cell death
+- Cell division
+- SOPs
+
+It is easy to add or remove a cellular event to this list, but necessitates to train new neural networks for this. Jupyter notebook is available in this repository to do it.
+
+### Event probability map
+Each window is associated an event probability which allow to generate an events probability map on the whole movie. This probability maps can be refined to precise spatio-temporal spots for each event.
+The results can be visualized by overlaying the initial movie and all the probability maps saved by DeXtrusion in Fiji with the saved by DeXtrusion with the [`deXtrusion_overlayProbabilityMaps.ijm`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) macro.
+
+<p align="center">
+![Example probability maps](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/images/SequenceProbamaps.png?raw=True "Probability map example") 
+</p>
+
+Example of probability maps (green: division, red: extrusion, blue: SOP
+
+### Event spot localization
+An event is visible in the probability map as a volume of connected pixels of high probability. To convert the probability map to a list of event, we place the event localization at the center of each of these high probability volumes.
+Moreover, to reduce false positive detections, the volumes can be thresholded to keep only big enough volume of high enough probability values. 
+The list of spots obtained in this way are saved in ROIS `.zip` file that can be open in Fiji through the `ROIManager` tool. The macro [`deXtrusion_showROIs.ijm`](#https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) allows to directly visualize with Fiji the results saved by DeXtrusion. 
+
+
+## Installation
+DeXtrusion is distributed as a python module, compatible with `python3`. 
+You can install it in a virtual environment to be sure to have the required versions.
+**DeXtrusion** can be installed either manually through the setup file or with pip:
+
+* DeXtrusion can be directly installed via pip. In your python virtual environment, enter: `pip install dextrusion` to install it.
+You should also download the trained neural network [DeXNet](#dexnets-dextrusion-neural-networks) that you want to use from this repository.
+
+* To install manually **DeXtrusion**, clone this github repository, and inside this repository type: `python setup.py install`. 
+If you want to install it in a virtual environment, you should have activated it before.
+It will install all the necessary dependencies.
+
+
+### Detailled installation on Linux (Ubuntu)
+Here's a step by step command lines to run in a Terminal to install DeXtrusion on Linux from scratch. It is creating a new virtual environment on which DeXtrusion will be installed (not necessary but recommended). Tested with `python 3.8`.
+
+* Installation with `pip`
+```sh
+python3 -m venv dextrusenv               ## create a virtual environment with python 3 called dextrusenv (you can choose the name)
+source dextrusenv/bin/activate           ## activate the virtual environment: now python commands will be runned in that environment
+pip install dextrusion                  ## install DeXtrusion, download all the necessary dependencies, can take time
+```
+DeXtrusion is installed and can be runned with:
+
+```sh
+python -m dextrusion 	                  ## run DeXtrusion. Next time to run it again with the same networks, you only have to do this line
+```
+
+DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the DeXNets repository), you have to download and uncompress it. From the command line:
+
+```sh
+mkdir DeXNets							## create directory on which neural networks will be put
+mkdir DeXNets/notum_ExtSOPDiv			## create directory for the neural networks traind with 4 events available in this repository
+cd DeXNets/notum_ExtSOPDiv               ## go inside the desired neural networks directory (here the network trained with 4 events)
+wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv0.zip   ## download the first neural network
+wget https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/DeXNets/notum_ExtSOPDiv/notumExtSOPDiv1.zip   ## download the second neural network
+unzip notumExtSOPDiv0.zip                ## uncompress it. It is now ready to be used
+unzip notumExtSOPDiv1.zip
+cd ../..                                 ## go back to main DeXtrusion directory
+```
+ 
+* You can also clone this repository and install DeXtrusion from the source code `python setup.py install` instead of using pip installation.
+
+
+### Detailled installation on Windows
+You need to have anaconda installed to run python and create a new virtual environment. On the command prompt, write:
+```cmd
+$ C:\ProgramData\Anaconda3\Scripts\Activate     ## activate conda (should be the path of your anaconda installation)
+$ conda create --name dextrusionenv python=3.8  ## to create virtual environment called dextrusionenv
+$ conda activate dextrusionenv                  ## activate the virtual environment that you juste created
+$ pip install dextrusion                        ## install DeXtrusion in it
+$ python -m dextrusion                          ## Run it
+```
+
+### Choose the neural network DeXNets to use
+DeXtrusion needs neural networks to classify each sliding window. To used our trained neural networks (in the [DeXNets repository](./DeXNets)), you have to download and uncompress it. 
+From DeXtrusion user interface, to select a network to run, you have to go inside its uncompressed directory (click on `Browse` and go there). If you want to use several networks together for the detection for better results (see our paper), the networks folders should be placed within the same directory. Go inside that directy with the interface, and it will use all the networks presents in that directory.
+
+## Usage
+
+DeXtrusion can be used directly within python. 
+To run an already trained network and detect cell events, run `python3 -m dextrusion` in your virtual environment. It will open a graphical interface to perform the detection.
+
+We also propose [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks) in this repository, to use dextrusion options. 
+You can find a notebook to perform the detection, train a new neural network, retrain a network or evaluate the performance of the network compared to a manual detection.
+
+
+## Data
+Data used for the training of our neural networks (raw movies with manual anotation of events) are freely available on Zenodo. 
+
+
+## DeXNets: deXtrusion neural networks
+DeXtrusion was trained on E-cadherin tagged drosophilia notum but can be easily adapted to other markers/biological conditions. Retraining of DeXtrusion network may be necessary when images are quite different.
+
+In the `deXNets` folder of this repository, we proposed several trained networks:
+- `notum_Ext`: trained on drosophilia notum movies with only extrusion events
+- `notum_ExtSOP`: trained on drosophilia notum movies with extrusion and SOP events
+- `notum_ExtSOPDiv`: trained on drosophilia notum movies with extrusion, division and SOP events
+- `notum_all`: trained on drosophilia notum movies with extrusion, division and SOP events, on all our annotated data (training and test). Networks to use by default.
+
+Download them and unzip to be ready to use in DeXtrusion.
+
+### Train/retrain a new DeXNet
+If you want to train/retrain a neural network, to add a new event to detect or to improve its performance on new datasets, Jupyter notebooks are proposed in this repository: [Jupyter notebooks](https://gitlab.pasteur.fr/gletort/dextrusion/-/tree/main/jupyter_notebooks). You can just follow step by step the notebook.
+
+If you want to change the architecture of DeXNet, you will have to change it in the `src/dextrusion/Network.py` file. The architecture is defined in the `action_model` function.
+
+
+## Fiji macros
+
+Fiji macros to prepare data for DeXtrusion neural network training or to handle DeXtrusion results are available in the [`Fiji macros`](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/) folder of this repository.
+
+* [deXtrusion_checkAndClearROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_checkAndClearROIs.ijm) allows to check manually all the detected ROIs and to keep only the correct ones. 
+It shows each event (point ROI) detected by deXtrusion as a pop-up window centered temporally and spatially around the event.
+The user is asked wether the detection is correct (if there is an event in the current window) by pressing `y` or `n`.
+If yes, the ROI is kept, else it will be removed from the list of ROIs.
+
+
+* [deXtrusion_scoreROIs_Random.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_scoreROIs_Random.ijm) allows to score manually the precision of the detected events.
+The macro will open randomly a given number of ROIs, and show a window centered temporally and spatially around the event.
+The user is asked wether the detection is correct (if it contains the event) by pressing `y` or `n`.
+The macro will output the count of correct and false detections and the precision. 
+The ROIs file will not be edited and the ROIs left after running this macro should not be saved as it deletes all the ROIs explored to be sure not to draw them twice.
+
+* [deXtrusion_overlayProbabilityMaps.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_overlayProbabilityMaps.ijm) allows to visualize the probability maps together with the original image.
+The user is asked for the original image to visualize and will open the probability maps in the `results` folder where they should be saved by default.
+The directory to look in can be changed in the macro. 
+
+* [deXtrusion_showROIs.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_showROIs.ijm) displays the original movie (chosen by the user) and the ROI file found in the `results` folder. 
+The location of the ROI file can be changed in the macro by changing the `resfold` parameter and the event to show (by default extrusion) can be changed in the `type` parameter.
+
+* [deXtrusion_subsetMovieAndRois.ijm](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/ijmacros/deXtrusion_subsetMovieAndRois.ijm) save a temporal subset of a movie, and keep only the corresponding ROIs. 
+
+
+## Jupyter notebooks
+We provide in this repository several jupyter notebooks to run, train/retrain, evaluate DeXtrusion. 
+* [detectEventsOnMovie.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/detectEventsOnMovie.ipynb) allows you to run DeXtrusion with the graphical interaface to choose the parameters. 
+* [deXtrusion_TrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_TrainNetwork.ipynb) to train a new DeXNet network with your own data (or using our data publicly available, see [data section](#Data)).
+* [deXtrusion_RetrainNetwork.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_RetrainNetwork.ipynb) to retrain an already trained neural network with new data.
+* [deXtrusion_CompareRois.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_CompareRois.ipynb) to compare two ROIs files (manual detection vs DeXtrusion detection) and gives the score. It can also generate ROIs files of the false detection (false positives and/or false negatives).
+* [deXtrusion_testClassification_OnWindows.ipynb](https://gitlab.pasteur.fr/gletort/dextrusion/-/blob/main/jupyter_notebooks/deXtrusion_testClassification_OnWindows.ipynb): run the trained neural network (DeXNet) on test data on generated windows, and print the resulting confusion matrix of the classification (DeXtrusion classification compared to the manual classification).
+
+#### Notebooks usage
+* If you have Jupyter installed on your computer, to add your virtual environment to the environment Jupyter can see:
+```
+ipython kernel install --user --name=dextrusionenv
+```
+You can refer to this [tutorial](https://www.geeksforgeeks.org/using-jupyter-notebook-in-virtual-environment/) for instructions on creating virtual environment and using it with jupyter.
+
+* You can also install Jupyter Lab or Jupyter notebook in your virtual environment if you don't have it installed in your computer:
+```sh
+pip install jupyterlab
+jupyter-lab
+```
+Refer to [Jupyter](https://jupyter.org/) webpage for more information.
+
+## References
+To know more about DeXtrusion, refer to our paper: Villars, Letort et al. 2023.
+
+## License
+DeXtrusion is distributed open-source under the BSD-3 license, see the license file in this repository.
+
+When you use DeXtrusion source code, neural networks or data for your projects, please cite our paper. 
+
```

