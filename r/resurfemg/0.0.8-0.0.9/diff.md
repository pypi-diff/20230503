# Comparing `tmp/resurfemg-0.0.8-py3-none-any.whl.zip` & `tmp/resurfemg-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 34031 bytes, number of entries: 13
--rw-r--r--  2.0 unx       24 b- defN 23-Feb-12 18:07 resurfemg/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 23-Feb-12 18:07 resurfemg/__main__.py
--rw-r--r--  2.0 unx     5196 b- defN 23-Feb-12 18:07 resurfemg/cli.py
--rw-r--r--  2.0 unx    11004 b- defN 23-Feb-12 18:07 resurfemg/config.py
--rw-r--r--  2.0 unx     4382 b- defN 23-Feb-12 18:07 resurfemg/converter_functions.py
--rw-r--r--  2.0 unx    48950 b- defN 23-Feb-12 18:07 resurfemg/helper_functions.py
--rw-r--r--  2.0 unx     2476 b- defN 23-Feb-12 18:07 resurfemg/ml.py
--rw-r--r--  2.0 unx    17071 b- defN 23-Feb-12 18:07 resurfemg/multi_lead_type.py
--rw-r--r--  2.0 unx     9450 b- defN 23-Feb-12 18:07 resurfemg/tmsisdk_lite.py
--rw-r--r--  2.0 unx    15189 b- defN 23-Feb-12 18:07 resurfemg-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-12 18:07 resurfemg-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-12 18:07 resurfemg-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1025 b- defN 23-Feb-12 18:07 resurfemg-0.0.8.dist-info/RECORD
-13 files, 114959 bytes uncompressed, 32337 bytes compressed:  71.9%
+Zip file size: 38309 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       24 b- defN 23-May-03 12:15 resurfemg/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 23-May-03 12:15 resurfemg/__main__.py
+-rw-r--r--  2.0 unx     5823 b- defN 23-May-03 12:15 resurfemg/cli.py
+-rw-r--r--  2.0 unx    11004 b- defN 23-May-03 12:15 resurfemg/config.py
+-rw-r--r--  2.0 unx     6306 b- defN 23-May-03 12:15 resurfemg/converter_functions.py
+-rw-r--r--  2.0 unx    62540 b- defN 23-May-03 12:15 resurfemg/helper_functions.py
+-rw-r--r--  2.0 unx     2476 b- defN 23-May-03 12:15 resurfemg/ml.py
+-rw-r--r--  2.0 unx    17071 b- defN 23-May-03 12:15 resurfemg/multi_lead_type.py
+-rw-r--r--  2.0 unx     9450 b- defN 23-May-03 12:15 resurfemg/tmsisdk_lite.py
+-rw-r--r--  2.0 unx    16131 b- defN 23-May-03 12:15 resurfemg-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 12:15 resurfemg-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-03 12:15 resurfemg-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1025 b- defN 23-May-03 12:15 resurfemg-0.0.9.dist-info/RECORD
+13 files, 132042 bytes uncompressed, 36615 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: resurfemg/multi_lead_type.py
 Comment: 
 
 Filename: resurfemg/tmsisdk_lite.py
 Comment: 
 
-Filename: resurfemg-0.0.8.dist-info/METADATA
+Filename: resurfemg-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: resurfemg-0.0.8.dist-info/WHEEL
+Filename: resurfemg-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: resurfemg-0.0.8.dist-info/top_level.txt
+Filename: resurfemg-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: resurfemg-0.0.8.dist-info/RECORD
+Filename: resurfemg-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## resurfemg/cli.py

```diff
@@ -13,14 +13,15 @@
 
 from argparse import ArgumentParser
 
 from .multi_lead_type import preprocess
 from .ml import applu_model
 from .config import Config
 from .config import make_realistic_syn_emg_cli
+from .converter_functions import save_j_as_np
 
 
 def common(parser):
     """
     This function defines some arguments that can be called from any command
     line function to be defined.
     """
@@ -103,14 +104,26 @@
         '--number',
         default=1,
         help='''
         Number of synthetic EMG to be made.
         '''
     )
 
+    save_np = subparsers.add_parser('save_np')
+    save_np.set_defaults(action='save_np')
+    common(save_np)
+    # save_np.add_argument(
+    #     '-N',
+    #     '--number',
+    #     default=1,
+    #     help='''
+    #     Number of synthetic EMG to be made.
+    #     '''
+    # )
+
     ml = subparsers.add_parser('ml')
     ml.set_defaults(action='ml')
     common(ml)
 
     ml.add_argument(
         '-V',
         '--verbose',
@@ -172,14 +185,25 @@
                 config.get_directory('preprocessed', parsed.output),
                 parsed.force,
             )
         except Exception as e:
             logging.exception(e)
             return 1
 
+    if parsed.action == 'save_np':
+        try:
+
+            save_j_as_np(
+                config.get_directory('data', parsed.input),
+                config.get_directory('made', parsed.output),
+            )
+        except Exception as e:
+            logging.exception(e)
+            return 1
+
     if parsed.action == 'synth':
         try:
 
             make_realistic_syn_emg_cli(
                 config.get_directory('data', parsed.input),
                 parsed.number,
                 config.get_directory('made', parsed.output),
```

## resurfemg/converter_functions.py

```diff
@@ -4,14 +4,16 @@
 
 This file contains functions to work with various EMG file types
 from various hardware/software combinations, and convert them down to
 an array that can be further processed with helper_functions or other modules.
 """
 
 
+import os
+import glob
 import pandas as pd
 import numpy as np
 import scipy.io as sio
 from resurfemg.tmsisdk_lite import Poly5Reader
 
 
 def poly5unpad(to_be_read):
@@ -32,15 +34,15 @@
 
 
 def matlab5_jkmn_to_array(file_name):
     """
     This file reads matlab5 files as produced in the Jonkman
     laboratory, on the Biopac system
     and returns arrays in the format and shape
-    our functions,those in helper_functions work on.
+    our functions, those in helper_functions work on.
 
     :param file_name: Filename of matlab5 files
     :type file_name: str
 
     :returns: arrayed
     :rtype: ~numpy.ndarray
     """
@@ -72,14 +74,79 @@
         .set_axis([f'lead.{i+1}' for i in range(file.shape[1])], axis=1)
     )
     arrayed = np.rot90(new_df)
     arrayed = np.flipud(arrayed)
     return arrayed
 
 
+def save_j_as_np(
+    file_directory,
+    made,
+    force=False
+):
+    """
+    This is an implementation of the save_j_as_np_single function in the
+    same module which can be run from the commmand-line cli module.
+
+    :param file_directory: the directory with EMG files
+    :type file_directory: str
+    :param processed: the output directory
+    :type processed: str
+    :param our_chosen_leads: the leads selected for the pipeline to run over
+    :type our_chosen_leads: list
+
+    """
+    file_directory_list = glob.glob(
+        os.path.join(file_directory, '**/*.csv'),
+        recursive=True,
+    )
+    for file_name in file_directory_list:
+        file = pd.read_csv(file_name)
+        new_df = (
+            file.T.reset_index().T.reset_index(drop=True)
+            .set_axis([f'lead.{i+1}' for i in range(file.shape[1])], axis=1)
+        )
+        arrayed = np.rot90(new_df)
+        arrayed = np.flipud(arrayed)
+
+        rel_fname = os.path.relpath(file_name, file_directory)
+        out_fname = os.path.join(made, rel_fname)
+        # check the directory does not exist
+        if not (os.path.exists(made)):
+            # create the directory you want to save to
+            os.mkdir(made)
+
+        np.save(out_fname, arrayed)
+
+
+def save_j_as_np_single(file_name):
+    """
+    This function takes a file in csv format
+    where teh sequence is top to bottom
+    and changes it
+    into the shape the library functions work on,
+    then saves it as a numpy file
+
+    :param file_name: Filename of csv files
+    :type file_name: str
+
+    :returns: arrayed
+    :rtype: ~numpy.ndarray
+    """
+    file = pd.read_csv(file_name)
+    new_df = (
+        file.T.reset_index().T.reset_index(drop=True)
+        .set_axis([f'lead.{i+1}' for i in range(file.shape[1])], axis=1)
+    )
+    arrayed = np.rot90(new_df)
+    arrayed = np.flipud(arrayed)
+    np.save(file_name, arrayed)
+    return arrayed
+
+
 def poly_dvrman(file_name):
     """
     This is a function to read in Duiverman type Poly5 files,
     which has 18 layers/pseudo-leads,
     and return an array of the twelve  unprocessed leads
     for further pre-processing. The leads eliminated
     were RMS calculated on other leads (leads 6-12).
@@ -122,15 +189,15 @@
     arrayed = np.flipud(arrayed)
     return arrayed
 
 
 def dvrmn_csv_freq_find(file_name):
     """
     This is means to extract the frequency of a Duiverman
-    type csv of emg. Note this data may be resampled down by a
+    type csv of EMG. Note this data may be resampled down by a
     factor of 10.
 
     :param file_name: Filename of csv file
     :type file_name: str
 
     :returns: freq
     :rtype: int
```

## resurfemg/helper_functions.py

```diff
@@ -1,42 +1,48 @@
 """
-Copyright 2022 Netherlands eScience Center and UTwente
+Copyright 2022 Netherlands eScience Center and University of Twente
 Licensed under the Apache License, version 2.0. See LICENSE for details.
 
 This file contains functions to work with various EMG arrays
 and other types of data arrays e.g. ventilator signals.
 
 """
 
+
 import collections
 from collections import namedtuple
 import math
+import warnings
+import time
 from math import log, e
 import copy
 import scipy
 from scipy import signal
 from scipy.fft import fft, fftfreq
 from scipy.signal import find_peaks
 from scipy.signal import savgol_filter
 from scipy.signal import butter, lfilter
+from scipy.stats import entropy
 import matplotlib.pyplot as plt
 import numpy as np
 from sklearn.decomposition import FastICA
 import textdistance
 import pandas as pd
 import logging
 
 
 class Range(namedtuple('RangeBase', 'start,end')):
+
     """Utility class for working with ranges (intervals).
 
     :ivar start: Start of the range
     :type start: ~number.Number
     :ivar end: End of the range
     :type end: ~number.Number
+
     """
 
     def intersects(self, other):
         """Returns :code:`True` if this range intersects :code:`other` range.
 
         :param other: Another range to compare this one to
         :type other: ~resurfemg.helper_functions.Range
@@ -70,15 +76,15 @@
         :rtype: slice
         """
         return slice(*map(int, self))   # maps whole tuple set
 
 
 def emg_bandpass_butter(data_emg, low_pass, high_pass):
     """The parameter taken in here is the Poly5 file. Output is
-    the emg after a bandpass as made here.
+    the EMG after a bandpass as made here.
 
     :param data_emg: Poly5 file with the samples to work over
     :type data_emg: ~TMSiSDK.file_readers.Poly5Reader
     :param low_pass: The number to cut off :code:`frequenciesabove`
     :type low_pass: int
     :param high_pass: The number to cut off :code:`frequenceisbelow`
     :type high_pass: int
@@ -89,30 +95,30 @@
     sos = signal.butter(
         3,
         [low_pass, high_pass],
         'bandpass',
         fs=data_emg.sample_rate,
         output='sos',
     )
-    # sos (output parameter)is second order section  -> "stabilizes" ?
+    # sos (output parameter) is second order section  -> "stabilizes" ?
     emg_filtered = signal.sosfiltfilt(sos, data_emg.samples)
     return emg_filtered
 
 
 def emg_bandpass_butter_sample(
     data_emg_samp,
     low_pass,
     high_pass,
     sample_rate,
     output='sos'
 ):
     """The paramemter taken in here is the Poly5 file.  Output is the
     EMG after a bandpass as made here.
 
-    :param data_emg_samp: The array in the poly5 or other sample
+    :param data_emg_samp: The array in the Poly5 or other sample
     :type data_emg_samp: ~numpy.ndarray
     :param low_pass: The number to cut off :code:`frequenciesabove`
     :type low_pass: int
     :param high_pass: The number to cut off :code:`frequenceisbelow`
     :type high_pass: int
     :param sample_rate: The number of samples per second i.e. Hertz
     :type sample_rate: int
@@ -135,15 +141,15 @@
 
 
 def bad_end_cutter(data_emg, percent_to_cut=7, tolerance_percent=10):
     """This algorithm takes the end off of EMGs where the end is
     radically altered, or if not radically altered cuts the last 10
     values but returns only the array, not an altered Poly5.
 
-    :param data_emg: A poly5
+    :param data_emg: A Poly5
     :type data_emg: ~TMSiSDK.file_readers.Poly5Reader
     :param percent_to_cut: Percentage to look at on the end
     :type percent_to_cut: int
     :param tolerance_percent: Percent variation tolerance to allow without
         cutting
     :type tolerance_percent: int
 
@@ -229,15 +235,15 @@
 
 
 def bad_end_cutter_better(data_emg, percent_to_cut=7, tolerance_percent=10):
     """This algorithm takes the end off of EMGs where the end is
     radically altered, or if not radically altered cuts the last 10
     values but returns only the array not an altered Poly5.
 
-    :param data_emg: A poly5
+    :param data_emg: A Poly5
     :type data_emg: ~TMSiSDK.file_readers.Poly5Reader
     :param percent_to_cut: Percentage to look at on the end
     :type percent_to_cut: int
     :param tolerance_percent: Percentage variation to allow without cut
     :type tolerance_percent: int
 
     :returns: The cut EMG sample data
@@ -267,23 +273,23 @@
 
     return sample_cut
 
 
 def notch_filter(sample, sample_frequ, freq_to_pull, quality_factor_q):
     """This is a filter designed to take out a specific frequency.  In
     the EU in some data electrical cords can interfere at around 50
-    hertz.  In some other locations the interference is at 60 Hertz.
+    Hertz.  In some other locations the interference is at 60 Hertz.
     The specificities of a local power grid may neccesitate notch
     filtering.
 
     :param sample: Percentage variation tolerance to allow without cutting
     :type sample: int
     :param sample_frequ: The frequency at which the sample was captured
     :type sample_frequ: int
-    :param freq_to_pull: The frequency you desire to remove from teh signal
+    :param freq_to_pull: The frequency you desire to remove from the signal
     :type freq_to_pull: int
     :param quality_factor_q: How high the quality of the removal is
     :type quality_factor_q: int
 
     :return: The filterered sample data
     :rtype: ~numpy.ndarray
 
@@ -298,15 +304,15 @@
     # make the output signal
     output_signal = signal.filtfilt(b_notch, a_notch, sample)
     return output_signal
 
 
 def show_my_power_spectrum(sample, sample_rate, upper_window):
     """This function plots a power spectrum of the frequencies
-    comtained in an emg based on a fourier transform.  It does not
+    comtained in an EMG based on a Fourier transform.  It does not
     return the graph, rather the values but plots the graph before it
     return.  Sample should be one single row (1-dimensional array.)
 
     :param sample: The sample array
     :type sample: ~numpy.ndarray
     :param sample_rate: Number of samples per second
     :type sample_rate: int
@@ -326,15 +332,15 @@
 
     plt.plot(xf[idx], yf[idx])
     plt.show()
     return yf, xf
 
 
 def emg_highpass_butter(data_emg, cut_above, sample_rate):
-    """The paramemter taken in here is the Poly5 file's samples or
+    """The parameter taken in here is the Poly5 file's samples or
     another array.  Output is the EMG after a bandpass as made here.
 
     :param data_emg: Samples from the EMG
     :type data_emg: ~numpy.ndarray
     :param cut_above: The number to cut off :code:`frequenceisbelow`
     :type cut_above: int
     :param sample_rate: The number of samples per second i.e. Hertz
@@ -347,20 +353,20 @@
     # sos (output parameter)is second order section  -> "stabilizes" ?
     emg_filtered = signal.sosfiltfilt(sos, data_emg)
     return emg_filtered
 
 
 def naive_rolling_rms(x, N):
     """This function computes a root mean squared envelope over an
-    array :code:`x`.  To do this it uses number of sample values
+    array :code:`x`. To do this it uses number of sample values
     :code:`N`.
 
     :param x: Samples from the EMG
     :type x: ~numpy.ndarray
-    :param N: Legnth of the sample use as window for function
+    :param N: Length of the sample use as window for function
     :type N: int
 
     :returns: The root-mean-squared EMG sample data
     :rtype: ~numpy.ndarray
     """
     xc = np.cumsum(abs(x)**2)
     emg_rms = np.sqrt((xc[N:] - xc[:-N])/N)
@@ -406,16 +412,16 @@
         else:
             i = 1
         array_list.append(i)
     return array_list
 
 
 def compute_ICA_two_comp(emg_samples):
-    """A function that performs an independant component analysis
-    (ICA) meant for EMG data that includes stacked three arrays.
+    """A function that performs an independent component analysis
+    (ICA) meant for EMG data that includes three stacked arrays.
 
     :param emg_samples: Original signal array with three layers
     :type emg_samples: ~numpy.ndarray
 
     :returns: Two arrays of independent components (ECG-like and EMG)
     :rtype: ~numpy.ndarray
     """
@@ -498,15 +504,15 @@
     # the absolute value is used, because the ICA decomposition might
     # produce a component with negative peaks. In this case
     # the signals will be maximally negatively correlated
 
     corr_matrix = abs(np.corrcoef(corr_tuple))
 
     # get the component with the lowest correlation to ECG
-    # the matriz is symmetric, so we can check just the first row
+    # the matrix is symmetric, so we can check just the first row
     # the first coefficient is the autocorrelation of the ECG lead,
     # so we can check row 1 and 2
 
     lowest_index = np.argmin(corr_matrix[0][1:])
     emg_component = components_tuple[lowest_index]
 
     return emg_component
@@ -530,15 +536,15 @@
     """
     c0 = components_tuple[0]
     c1 = components_tuple[1]
     corr_tuple = np.row_stack((ecg_lead, c0, c1))
     corr_matrix = abs(np.corrcoef(corr_tuple))
 
     # get the component with the highest correlation to ECG
-    # the matriz is symmetric, so we can check just the first row
+    # the matrix is symmetric, so we can check just the first row
     # the first coefficient is the autocorrelation of the ECG lead,
     # so we can check row 1 and 2
 
     hi_index = np.argmax(corr_matrix[0][1:])
     ecg_component = components_tuple[hi_index]
 
     return ecg_component
@@ -547,15 +553,15 @@
 def working_pipeline_exp(our_chosen_file):
     """This function is legacy.
     It produces a filtered respiratory EMG signal from a
     3 lead sEMG file. A better
     option is a corresponding function in multi_lead_type
     The inputs are :code:`our_chosen_file` which we
     give the function as a string of filename.  The output is the
-    processed EMG signal filtered and seperated from ecg components.
+    processed EMG signal filtered and seperated from ECG components.
     The algorithm to pick out the EMG here is by having
     more peaks.
 
     :param our_chosen_file: Poly5 file
     :type our_chosen_file: ~TMSiSDK.file_readers.Poly5Reader
 
     :returns: final_envelope_a
@@ -577,37 +583,37 @@
     re_cut_file_data = bad_end_cutter_for_samples(
         bd_filtered_file_data,
         percent_to_cut=3,
         tolerance_percent=5,
     )
     # do ICA
     components = compute_ICA_two_comp(re_cut_file_data)
-    #  pick components with more peaj
+    #  pick components with more peak
     emg = pick_more_peaks_array(components)
     # now process it in final steps
     abs_values = abs(emg)
     final_envelope_d = emg_highpass_butter(abs_values, 150, 2048)
     final_envelope_a = naive_rolling_rms(final_envelope_d, 300)
 
     return final_envelope_a
 
 
 def working_pipeline_pre_ml(our_chosen_samples, picker='heart'):
     """
     This is a pipeline to pre-process
-    an array of specific fixed dimenstions
+    an array of specific fixed dimensions
     i.e. a three lead array into an EMG singal,
     the function is legacy code, and most
     processsing should be done with
     :code:`multi_lead_type.working_pipeline_pre_ml_multi`
     or :code:`multi_lead_type.working_pipeline_pre_ml_multi`
 
     :param our_chosen_samples: the read EMG file arrays
     :type our_chosen_samples: ~numpy.ndarray
-    :param picker: the picking strategy for independant components
+    :param picker: the picking strategy for independent components
     :type picker: str
 
     :returns: final_envelope_a
     :rtype: ~numpy.ndarray
     """
     cut_file_data = bad_end_cutter_for_samples(
         our_chosen_samples,
@@ -641,72 +647,91 @@
     abs_values = abs(emg)
     final_envelope_d = emg_highpass_butter(abs_values, 150, 2048)
 
     return final_envelope_d
 
 
 def slices_slider(array_sample, slice_len):
-    """This function produces continous sequential slices over an
-    array of a certain legnth.  The inputs are the following -
+    """This function produces continuous sequential slices over an
+    array of a certain length.  The inputs are the following -
     :code:`array_sample`, the signal and :code:`slice_len` - the
     window which you wish to slide with.  The function yields, does
     not return these slices.
 
     :param array_sample: array containing the signal
     :type array_sample: ~numpy.ndarray
-    :param slice_len: the legnth of window on the array
+    :param slice_len: the length of window on the array
     :type slice_len: int
 
     :returns: Actually yields, no return
     :rtype: ~numpy.ndarray
     """
     for i in range(len(array_sample) - slice_len + 1):
         yield array_sample[i:i + slice_len]
 
 
 def slices_jump_slider(array_sample, slice_len, jump):
     """
-    This function produces continous sequential slices over an
-    array of a certain legnth spaced out by a 'jump'.
+    This function produces continuous sequential slices over an
+    array of a certain length spaced out by a 'jump'.
     The function yields, does
     not return these slices.
 
     :param array_sample: array containing the signal
     :type array_sample: ~numpy.ndarray
-    :param slice_len: the legnth of window on the array
+    :param slice_len: the length of window on the array
     :type slice_len: int
-    :param jump: the amount by which the winow is moved at iteration
+    :param jump: the amount by which the window is moved at iteration
     :type jump: int
 
     :returns: Actually yields, no return
     :rtype: ~numpy.ndarray
 
     """
     for i in range(len(array_sample) - (slice_len)):
         yield array_sample[(jump*i):((jump*i) + slice_len)]
 
 
 def entropical(sig):
-    """This function computes a certain type of entropy of a series
-    signal array.  Input is sig, the signal, and output is an array of
-    entropy measurements. The function can be used inside a generator
-    to read over slices.
+    """This function computes something close to certain type of entropy
+    of a series signal array.  Input is sig, the signal, and output is an
+    array of entropy measurements. The function can be used inside a generator
+    to read over slices. Note it is not a true entropy, and works best with
+    very small numbers.
 
     :param sig: array containin the signal
     :type sig: ~numpy.ndarray
 
-    :returns: A number expressing the entropy using math.log w/base 2
+    :returns: number for an entropy-like signal using math.log w/base 2
     :rtype: float
 
     """
     probabilit = [n_x/len(sig) for x, n_x in collections.Counter(sig).items()]
     e_x = [-p_x*math.log(p_x, 2) for p_x in probabilit]
     return sum(e_x)
 
 
+def entropy_scipy(sli, base=None):
+    """
+    This function wraps scipy.stats entropy  (which is a Shannon entropy)
+    for use in the resurfemg library, it can be used in a slice iterator
+    as a drop-in substitute for the hf.entropical but it is a true entropy.
+
+    :param sli: array
+    :type sli: ~numpy.ndarray
+
+    :returns: entropy_count
+    :rtype: float
+    """
+
+    value, counts = np.unique(sli, return_counts=True)
+    entropy_count = entropy(counts/len(counts), base=base)
+    return entropy_count
+
+
 def compute_power_loss(
     original_signal,
     original_signal_sampling_frequency,
     processed_signal,
     processed_signal_sampling_frequency
 ):
     """This function computes the percentage of power loss after the
@@ -774,17 +799,17 @@
     single_filtered_array, start=None, end=None, smooth=100
 ):
     """
     This is an adaptive smoothing a series that overvalues closer numbers.
 
     :param single_filtered_array: Array.
     :type single_filtered_array: ~numpy.ndarray
-    :param start: The number on samples to work from
+    :param start: The number of samples to work from
     :type start: int
-    :param end: The number on samples to work until
+    :param end: The number of samples to work until
     :type end: int
     :param smooth: The number of samples to work over
     :type smooth: int
 
     :return: tuple of arrays
     :rtype: tuple
     """
@@ -811,17 +836,17 @@
     """This is the same as smooth for baseline, but we also get an
     overlay 0 or 1 mask tagging the baseline.
 
     :param my_own_array: Array
     :type  my_own_array: ~numpy.ndarray
     :param threshold: Number where to cut the mask for overlay
     :type threshold: int
-    :param start: The number on samples to work from
+    :param start: The number of samples to work from
     :type start: int
-    :param end: The number on samples to work until
+    :param end: The number of samples to work until
     :type end: int
     :param smooth: The number of samples to work over
     :type smooth: int
 
     :return: tuple of arrays
     :rtype: tuple
     """
@@ -916,41 +941,41 @@
     :param rsignal2: Binary signal 2
     :type rsignal2: ~numpy.ndarray
 
     :returns: Raw overlap percent
     :rtype: float
     """
     if len(signal1) != len(signal2):
-        print('Warning: legnth of arrays is not matched')
+        print('Warning: length of arrays is not matched')
         longer_signal_len = np.max([len(signal1), len(signal2)])
     else:
         longer_signal_len = len(signal1)
 
     raw_overlap_percent = sum(
         signal1.astype(int) & signal2.astype(int)
     ) / longer_signal_len
     return raw_overlap_percent
 
 
 def relative_levenshtein(signal1, signal2):
     """
     Here we take two arrays, and create an edit distance based on Levelshtien
     edit distance The distance is then normalized between 0 and one regardless
-    of signal legnth
+    of signal length
 
     """
     signal1_list = []
     signal2_list = []
     for element in signal1:
         signal1_list.append(element)
     for element in signal2:
         signal2_list.append(element)
     distance = textdistance.levenshtein.similarity(signal1_list, signal2_list)
     if len(signal1) != len(signal2):
-        print('Warning: legnth of arrays is not matched')
+        print('Warning: length of arrays is not matched')
     longer_signal_len = np.max([len(signal1), len(signal2)])
     normalized_distance = distance / longer_signal_len
     return normalized_distance
 
 
 def full_rolling_rms(x, N):
     """This function computes a root mean squared envelope over an
@@ -1120,15 +1145,15 @@
     """
     Takes a 1d signal array, and extracts 'high'envelope,
     then makes high envelope, based on connecting peaks
     dmax: int, size of chunks,
 
     :param our_signal: 1d signal array usually of emg
     :type our_signal: ~numpy.ndarray
-    :param dmax: legnth of chunk to look for local max in
+    :param dmax: length of chunk to look for local max in
     :type dmax: int
 
     :returns: src_signal_gated, the gated result
     :rtype: ~numpy.ndarray
     """
     # locals max is lmax
     lmax = (np.diff(np.sign(np.diff(our_signal))) < 0).nonzero()[0] + 1
@@ -1228,15 +1253,15 @@
 
 def times_under_curve(
     array,
     start_index,
     end_index,
 ):
     """
-    This function is meant to calculate the legnth of time to peak in
+    This function is meant to calculate the length of time to peak in
     an absolute and relative sense
 
     :param array: an array e.g. single lead EMG recording
     :type array: np.array
     :param start_index: which index number the breath starts on
     :type start_index: int
     :param end_index: which index number the breath ends on
@@ -1253,36 +1278,43 @@
     return times
 
 
 def pseudo_slope(
     array,
     start_index,
     end_index,
+    smoothing=True,
 ):
     """
     This is a function to get the shape/slope of the take-off angle
     of the resp. surface EMG signal, however we are returning values of
     mV divided by samples (in abs values), not a true slope
     and the number will depend on sampling rate
-    and pre-processing, therefore it is reccomended
+    and pre-processing, therefore it is recommended
     only to compare across the same single sample run
 
     :param array: an array e.g. single lead EMG recording
     :type array: np.array
     :param start_index: which index number the breath starts on
     :type start_index: int
     :param end_index: which index number the breath ends on
     :type end_index: int
+    :param smoothing: smoothing which can or can not run before calculations
+    :type smoothing: bool
+
     :returns: pseudoslope
     :rtype: float
     """
     breath_arc = array[start_index:end_index]
     pos_arc = abs(breath_arc)
-    smoothed_breath = running_smoother(pos_arc)
-    abs_time = smoothed_breath.argmax()
+    if smoothing:
+        smoothed_breath = running_smoother(pos_arc)
+        abs_time = smoothed_breath.argmax()
+    else:
+        abs_time = pos_arc.argmax()
     abs_height = pos_arc[abs_time]
     pseudoslope = abs_height / abs_time
     return pseudoslope
 
 
 def area_under_curve(
     array,
@@ -1290,19 +1322,19 @@
     end_index,
     end_curve=70,
     smooth_algorithm='none',
 ):
     """
     This algorithm should be applied to breaths longer than 60 values
     on an index. The mid_savgol assumes a parabolic fit. It is
-    reccomended to test a smoothing algorithm first, apply,
+    recommended to test a smoothing algorithm first, apply,
     then run the area_under the curve with none for smooth_algortihm.
     If a cutoff of the curve before it hits bottom is desired then a value
     other than zero must be in end_curve variable. This variable
-    should be written from 0 to 100 for the perfentage of the max value
+    should be written from 0 to 100 for the percentage of the max value
     at which to cut off after the peak.
     :param array: an array e.g. single lead EMG recording
     :type array: np.array
     :param start_index: which index number the breath starts on
     :type start_index: int
     :param end_index: which index number the breath ends on
     :type end_index: int
@@ -1357,62 +1389,75 @@
     array,
     start_index,
     end_index,
     smooth_algorithm='none'
 ):
     """
     This algorithm locates peaks on a breath. It is assumed
-    an array of absolute values for electrophysiological signal
-    will be used as the array. Te mid_savgol assumes a parabolic fit.
-    It is reccomended to test a smoothing
+    an array of absolute values for electrophysiological signals
+    will be used as the array. The mid_savgol assumes a parabolic fit.
+    The convy option uses a convolution to essentially
+    smooth values with those around it as in function
+    running_smoother() in the same module.
+    It is recommended to test a smoothing
     algorithm first, apply, then run the find peak algorithm.
 
     :param array: an array e.g. single lead EMG recording
     :type array: np.array
     :param start_index: which index number the breath starts on
     :type start_index: int
     :param end_index: which index number the breath ends on
     :type end_index: int
-    :param smooth_algorithm: algorithm for smoothing (none or 'mid-savgol')
+    :param smooth_algorithm: algorithm for smoothing (none or
+        'mid-savgol' or 'convy')
     :type smooth_algorithm: str
 
-    :returns: index of max point, value at max point
+    :returns: index of max point, value at max point, smoothed value
     :rtype: tuple
     """
     new_array = array[start_index: (end_index+1)]
     if smooth_algorithm == 'mid_savgol':
-        new_array = savgol_filter(
-            new_array, int(len(new_array)),
+        new_array2 = savgol_filter(
+            abs(new_array), int(len(new_array)),
             2,
             deriv=0,
             delta=1.0,
             axis=- 1,
             mode='interp',
             cval=0.0,
         )
-        max_ind = (new_array.argmax())
+        max_ind = (new_array2.argmax())
         max_val = new_array[max_ind]
-    else:
-        max_ind = (new_array.argmax())
+        smooth_max = new_array2[max_ind]
+    elif smooth_algorithm == 'convy':
+        abs_new_array = abs(new_array)
+        new_array2 = running_smoother(abs_new_array)
+        max_ind = (new_array2.argmax())
         max_val = new_array[max_ind]
-    return (max_ind, max_val)
+        smooth_max = new_array2[max_ind]
+    else:
+        abs_new_array = abs(new_array)
+        max_ind = (abs_new_array.argmax())
+        max_val = abs_new_array[max_ind]
+        smooth_max = max_val
+    return (max_ind, max_val, smooth_max)
 
 
 def distance_matrix(array_a, array_b):
     """
     :param array_a: an array of same size as other parameter array
     :type array_a: array or list
     :param array_b: an array of same size as other parameter array
     :type array_b: array or list
 
     :returns: distances
     :rtype: pd.DataFrame
     """
     if len(array_a) != len(array_b):
-        print('Your arrays do not match in legnth, caution!')
+        print('Your arrays do not match in length, caution!')
     array_a_list = array_a.tolist()
     array_b_list = array_b.tolist()
     distance_earthmover = scipy.stats.wasserstein_distance(array_a, array_b)
     distance_edit_distance = textdistance.levenshtein.similarity(
         array_a_list,
         array_b_list,
     )
@@ -1439,15 +1484,15 @@
     return butter(order, cutoff, fs=fs, btype='low', analog=False)
 
 
 def emg_lowpass_butter(array, cutoff, fs, order=5):
     """
     This is a lowpass filter of butterworth design.
 
-    :param array: 1d signal array usually of emg
+    :param array: 1d signal array usually of EMG
     :type array: ~numpy.ndarray
     :param cutoff: frequency above which to filter out
     :type cutoff: int
     :param fs: frequency array sampled at in Hertz
     :type fs: int
     :param order: order of the filter
     :type order: int
@@ -1461,15 +1506,15 @@
 
 
 def find_peaks_in_ecg_signal(ecg_signal, lower_border_percent=50):
     """
     This function assumes you have isolated an ecg-like signal with
     QRS peaks "higher" (or lower) than ST waves.
     In this case it can be applied to return an array of
-    ecg peak locations. NB: This function assumes that the ECG
+    ECG peak locations. NB: This function assumes that the ECG
     signal has already been through a bandpass or low-pass filter
     or has little baseline drift.
 
     :param ecg_signal: frequency array sampled at in Hertz
     :type ecg_signal: ~numpy.ndarray
     :param low_border_percent: percentage max below which no peaks expected
     :type low_border_percent: int
@@ -1481,7 +1526,366 @@
     ecg_signal = abs(ecg_signal)
     max_peak = ecg_signal.max() - ecg_signal.min()
     set_ecg_peaks = find_peaks(
         ecg_signal,
         prominence=(max_peak*lower_border_percent/100, max_peak)
     )
     return set_ecg_peaks
+
+
+def variability_maker(
+        array,
+        segment_size,
+        method='variance',
+        fill_method='avg',
+):
+    """
+    Calculate variability of segments of an array according to a specific
+    method, then interpolate the values back to the original legnth of array
+
+
+    :param array: the input array
+    :type array: ~numpy.ndarray
+
+    :param segment_size: length over which variabilty calculated
+    :type segment_size: int
+
+    :param method: method for calculation i.e. variance or standard deviation
+    :type method: str
+
+    :param fill_method: method to fill missing values at end result array,
+        'avg' will fill with average of last values, 'zeros' fills zeros, and
+        'resample' will resample (not fill) and strech array
+        to the full 'correct' length of the original signal
+    :type method: str
+
+    :returns: variability_values array showing variability over segments
+    :rtype: ~numpy.ndarray
+
+    """
+    variability_values = []
+    if method == 'variance':
+        variability_values = [
+            np.var(array[i:i + segment_size])
+            for i in range(1, len(array) - segment_size)
+        ]
+
+        values_out = np.array(variability_values)
+
+    elif method == 'std':
+        # Calculate the standard deviation of each segment
+        variability_values = [
+            np.std(array[i:i+segment_size])
+            for i in range(0, len(array), segment_size)
+        ]
+        values_out = np.array(variability_values)
+
+    else:
+        print("You did not choose an exisitng method")
+    num_missing_values = len(array) - len(values_out)
+    avg_values_end = np.sum(
+        values_out[(len(values_out) - num_missing_values):]
+        ) \
+        / num_missing_values
+    last_values_avg = np.full(num_missing_values, avg_values_end)
+
+    if fill_method == 'avg':
+        variability_array = np.hstack((values_out, last_values_avg))
+    elif fill_method == 'zeros':
+        variability_array = np.hstack(
+            (values_out, np.zeros(num_missing_values))
+        )
+    elif fill_method == 'resample':
+        variability_array = scipy.signal.resample(values_out, len(array))
+    else:
+        print("You did not choose an exisitng method")
+        variability_array = np.hstack((values_out, last_values_avg))
+
+    return variability_array
+
+
+def rowwise_chebyshev(x, y):
+    return np.max(np.abs(x - y), axis=1)
+
+
+def delay_embedding(data, emb_dim, lag=1):
+    """
+    The following code is adapted from openly licensed code written by
+    Christopher Schölzel in his package nolds
+    (NOnLinear measures for Dynamical Systems).
+    It performs a time-delay embedding of a time series
+
+    :param data: array-like
+    :type data: array
+    :param emb_dim: the embedded dimension
+    :type emb_dim: int
+    :param lag: the lag between elements in the embedded vectors
+    :type lag: int
+
+    :returns: matrix_vectors
+    :rtype: ~nd.array
+    """
+    data = np.asarray(data)
+    min_len = (emb_dim - 1) * lag + 1
+    if len(data) < min_len:
+        msg = "cannot embed data of length {} with embedding dimension {} " \
+            + "and lag {}, minimum required length is {}"
+        raise ValueError(msg.format(len(data), emb_dim, lag, min_len))
+    m = len(data) - min_len + 1
+    indices = np.repeat([np.arange(emb_dim) * lag], m, axis=0)
+    indices += np.arange(m).reshape((m, 1))
+    matrix_vectors = data[indices]
+    return matrix_vectors
+
+
+def sampen(
+        data,
+        emb_dim=2,
+        tolerance=None,
+        dist=rowwise_chebyshev,
+        closed=False,
+):
+    """
+    The following code is adapted from openly licensed code written by
+    Christopher Schölzel in his package
+    nolds (NOnLinear measures for Dynamical Systems).
+    It computes the sample entropy of time sequence data.
+    Returns
+    the sample entropy of the data (negative logarithm of ratio between
+    similar template vectors of length emb_dim + 1 and emb_dim)
+    [c_m, c_m1]:
+    list of two floats: count of similar template vectors of length emb_dim
+    (c_m) and of length emb_dim + 1 (c_m1)
+    [float list, float list]:
+    Lists of lists of the form ``[dists_m, dists_m1]`` containing the
+    distances between template vectors for m (dists_m)
+    and for m + 1 (dists_m1).
+    Reference
+    .. [se_1] J. S. Richman and J. R. Moorman, “Physiological time-series
+    analysis using approximate entropy and sample entropy,”
+    American Journal of Physiology-Heart and Circulatory Physiology,
+    vol. 278, no. 6, pp. H2039-H2049, 2000.
+
+    Kwargs are
+    emb_dim (int):
+    the embedding dimension (length of vectors to compare)
+    tolerance (float):
+    distance threshold for two template vectors to be considered equal
+    (default: 0.2 * std(data) at emb_dim = 2, corrected for
+    dimension effect for other values of emb_dim)
+    dist (function (2d-array, 1d-array) -> 1d-array):
+    distance function used to calculate the distance between template
+    vectors. Sampen is defined using ``rowwise_chebyshev``. You should only
+    use something else, if you are sure that you need it.
+    closed (boolean):
+    if True, will check for vector pairs whose distance is in the closed
+    interval [0, r] (less or equal to r), otherwise the open interval
+    [0, r) (less than r) will be used
+
+    :param data: array-like
+    :type data: array
+    :param emb_dim: the embedded dimension
+    :type emb_dim: int
+    :param tolerance: distance threshold for two template vectors
+    :type tolerance: float
+    :param distance: function to calculate distance
+    :type distance: function
+
+    :returns: saen
+    :rtype: float
+    """
+    data = np.asarray(data)
+
+    if tolerance is None:
+        lint_helper = (0.5627 * np.log(emb_dim) + 1.3334)
+        tolerance = np.std(data, ddof=1) * 0.1164 * lint_helper
+    n = len(data)
+
+    # build matrix of "template vectors"
+    # (all consecutive subsequences of length m)
+    # x0 x1 x2 x3 ... xm-1
+    # x1 x2 x3 x4 ... xm
+    # x2 x3 x4 x5 ... xm+1
+    # ...
+    # x_n-m-1     ... xn-1
+
+    # since we need two of these matrices for m = emb_dim and
+    #  m = emb_dim +1,
+    # we build one that is large enough => shape (emb_dim+1, n-emb_dim)
+
+    # note that we ignore the last possible template vector with
+    #  length emb_dim,
+    # because this vector has no corresponding vector of length m+
+    # 1 and thus does
+    # not count towards the conditional probability
+    # (otherwise first dimension would be n-emb_dim+1 and not n-emb_dim)
+    t_vecs = delay_embedding(np.asarray(data), emb_dim + 1, lag=1)
+    counts = []
+    for m in [emb_dim, emb_dim + 1]:
+        counts.append(0)
+        # get the matrix that we need for the current m
+        t_vecs_m = t_vecs[:n - m + 1, :m]
+        # successively calculate distances between each pair of templ vectrs
+        for i in range(len(t_vecs_m) - 1):
+            dsts = dist(t_vecs_m[i + 1:], t_vecs_m[i])
+            # count how many distances are smaller than the tolerance
+            if closed:
+                counts[-1] += np.sum(dsts <= tolerance)
+            else:
+                counts[-1] += np.sum(dsts < tolerance)
+    if counts[0] > 0 and counts[1] > 0:
+        saen = -np.log(1.0 * counts[1] / counts[0])
+    else:
+        # log would be infinite or undefined => cannot determine saen
+        zcounts = []
+        if counts[0] == 0:
+            zcounts.append("emb_dim")
+        if counts[1] == 0:
+            zcounts.append("emb_dim + 1")
+        print_message = (
+            "Zero vectors are within tolerance for {}. "
+            "Consider raising tolerance parameter to avoid {} result."
+        )
+        warnings.warn(
+            print_message.format(
+                " and ".join(zcounts),
+                "NaN" if len(zcounts) == 2 else "inf",
+            ),
+            RuntimeWarning
+        )
+        if counts[0] == 0 and counts[1] == 0:
+            saen = np.nan
+        elif counts[0] == 0:
+            saen = -np.inf
+        else:
+            saen = np.inf
+    return saen
+
+
+def sampen_optimized(
+        data,
+        tolerance=None,
+        closed=False,
+):
+    """
+
+    The following code is adapted from openly licensed code written by
+    Christopher Schölzel in his package
+    nolds (NOnLinear measures for Dynamical Systems).
+    It computes the sample entropy of time sequence data.
+    emb_dim has been set to 1 (not parameterized)
+    Returns
+    the sample entropy of the data (negative logarithm of ratio between
+    similar template vectors of length emb_dim + 1 and emb_dim)
+    [c_m, c_m1]:
+    list of two floats: count of similar template vectors of length emb_dim
+    (c_m) and of length emb_dim + 1 (c_m1)
+    [float list, float list]:
+    Lists of lists of the form ``[dists_m, dists_m1]`` containing the
+    distances between template vectors for m (dists_m)
+    and for m + 1 (dists_m1).
+    Reference:
+    .. [se_1] J. S. Richman and J. R. Moorman, “Physiological time-series
+    analysis using approximate entropy and sample entropy,”
+    American Journal of Physiology-Heart and Circulatory Physiology,
+    vol. 278, no. 6, pp. H2039–H2049, 2000.
+
+    Kwargs are pre-set and not available. For more extensive
+    you should use the sampen function.
+
+    :param data: array-like
+    :type data: array
+    :param tolerance: distance threshold for two template vectors
+    :type tolerance: float
+    :param distance: function to calculate distance
+    :type distance: function
+
+    :returns: saen
+    :rtype: float
+    """
+    # TODO: this function can still be further optimized
+    data = np.asarray(data)
+    if tolerance is None:
+        lint_helper = (0.5627 * np.log(1) + 1.3334)
+        tolerance = np.std(data, ddof=1) * 0.1164 * lint_helper
+    n = len(data)
+
+    # TODO(): This can be done with just using NumPy
+    t_vecs = delay_embedding(np.asarray(data), 3, lag=1)
+
+    if closed:
+        counts = calc_closed_sampent(t_vecs, n, tolerance)
+    else:
+        counts = calc_open_sampent(t_vecs, n, tolerance)
+
+    if counts[0] > 0 and counts[1] > 0:
+        saen = -np.log(1.0 * counts[1] / counts[0])
+    else:
+        # log would be infinite or undefined => cannot determine saen
+        zcounts = []
+        if counts[0] == 0:
+            zcounts.append("1")
+        if counts[1] == 0:
+            zcounts.append("2")
+        print_message = (
+            "Zero vectors are within tolerance for {}. "
+            "Consider raising tolerance parameter to avoid {} result."
+        )
+        warnings.warn(
+            print_message.format(
+                " and ".join(zcounts),
+                "NaN" if len(zcounts) == 2 else "inf",
+            ),
+            RuntimeWarning
+        )
+        if counts[0] == 0 and counts[1] == 0:
+            saen = np.nan
+        elif counts[0] == 0:
+            saen = -np.inf
+        else:
+            saen = np.inf
+    return saen
+
+
+def calc_closed_sampent(t_vecs, n, tolerance):
+    # TODO(someone?): Analogous to calc_open_sampent
+    return np.nan, np.nan
+
+
+def calc_open_sampent(t_vecs, n, tolerance):
+    triplets = t_vecs[:n - 2, :3]
+
+    raw_dsts = tuple(
+        triplets[i + 1:] - triplets[i]
+        for i in range(len(triplets) - 1)
+    )
+    dsts = np.concatenate(raw_dsts)
+    dsts_abs = np.abs(dsts)
+    dsts_gt = dsts_abs < tolerance
+    dsts_max_a = np.logical_and(dsts_gt[:, 0], dsts_gt[:, 1])
+    dsts_max = np.logical_and(dsts_max_a, dsts_gt[:, 2])
+    return np.sum(dsts_max_a), np.sum(dsts_max)
+
+
+def entropy_maker(
+        array,
+        method='sample_entropy',
+        base=None,
+):
+    """
+    The following code allows a user to input an array and calculate either
+    a time-series specific entropy i.e. the nolds or a more general
+    Shannon entropy as calculated in scipy.
+    It calls entropy functions in the file.
+
+    """
+    if method == 'scipy':
+        output = entropy_scipy(array, base=base)
+    elif method == 'nolds':
+        output = sampen(array)
+    elif method == 'sample_entropy':
+        output = sampen_optimized(array)
+    else:
+        print('your method is not an option,')
+        print('we defaulted to a slow unoptimized sample entropy')
+        output = sampen(array)
+    return output
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `resurfemg-0.0.8.dist-info/METADATA` & `resurfemg-0.0.9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resurfemg
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for analysis of respiratory EMG data
 Home-page: https://github.com/ReSurfEMG/ReSurfEMG
 Author: A team including the NLeSC and the U. of Twente
 Author-email: c.moore@esciencecenter.nl
 License: Apache v2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -32,14 +32,15 @@
 [![PyPI](https://img.shields.io/pypi/v/resurfemg.svg)](https://pypi.python.org/pypi/resurfemg/)
 [![Anaconda-Server Badge](https://anaconda.org/resurfemg/resurfemg/badges/version.svg)](https://anaconda.org/resurfemg/resurfemg)
 [![Sanity](https://github.com/resurfemg/resurfemg/actions/workflows/on-commit.yml/badge.svg)](https://github.com/resurfemg/resurfemg/actions/workflows/on-commit.yml)
 [![Sanity](https://github.com/resurfemg/resurfemg/actions/workflows/on-tag.yml/badge.svg)](https://github.com/resurfemg/resurfemg/actions/workflows/on-tag.yml)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6487/badge)](https://bestpractices.coreinfrastructure.org/projects/6487)
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![status](https://joss.theoj.org/papers/5f08d1f2bb717b7d05762296e37ded3d/status.svg)](https://joss.theoj.org/papers/5f08d1f2bb717b7d05762296e37ded3d)
 
 **ReSurfEMG** is an open source collaborative python library for analysis
 of respiratory electromyography (EMG).  On the same site as 
 the repository for this library we keep [related resources](https://github.com/ReSurfEMG?tab=repositories). 
 
 Most important to know before using ReSurfEMG is that we have a [main code library](https://github.com/ReSurfEMG/ReSurfEMG) where the user can access the code to change various filter and analysis settings directly and/or in our [researcher interface notebooks](https://github.com/ReSurfEMG/ReSurfEMG/tree/main/researcher_interface), and a [dashboard interface](https://github.com/ReSurfEMG/ReSurfEMG-dashboard) which contains default settings for preprocessing and analysis which can be changed through a graphical (no code) interface. We have some functionality available through a [command line interface](#command-line-interface) as well.
 
@@ -74,14 +75,21 @@
 
 ### Data sets
 
 The notebooks are configured to run on various datasets.  Contact
 Dr. Eline Mos-Oppersma( 📫 e.mos-oppersma@utwente.nl) to discuss any
 questions on data configuration for your datasets.
 
+If you want to use a standardized dataset for any purpose we reccomend
+the data in the ReSurfEMG/synthetic_data repository
+
+[![DOI](https://zenodo.org/badge/635680008.svg)](https://zenodo.org/badge/latestdoi/635680008)
+
+Data there can be used with any respiratory EMG algorithms in any program. Thus that data can function as a benchmarking set to compare algorithms across different programs.
+
 
 ### Configuring (to work with your data)
 
 In order to preprocess and/or to train  models the code needs to be
 able to locate the raw data you want it to find.
 
 There are several ways to specify the location of the following
@@ -130,56 +138,59 @@
 
 
 ## Getting started
 
 How to get the notebooks running?  Assuming the raw data set and
 metadata is available.
 
-0. In theory if you want to work, but never develop, as a conda user
-   with the stable version create an empty environment, and install
-   there:
-
-   _NB: at present (February 2023) we do not reccomend this route for
-   any users._
-
-    * Make sure you are in no environment:
+0. Assuming you are using conda for package management:    
+  * Make sure you are in no environment:
 
       ```sh
       conda deactivate
       ```
 
       _(repeat if you are in the base environment)_
 
-      You should be in no environment now
+      You should be in no environment now, (or alternatively you can build on your
+      base environment if you want)
 
-    * Create a blank environment with python pinned to 3.8
 
-      ```sh
-      conda create -n blank python=3.8
-      ```
-
-    * Install within the blank environment:
-
-      ```sh
-      conda activate blank
-      conda install -c conda-forge -c resurfemg resurfemg jupyter ipympl
-      ```
+1. Option A: To work with the most current versions with the possibility for development:
+  Install all Python packages required, using `conda` and the `environment.yml` file. 
 
-1. To work with the most current versions: Install all Python packages
-   required, using `conda` and the `environment.yml` file.
 
    * The command for Windows/Anaconda users can be something like:
 
      ```sh
      conda env create -f environment.yml
      ```
 
    * Linux users can create their own environment by hand (use
      install_dev as in setup).
 
+  Make sure to enter your newly created environment.
+
+Option B: In theory if you want to work, but never develop (i.e. add code), as a conda user
+   with the stable (released) version create an empty environment, and install
+   there: 
+
+
+   * Create a blank environment with python pinned to 3.8:
+
+     ```sh
+     conda create -n blank python=3.8
+     ```
+
+   * Install within the blank environment
+      ```sh
+        conda activate blank
+        conda install -c conda-forge -c resurfemg resurfemg jupyter ipympl
+        ```
+
 2. Open a notebook (we use [Jupyter
    notebooks](https://jupyter.org/try-jupyter/retro/notebooks/?path=notebooks/Intro.ipynb))
    in researcher_interface folder and interactively run the cells.
    You can use the command `jupyter notebook` to open a browser window
    on the folders of notebooks.  Note, if you run with an installed
    library import appropriately.
 
@@ -365,15 +376,17 @@
         mount --bind /ReSurfEMG/tests/not_pushed/ ./not_pushed/
         python setup.py test'
 ```
 
 ## Command-Line Interface
 
 You will be able to preprocess, train and use models using command-line interface.
-(Some functionality still pending module development completion)
+You can also, in some cases, create files in the correct format for our Dashboard
+in a per folder batch process.
+
 Below is an example of how to do that:
 
 This will pre-process (with the alternative_a_pipeline_multi algorithm) the
  Poly5 files in the
 `/mnt/data/originals` directory, and output leads 1 and 2 preprocessed.
 (Note the \ symbol is simply a line-break and not meant to be included.)
 
@@ -389,14 +402,17 @@
     python -m resurfemg ml |
             --input /mnt/data/preprocessed \
             --output /mnt/data/ml_output \
             --model  ml_models/finalized_lr_model_in_111.sav \
 
 You can also make synthetic data. To explore this start with
     `python -m resurfemg synth --help`
+You can also make from horizontally formated csv files 
+that can be read by the dashboard. To explore this start with
+    `python -m resurfemg save_np --help`
 The help commandis also available for ml and acquire.
 
 All long options have short aliases.
 
 
 ✨Copyright 2022 Netherlands eScience Center and U. Twente
 Licensed under the Apache License, version 2.0. See LICENSE for details.✨
```

## Comparing `resurfemg-0.0.8.dist-info/RECORD` & `resurfemg-0.0.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 resurfemg/__init__.py,sha256=iwhKnzeBJLKxpRVjvzwiRE63_zNpIBfaKLITauVph-0,24
 resurfemg/__main__.py,sha256=J6JHq_4OmTwwbvOsXNh--mDrH5vAfT_6hsYj6Ys5X-c,90
-resurfemg/cli.py,sha256=DOT3AQeCsK0152Q4e3whAlxspeTE5m2iGWFfo0NkMCs,5196
+resurfemg/cli.py,sha256=_WBLYxKUMhgQxuVjraC0ubKgl86MHbnf8BOpuMpny4g,5823
 resurfemg/config.py,sha256=G8xtUi32QXkHl-CKu_lTT09As7Es9MH5BDeOLU17Ltw,11004
-resurfemg/converter_functions.py,sha256=wcKA8UJKzRsv-tvtvE3dzOpQS5lVMRmHZ_WIaNkiJVk,4382
-resurfemg/helper_functions.py,sha256=8lI7VZ1rL-zB8TIR8edhSt1JEyhZQIoSPC48WguOZ2o,48950
+resurfemg/converter_functions.py,sha256=4OnXwNPgR7hsS5M55lrrHQpPnsF1EEgYHnzuiWfLzn8,6306
+resurfemg/helper_functions.py,sha256=HplF3TuunvlkwaRUDIER17rSUXd5BLo6YgFpKVUiYaQ,62540
 resurfemg/ml.py,sha256=Ugjh2EuDU_r2HBirG0FZWfhtaIGA59U7ge-dBh3GNIA,2476
 resurfemg/multi_lead_type.py,sha256=nJPRO5rWZp6TSlXoU79fBG5n9YW7gfHxXt5p5RxeqWY,17071
 resurfemg/tmsisdk_lite.py,sha256=2DK6r8PqBAhwBUPLJxedoaW9YW1z5Bo3X3OgxKvWCzM,9450
-resurfemg-0.0.8.dist-info/METADATA,sha256=k2PjbzvY2DeDoyIZwlOF0zOkqMILsGcodqJqipq8XIs,15189
-resurfemg-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-resurfemg-0.0.8.dist-info/top_level.txt,sha256=u30hNTZIkHnbFMEMG0n9CswHMS6bEFL6iqbq1RX6jwU,10
-resurfemg-0.0.8.dist-info/RECORD,,
+resurfemg-0.0.9.dist-info/METADATA,sha256=7hHazkqBwb5WyYJLgr1Y8ZHvA7saD-OBpWpQmjZwIlo,16131
+resurfemg-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+resurfemg-0.0.9.dist-info/top_level.txt,sha256=u30hNTZIkHnbFMEMG0n9CswHMS6bEFL6iqbq1RX6jwU,10
+resurfemg-0.0.9.dist-info/RECORD,,
```

