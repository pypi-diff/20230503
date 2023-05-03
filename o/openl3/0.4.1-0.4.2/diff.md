# Comparing `tmp/openl3-0.4.1.tar.gz` & `tmp/openl3-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openl3-0.4.1.tar", last modified: Wed Aug  4 16:58:15 2021, max compression
+gzip compressed data, was "openl3-0.4.2.tar", last modified: Wed May  3 18:19:30 2023, max compression
```

## Comparing `openl3-0.4.1.tar` & `openl3-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 beasteers   (501) admin       (80)        0 2021-08-04 16:58:15.000000 openl3-0.4.1/
--rw-r--r--   0 beasteers   (501) admin       (80)     6319 2021-08-04 16:58:15.000000 openl3-0.4.1/PKG-INFO
--rw-r--r--   0 beasteers   (501) admin       (80)     4438 2021-08-04 15:42:42.000000 openl3-0.4.1/README.md
-drwxr-xr-x   0 beasteers   (501) admin       (80)        0 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3/
--rw-r--r--   0 beasteers   (501) admin       (80)      252 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/__init__.py
--rw-r--r--   0 beasteers   (501) admin       (80)      102 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/__main__.py
--rw-r--r--   0 beasteers   (501) admin       (80)    10882 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/cli.py
--rw-r--r--   0 beasteers   (501) admin       (80)    39042 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/core.py
--rw-r--r--   0 beasteers   (501) admin       (80)    22117 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/models.py
--rw-r--r--   0 beasteers   (501) admin       (80)       81 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/openl3_exceptions.py
--rw-r--r--   0 beasteers   (501) admin       (80)       78 2021-08-04 15:42:42.000000 openl3-0.4.1/openl3/openl3_warnings.py
--rw-r--r--   0 beasteers   (501) admin       (80)       40 2021-08-04 16:40:09.000000 openl3-0.4.1/openl3/version.py
-drwxr-xr-x   0 beasteers   (501) admin       (80)        0 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/
--rw-r--r--   0 beasteers   (501) admin       (80)     6319 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/PKG-INFO
--rw-r--r--   0 beasteers   (501) admin       (80)      366 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/SOURCES.txt
--rw-r--r--   0 beasteers   (501) admin       (80)        1 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/dependency_links.txt
--rw-r--r--   0 beasteers   (501) admin       (80)       44 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/entry_points.txt
--rw-r--r--   0 beasteers   (501) admin       (80)      253 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/requires.txt
--rw-r--r--   0 beasteers   (501) admin       (80)        7 2021-08-04 16:58:15.000000 openl3-0.4.1/openl3.egg-info/top_level.txt
--rw-r--r--   0 beasteers   (501) admin       (80)      172 2021-08-04 16:58:15.000000 openl3-0.4.1/setup.cfg
--rw-r--r--   0 beasteers   (501) admin       (80)     3654 2021-08-04 15:42:42.000000 openl3-0.4.1/setup.py
+drwxrwxr-x   0 aurora    (1000) aurora    (1000)        0 2023-05-03 18:19:30.594431 openl3-0.4.2/
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     1115 2023-05-03 17:56:43.000000 openl3-0.4.2/LICENSE
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     6375 2023-05-03 18:19:30.594431 openl3-0.4.2/PKG-INFO
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     5280 2023-05-03 17:56:09.000000 openl3-0.4.2/README.md
+drwxrwxr-x   0 aurora    (1000) aurora    (1000)        0 2023-05-03 18:19:30.590431 openl3-0.4.2/openl3/
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)      252 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/__init__.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)      102 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/__main__.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)    10882 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/cli.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)    40215 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/core.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)    23945 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/models.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)       81 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/openl3_exceptions.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)       78 2023-05-03 17:42:46.000000 openl3-0.4.2/openl3/openl3_warnings.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)       40 2023-05-03 18:01:25.000000 openl3-0.4.2/openl3/version.py
+drwxrwxr-x   0 aurora    (1000) aurora    (1000)        0 2023-05-03 18:19:30.590431 openl3-0.4.2/openl3.egg-info/
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     6375 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/PKG-INFO
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)      457 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)        1 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)       43 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/entry_points.txt
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)      240 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/requires.txt
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)        7 2023-05-03 18:19:30.000000 openl3-0.4.2/openl3.egg-info/top_level.txt
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)      172 2023-05-03 18:19:30.594431 openl3-0.4.2/setup.cfg
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     3626 2023-05-03 18:08:57.000000 openl3-0.4.2/setup.py
+drwxrwxr-x   0 aurora    (1000) aurora    (1000)        0 2023-05-03 18:19:30.594431 openl3-0.4.2/tests/
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     8027 2023-05-03 17:42:46.000000 openl3-0.4.2/tests/test_cli.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)    46316 2023-05-03 17:42:46.000000 openl3-0.4.2/tests/test_core.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     6839 2023-05-03 17:42:46.000000 openl3-0.4.2/tests/test_models.py
+-rw-rw-r--   0 aurora    (1000) aurora    (1000)     8318 2023-05-03 17:42:46.000000 openl3-0.4.2/tests/test_regression.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openl3-0.4.1/README.md` & `openl3-0.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # OpenL3
 
 OpenL3 is an open-source Python library for computing deep audio and image embeddings.
 
-[![PyPI](https://img.shields.io/badge/python-2.7%2C%203.5%2C%203.6-blue.svg)](https://pypi.python.org/pypi/openl3)
+[![PyPI](https://img.shields.io/badge/python-3.6%2C%203.7%2C%203.8-blue.svg)](https://pypi.python.org/pypi/openl3)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://choosealicense.com/licenses/mit/)
-[![Build Status](https://travis-ci.org/marl/openl3.svg?branch=master)](https://travis-ci.org/marl/openl3)
-[![Coverage Status](https://coveralls.io/repos/github/marl/openl3/badge.svg?branch=master)](https://coveralls.io/github/marl/openl3?branch=master)
+[![Build Status](https://travis-ci.com/marl/openl3.svg?branch=main)](https://travis-ci.com/marl/openl3)
+[![Coverage Status](https://coveralls.io/repos/github/marl/openl3/badge.svg?branch=main)](https://coveralls.io/github/marl/openl3?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/openl3/badge/?version=latest)](http://openl3.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/openl3)](https://pepy.tech/project/openl3)
 
 Please refer to the [documentation](https://openl3.readthedocs.io/en/latest/) for detailed instructions and examples.
 
 > **UPDATE:** Openl3 now has Tensorflow 2 support!
 
+> **NOTE:** Whoops! A bug was reported in the [training code](https://github.com/marl/l3embedding), with the effect that positive audio-image pairs that come from the same video do not necessarily overlap in time. Nonetheless, the embedding still seems to capture useful semantic information.
+
 The audio and image embedding models provided here are published as part of [1], and are based on the Look, Listen and Learn approach [2]. For details about the embedding models and how they were trained, please see:
 
 [Look, Listen and Learn More: Design Choices for Deep Audio Embeddings](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/cramer_looklistenlearnmore_icassp_2019.pdf)<br/>
-Jason Cramer, Ho-Hsiang Wu, Justin Salamon, and Juan Pablo Bello.<br/>
+Aurora Cramer, Ho-Hsiang Wu, Justin Salamon, and Juan Pablo Bello.<br/>
 IEEE Int. Conf. on Acoustics, Speech and Signal Processing (ICASSP), pages 3852–3856, Brighton, UK, May 2019.
 
 
 # Installing OpenL3
 
 Dependencies
 ------------
@@ -65,19 +68,19 @@
 The simplest way to install OpenL3 is by using ``pip``, which will also install the additional required dependencies
 if needed. To install OpenL3 using ``pip``, simply run
 
     pip install openl3
 
 To install the latest version of OpenL3 from source:
 
-1. Clone or pull the lastest version:
+1. Clone or pull the latest version, only retrieving the ``main`` branch to avoid downloading the branch where we store the model weight files (these will be properly downloaded during installation).
 
-        git clone git@github.com:marl/openl3.git
+        git clone git@github.com:marl/openl3.git --branch main --single-branch
 
-2. Install using pip to handle python dependencies:
+2. Install using pip to handle python dependencies. The installation also downloads model files, **which requires a stable network connection**.
 
         cd openl3
         pip install -e .
 
 # Using OpenL3
 
 To help you get started with OpenL3 please see the
@@ -85,13 +88,16 @@
 
 
 # Acknowledging OpenL3
 
 Please cite the following papers when using OpenL3 in your work:
 
 [1] [Look, Listen and Learn More: Design Choices for Deep Audio Embeddings](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/cramer\_looklistenlearnmore\_icassp\_2019.pdf)<br/>
-Jason Cramer, Ho-Hsiang Wu, Justin Salamon, and Juan Pablo Bello.<br/>
+Aurora Cramer, Ho-Hsiang Wu, Justin Salamon, and Juan Pablo Bello.<br/>
 IEEE Int. Conf. on Acoustics, Speech and Signal Processing (ICASSP), pages 3852–3856, Brighton, UK, May 2019.
 
 [2] [Look, Listen and Learn](http://openaccess.thecvf.com/content\_ICCV\_2017/papers/Arandjelovic\_Look\_Listen\_and\_ICCV\_2017\_paper.pdf)<br/>
 Relja Arandjelović and Andrew Zisserman<br/>
 IEEE International Conference on Computer Vision (ICCV), Venice, Italy, Oct. 2017.
+
+# Model Weights License
+The model weights are made available under a [Creative Commons Attribution 4.0 International (CC BY 4.0) License](https://creativecommons.org/licenses/by/4.0/).
```

### Comparing `openl3-0.4.1/openl3/cli.py` & `openl3-0.4.2/openl3/cli.py`

 * *Files identical despite different names*

### Comparing `openl3-0.4.1/openl3/core.py` & `openl3-0.4.2/openl3/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,28 +99,28 @@
     return x
 
 
 def _librosa_linear_frontend(audio, n_fft=512, hop_length=242, db_amin=1e-10, 
                              db_ref=1.0, dynamic_range=80.0):
     '''Librosa linear frontend designed to match original Kapre (0.1.4).'''
     import librosa
-    S = np.abs(librosa.stft(audio, n_fft=n_fft, hop_length=hop_length, center=False))
-    S = librosa.power_to_db(S, ref=db_ref, amin=db_amin, top_db=dynamic_range)
+    S = np.abs(librosa.stft(y=audio, n_fft=n_fft, hop_length=hop_length, center=False))
+    S = librosa.power_to_db(S=S, ref=db_ref, amin=db_amin, top_db=dynamic_range)
     S -= S.max()
     return S
 
 
 def _librosa_mel_frontend(audio, sr, n_mels=128, n_fft=2048, hop_length=242,
                           db_amin=1e-10, db_ref=1.0, dynamic_range=80.0):
     '''Librosa mel frontend designed to match original Kapre (0.1.4).'''
     import librosa
     S = librosa.feature.melspectrogram(
-        audio, sr, n_mels=n_mels, n_fft=n_fft, hop_length=hop_length, 
+        y=audio, sr=sr, n_mels=n_mels, n_fft=n_fft, hop_length=hop_length,
         center=True, power=1.0)
-    S = librosa.power_to_db(S, ref=db_ref, amin=db_amin, top_db=dynamic_range)
+    S = librosa.power_to_db(S=S, ref=db_ref, amin=db_amin, top_db=dynamic_range)
     S -= S.max()
     return S
 
 
 def preprocess_audio(audio, sr, hop_size=0.1, input_repr=None, center=True, **kw):
     """
     Preprocess the audio into a format compatible with the model.
@@ -445,14 +445,15 @@
 
     Returns
     -------
     batch : np.ndarray [shape=(N, H, W, C)]
         4d numpy array of image data.
     """
     import skimage
+    import skimage.transform
     if image.size == 0:
         raise OpenL3Error('Got empty image')
 
     # Warn user if image is all zero
     if np.all(image == 0):
         warnings.warn('Provided image is all zeros', OpenL3Warning)
 
@@ -476,15 +477,32 @@
         # If image is not 224x224, rescale to 256x256, and take center
         # 224x224 image patch, corresponding to what was done in L3
         scaling = 256.0 / min(image.shape[1], image.shape[2])
         batch = np.zeros((image.shape[0], 224, 224, 3))
         for idx, frame in enumerate(image):
             # Only reshape if image is larger than 256x256
             if min(frame.shape[0], frame.shape[1]) > 256:
-                frame = skimage.transform.rescale(frame, scaling)
+                try:
+                    frame = skimage.transform.rescale(frame, scaling,
+                                                      mode='constant',
+                                                      cval=0,
+                                                      clip=True,
+                                                      preserve_range=False,
+                                                      channel_axis=-1,
+                                                      anti_aliasing=False,
+                                                      anti_aliasing_sigma=None)
+                except TypeError:
+                    frame = skimage.transform.rescale(frame, scaling,
+                                                      mode='constant',
+                                                      cval=0,
+                                                      clip=True,
+                                                      preserve_range=False,
+                                                      multichannel=True,
+                                                      anti_aliasing=False,
+                                                      anti_aliasing_sigma=None)
             x1, x2 = frame.shape[:-1]
             startx1 = x1//2-(224//2)
             startx2 = x2//2-(224//2)
             batch[idx] = frame[startx1:startx1+224,startx2:startx2+224]
     else:
         batch = image
 
@@ -675,15 +693,15 @@
     verbose : bool
         If True, prints verbose messages.
 
     Returns
     -------
 
     """
-    import skimage
+    import skimage.io
     if isinstance(filepath, str):
         filepath_list = [filepath]
     elif isinstance(filepath, list):
         filepath_list = filepath
     else:
         err_msg = 'filepath should be type str or list[str], but got {}.'
         raise OpenL3Error(err_msg.format(filepath))
```

### Comparing `openl3-0.4.1/openl3/models.py` & `openl3-0.4.2/openl3/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         Flatten, Activation, Lambda)
     import tensorflow.keras.regularizers as regularizers
 
 
 VALID_FRONTENDS = ("librosa", "kapre")
 VALID_INPUT_REPRS = ("linear", "mel128", "mel256")
 VALID_CONTENT_TYPES = ("music", "env")
-VALID_EMBEDDING_SIZES = (6144, 512)
+VALID_AUDIO_EMBEDDING_SIZES = (6144, 512)
+VALID_IMAGE_EMBEDDING_SIZES = (8192, 512)
 
 
 def _log10(x):
     '''log10 tensorflow function.'''
     return tf.math.log(x) / tf.math.log(tf.constant(10, dtype=x.dtype))
 
 
@@ -125,22 +126,50 @@
         be included. Otherwise no frontend will be added inside the keras model.
 
     Returns
     -------
     model : tf.keras.Model
         Model object.
     """
+    model_path = get_audio_embedding_model_path(input_repr, content_type)
+    return load_audio_embedding_model_from_path(model_path, input_repr, embedding_size, frontend=frontend)
+
+
+def load_audio_embedding_model_from_path(model_path, input_repr, embedding_size, frontend='kapre'):
+    """
+    Loads a model with weights at the given path.
+
+    Parameters
+    ----------
+    model_path : str
+        Path to model weights HDF5 (.h5) file. Must be in format
+        `*._<input_repr>_<content_type>.h5` or
+        `*._<input_repr>_<content_type>-.*.h5`, since model configuration
+        will be determined from the filename.
+    input_repr : "linear", "mel128", or "mel256"
+        Spectrogram representation used for audio model.
+    embedding_size : 6144 or 512
+        Embedding dimensionality.
+    frontend : "kapre" or "librosa"
+        The audio frontend to use. If frontend == 'kapre', then the kapre frontend will
+        be included. Otherwise no frontend will be added inside the keras model.
+
+    Returns
+    -------
+    model : tf.keras.Model
+        Model object.
+    """
     frontend, input_repr = _validate_audio_frontend(frontend, input_repr)
 
     # Construct embedding model and load model weights
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         m = AUDIO_MODELS[input_repr](include_frontend=frontend == 'kapre')
 
-    m.load_weights(get_audio_embedding_model_path(input_repr, content_type))
+    m.load_weights(model_path)
 
     # Pooling for final output embedding size
     pool_size = AUDIO_POOLING_SIZES[input_repr][embedding_size]
     y_a = MaxPooling2D(pool_size=pool_size, padding='same')(m.output)
     y_a = Flatten()(y_a)
     m = Model(inputs=m.input, outputs=y_a)
     m.frontend = frontend
@@ -175,29 +204,56 @@
 
     Parameters
     ----------
     input_repr : "linear", "mel128", or "mel256"
         Spectrogram representation used for audio model.
     content_type : "music" or "env"
         Type of content used to train embedding.
+    embedding_size : 8192 or 512
+        Embedding dimensionality.
+
+    Returns
+    -------
+    model : tf.keras.Model
+        Model object.
+    """
+
+    model_path = get_image_embedding_model_path(input_repr, content_type)
+    return load_image_embedding_model_from_path(model_path, embedding_size)
+
+
+def load_image_embedding_model_from_path(model_path, embedding_size):
+    """
+    Loads a model with weights at the given path.
+
+    Parameters
+    ----------
+    model_path : str
+        Path to model weights HDF5 (.h5) file.
     embedding_size : 6144 or 512
         Embedding dimensionality.
+    input_repr : "linear", "mel128", or "mel256"
+        Spectrogram representation used for audio model.
+    content_type : "music" or "env"
+        Type of content used to train embedding.
+    embedding_size : 8192 or 512
+        Embedding dimensionality.
 
     Returns
     -------
     model : tf.keras.Model
         Model object.
     """
 
     # Construct embedding model and load model weights
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         m = _construct_image_network()
 
-    m.load_weights(get_image_embedding_model_path(input_repr, content_type))
+    m.load_weights(model_path)
 
     # Pooling for final output embedding size
     pool_size = IMAGE_POOLING_SIZES[embedding_size]
     y_i = MaxPooling2D(pool_size=pool_size, padding='same')(m.output)
     y_i = Flatten()(y_i)
     m = Model(inputs=m.input, outputs=y_i)
     return m
```

### Comparing `openl3-0.4.1/setup.py` & `openl3-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,26 +36,26 @@
                     target.write(source.read())
             print('Decompression complete')
             os.remove(compressed_path)
             print('Removing compressed file')
 
 version = imp.load_source('openl3.version', os.path.join('openl3', 'version.py'))
 
-with open('README.md') as file:
+with open('README.md', encoding='utf8') as file:
     long_description = file.read()
 
 setup(
     name='openl3',
     version=version.version,
     description='Deep audio and image embeddings, based on Look, Listen, and Learn approach',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/marl/openl3',
-    author='Jason Cramer, Ho-Hsiang Wu, Bea Steers, and Justin Salamon',
-    author_email='jtcramer@nyu.edu',
+    author='Aurora Cramer, Ho-Hsiang Wu, Bea Steers, and Justin Salamon',
+    author_email='jtc440@nyu.edu',
     packages=find_packages(),
     entry_points={
         'console_scripts': ['openl3=openl3.cli:main'],
     },
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -77,22 +77,22 @@
     install_requires=[
         'tensorflow>=2.0.0',
         'numpy>=1.13.0',
         'scipy>=0.19.1',
         'kapre>=0.3.5',
         'soundfile>=0.9.0.post1',
         'resampy>=0.2.1,<0.3.0',
-        'h5py>=2.7.0,<3.0.0',
+        'h5py>=2.7.0',
         'moviepy>=1.0.0',
-        'scikit-image>=0.14.3'
+        'scikit-image>=0.14.3',
         'librosa>=0.7.2',  # version limit from kapre
     ],
     extras_require={
         'docs': [
-                'sphinx==1.2.3',  # autodoc was broken in 1.3.1
+                'sphinx',
                 'sphinxcontrib-napoleon',
                 'sphinx_rtd_theme',
                 'numpydoc',
             ],
         'tests': []
     },
     package_data={
```

