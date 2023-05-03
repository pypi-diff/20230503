# Comparing `tmp/cahmml-1.0.1.tar.gz` & `tmp/cahmml-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cahmml-1.0.1.tar", max compression
+gzip compressed data, was "cahmml-1.0.2.tar", max compression
```

## Comparing `cahmml-1.0.1.tar` & `cahmml-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1083 2023-01-09 21:53:58.069232 cahmml-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0       18 2023-01-04 22:17:53.882609 cahmml-1.0.1/cahmml/__init__.py
--rw-r--r--   0        0        0    11552 2023-01-18 17:30:22.897002 cahmml-1.0.1/cahmml/hmm.py
--rw-r--r--   0        0        0    11049 2023-01-09 22:49:44.293644 cahmml-1.0.1/cahmml/test/test_hmm.py
--rw-r--r--   0        0        0      104 2023-01-04 22:17:53.889501 cahmml-1.0.1/cahmml/util.py
--rw-r--r--   0        0        0      352 2023-01-18 18:03:37.546066 cahmml-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      642 2023-01-18 18:04:05.238563 cahmml-1.0.1/setup.py
--rw-r--r--   0        0        0      375 2023-01-18 18:04:05.239609 cahmml-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-09 21:53:58.069232 cahmml-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0       18 2023-01-04 22:17:53.882609 cahmml-1.0.2/cahmml/__init__.py
+-rw-r--r--   0        0        0    16668 2023-04-11 19:47:13.273595 cahmml-1.0.2/cahmml/hmm.py
+-rw-r--r--   0        0        0    13573 2023-04-11 19:47:13.297727 cahmml-1.0.2/cahmml/test/test_hmm.py
+-rw-r--r--   0        0        0      772 2023-04-11 19:47:13.315905 cahmml-1.0.2/cahmml/util.py
+-rw-r--r--   0        0        0      355 2023-05-03 18:07:28.527107 cahmml-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      627 2023-05-03 18:07:34.138341 cahmml-1.0.2/setup.py
+-rw-r--r--   0        0        0      360 2023-05-03 18:07:34.138919 cahmml-1.0.2/PKG-INFO
```

### Comparing `cahmml-1.0.1/LICENSE.txt` & `cahmml-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cahmml-1.0.1/cahmml/hmm.py` & `cahmml-1.0.2/cahmml/hmm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Built-in libraries
-from typing import Iterable
+from typing import Iterable, Tuple
 from abc import ABC, abstractmethod
 import warnings
 
 # Internal libraries
 from . import util as hu
 
 # External libraries
@@ -97,15 +97,15 @@
 
         Args:
             obs (Iterable[Observation]): Observations for which to compute probability
             t (int): Timepoint index
             hyperparameters (dict, optional): Any hyperparameters you'll want passed in later. Defaults to {}.
 
         Returns:
-            float: log10(P(obs|self)) x |SAMPLES|
+            float: P(obs|self) x |SAMPLES|
         """
         pass
 
     @abstractmethod
     def transition_probability(
         self,
         next: "State",
@@ -118,15 +118,15 @@
         Args:
             next (State): destination State for which to compute probability
             obs (Iterable[Observations]): Observations for each sample
             t (int): Timepoint index
             hyperparameters (dict, optional): Any hyperparameters you'll want passed in later. Defaults to {}.
 
         Returns:
-            float: log10(P(next|self)) x |SAMPLES|
+            float: P(next|self) x |SAMPLES|
         """
         pass
 
 
 class HMM:
     def __init__(self, states: Iterable[State]):
         """Constructor for HMM
@@ -158,23 +158,28 @@
         self.samples = samples
         self.initial_probabilities = np.array(initial_probabilities)
         self.e_hparams = e_hparams
         self.t_hparams = t_hparams
         # Any validations we need to assume before fitting
         self._validate()
 
-        self.initial_probabilities = np.log10(self.initial_probabilities)
-
-    def sample_iterator(self):
+    def sample_iterator(self, reversed: bool = False):
         """Internal iterator to be passed to emission_probability and transition_probability
 
+        Args:
+            reversed (bool, optional): Reverse observation order. Defaults to False.
+
         Yields:
             List[Observation]: Observations for each Sample at a given timepoint
+
         """
-        sample_iters = [iter(sample.obs) for sample in self.samples]
+        if reversed:
+            sample_iters = [iter(sample.obs[::-1]) for sample in self.samples]
+        else:
+            sample_iters = [iter(sample.obs) for sample in self.samples]
         for i in range(self.n_obs):
             yield i, [next(sample_iter) for sample_iter in sample_iters]
 
     def _validate(self):
         self.n_states = 0
         self.n_samples = 0
         self.n_obs = 0
@@ -263,15 +268,15 @@
         try:
             assert len(self.initial_probabilities) == self.n_states
         except AssertionError:
             raise hu.HMMValidationError(
                 f"Initial probabilities shape does not match number of states ({len(self.initial_probabilities)} vs {self.n_states})"
             )
 
-    def viterbi(self) -> np.ndarray:        
+    def viterbi(self) -> np.ndarray:
         """Solve a fitted HMM using Viterbi
 
         Raises:
             hu.HMMValidationError: Raised if fit() was not called first
 
         Returns:
             np.ndarray: |Samples| x |Observations| matrix with state predictions
@@ -282,48 +287,47 @@
             assert self.samples is not None
         except AssertionError:
             raise hu.HMMValidationError("Call fit() before viterbi()")
 
         # Placeholder matrices for probabilities
         T1 = np.zeros([self.n_samples, self.n_states, self.n_obs])
         T2 = np.zeros_like(T1, dtype=int)
-        T_o = np.zeros([self.n_samples,self.n_states,self.n_states])
-        E_o = np.zeros([self.n_samples,self.n_states])
+        T_o = np.zeros([self.n_samples, self.n_states, self.n_states])
+        E_o = np.zeros([self.n_samples, self.n_states])
 
         # Populate Viterbi
-        for o,obs in track(
+        for o, obs in track(
             self.sample_iterator(), total=self.n_obs, description="Fitting"
         ):
 
             # Calculate emission probabilities
             for i, s_i in enumerate(self.states):
-                E_o[:,i] = s_i.emission_probability(obs,o,self.e_hparams)
+                E_o[:, i] = np.log10(s_i.emission_probability(obs, o, self.e_hparams))
             if (E_o > 0).any():
                 raise hu.HMMValidationError("Emission probability cannot exceed 1.")
 
             # Special case: first observation
             if o == 0:
-                T1[:,:,o] = self.initial_probabilities + E_o
+                T1[:, :, o] = np.log10(self.initial_probabilities) + E_o
                 continue
 
             # Calculate transition probabilities
             for i, s_i in enumerate(self.states):
                 for j, s_j in enumerate(self.states):
-                    T_o[:,i,j] = s_i.transition_probability(s_j,obs,o,self.t_hparams)
+                    T_o[:, i, j] = np.log10(s_i.transition_probability(
+                        s_j, obs, o, self.t_hparams
+                    ))
             if (T_o > 0).any():
                 raise hu.HMMValidationError("Transition probability cannot exceed 1.")
 
             # This line is very confusing, so here's more of a description
             # Line 1: T1[k,j-1]
             # Line 2: Aki
             # Line 3: Biy
-            tmp = (
-                np.repeat(T1[:, :, o - 1, np.newaxis], self.n_states, axis=-1)
-                + T_o
-            )
+            tmp = np.repeat(T1[:, :, o - 1, np.newaxis], self.n_states, axis=-1) + T_o
 
             # Max and argmax, respectively
             T1[:, :, o] = tmp.max(axis=1) + E_o
             T2[:, :, o] = tmp.argmax(axis=1)
 
         # Backtrack to find the best path
         bt_ptr = T1[:, :, -1].argmax(axis=1)
@@ -337,7 +341,123 @@
                 np.array(bt_ptr),
                 np.array([o + 1] * self.n_samples),
             ]
             bt[:, o] = bt_ptr
 
         # Return states as an array
         return bt
+
+    def _forward(self):
+        """Forward component of forward-backward algorithm, don't call this.
+
+        Returns:
+            Tuple[np.ndarray]: full forward array and final probabilities
+        """
+        fwd = np.zeros([self.n_samples, self.n_states, self.n_obs])
+        prev_sum = np.zeros([self.n_samples, self.n_states])
+        prev = None
+        T_o = np.zeros([self.n_samples, self.n_states, self.n_states])
+        E_o = np.zeros([self.n_samples, self.n_states])
+
+        for o, obs in track(
+            self.sample_iterator(), total=self.n_obs, description="Forward"
+        ):  
+            # Calculate emission probabilities
+            for i, s_i in enumerate(self.states):
+                E_o[:, i] = np.log10(s_i.emission_probability(obs, o, self.e_hparams))
+            if (E_o > 0).any():
+                raise hu.HMMValidationError("Emission probability cannot exceed 1.")
+
+            # Calculate transition probabilities
+            for i, s_i in enumerate(self.states):
+                for j, s_j in enumerate(self.states):
+                    T_o[:, i, j] = np.log10(s_i.transition_probability(
+                        s_j, obs, o, self.t_hparams
+                    ))
+            if (T_o > 0).any():
+                raise hu.HMMValidationError("Transition probability cannot exceed 1.")
+            
+            if o == 0:
+                # Special case: first observation
+                prev_sum = np.repeat(np.log10(self.initial_probabilities)[np.newaxis, :], self.n_samples, axis=0)
+            else:
+                # General case
+                prev_sum = hu.logsum10(np.transpose(prev[:,np.newaxis], axes=(0,2,1)) + T_o, axis=1)
+            prev = prev_sum + E_o
+            fwd[:, :, o] =  prev
+        p_fwd = hu.logsum10(fwd[:, :, -1], axis=1)
+        return fwd, p_fwd
+
+
+    def _backward(self) -> Tuple[np.ndarray]:
+        """Backward component of forward-backward algorithm, don't call this.
+
+        Returns:
+            Tuple[np.ndarray]: full backward array and final probabilities
+        """
+        bwd = np.zeros([self.n_samples, self.n_states, self.n_obs])
+        prev_sum = np.zeros([self.n_samples, self.n_states])
+        prev = None
+        pre_obs = None
+        T_o = np.zeros([self.n_samples, self.n_states, self.n_states])
+        E_o = np.zeros([self.n_samples, self.n_states])
+
+        for o, obs in track(
+            self.sample_iterator(reversed=True), total=self.n_obs, description="Backward"
+        ):
+            if o == 0:
+                # Special case: first observation
+                prev_sum = np.zeros((self.n_samples, self.n_states))
+            else:
+                # General case
+
+                # Calculate emission probabilities
+                for i, s_i in enumerate(self.states):
+                    E_o[:, i] = np.log10(s_i.emission_probability(pre_obs, self.n_obs-1-o, self.e_hparams))
+                if (E_o > 0).any():
+                    raise hu.HMMValidationError("Emission probability cannot exceed 1.")
+
+                # Calculate transition probabilities
+                for i, s_i in enumerate(self.states):
+                    for j, s_j in enumerate(self.states):
+                        T_o[:, i, j] = np.log10(s_i.transition_probability(
+                            s_j, pre_obs, self.n_obs-1-o, self.t_hparams
+                        ))
+                if (T_o > 0).any():
+                    raise hu.HMMValidationError("Transition probability cannot exceed 1.")
+
+                prev_sum = hu.logsum10(T_o + E_o[:,np.newaxis] + prev[:,np.newaxis], axis=2)
+            prev = prev_sum
+            bwd[:, :, -o-1] =  prev
+            pre_obs = obs
+
+        # Calculate emission probabilities for backward probability
+        for i, s_i in enumerate(self.states):
+            E_o[:, i] = np.log10(s_i.emission_probability(pre_obs, self.n_obs-o, self.e_hparams))
+        if (E_o > 0).any():
+            raise hu.HMMValidationError("Emission probability cannot exceed 1.")
+
+        p_bwd = hu.logsum10(np.repeat(np.log10(self.initial_probabilities)[np.newaxis, :], self.n_samples, axis=0) + E_o + bwd[:, :, 0], axis=1)
+        return bwd, p_bwd
+
+    def fb(self) -> np.ndarray:
+        """Forward-backward algorithm to obtain a-posteriori probabilities
+
+        Raises:
+            hu.HMMValidationError: Raised if fit() was not called first
+
+        Returns:
+            np.ndarray: |Samples| x |States| x |Observations| matrix with state probabilities
+        """
+        # Validate that we've already fit samples
+        try:
+            assert self.samples is not None
+        except AssertionError:
+            raise hu.HMMValidationError("Call fit() before fb()")
+
+        fwd, p_fwd = self._forward()
+        bwd, p_bwd = self._backward()
+
+        posterior = np.power(10, fwd + bwd - p_fwd[:, np.newaxis, np.newaxis])
+
+        assert (np.isclose(p_fwd, p_bwd, rtol=1e-20)).all()
+        return posterior
```

### Comparing `cahmml-1.0.1/cahmml/test/test_hmm.py` & `cahmml-1.0.2/cahmml/test/test_hmm.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             elif self.state_eg == "state3":
                 if o.obs_eg == "obs1":
                     probs.append(0.001)
                 elif o.obs_eg == "obs2":
                     probs.append(0.199)
                 elif o.obs_eg == "obs3":
                     probs.append(0.8)
-        return h.np.log10(h.np.array(probs))
+        return h.np.array(probs)
 
     def transition_probability(
         self,
         next: "StateExample",
         obs: h.Iterable[ObsExample],
         t: int,
         hyperparameters: dict = {},
@@ -112,15 +112,15 @@
             elif self.state_eg == "state3":
                 if next.state_eg == "state1":
                     probs.append(0.1)
                 elif next.state_eg == "state2":
                     probs.append(0.3)
                 elif next.state_eg == "state3":
                     probs.append(0.6)
-        return h.np.log10(h.np.array(probs))
+        return h.np.array(probs)
 
 
 class TestHMM:
 
     states = [StateExample("state1"), StateExample("state2"), StateExample("state3")]
     obs_options = [ObsExample("obs1"), ObsExample("obs2"), ObsExample("obs3")]
 
@@ -130,15 +130,15 @@
         assert model.T == None
         assert model.E == None
         assert model.initial_probabilities == None
 
     def fit_test_helper(self, samples, obs, initial_prob, model):
         assert h.np.array_equal(samples, model.samples)
         assert h.np.array_equal(
-            h.np.log10(h.np.array(initial_prob)), model.initial_probabilities
+            h.np.array(initial_prob), model.initial_probabilities
         )
         assert model.n_states == len(self.states)
         assert model.n_samples == len(samples)
         assert model.n_obs == len(obs)
         assert model.obs_type == type(self.obs_options[0])
         assert model.state_type == type(self.states[0])
         assert model.sample_type == type(samples[0])
@@ -168,14 +168,24 @@
             assert obs_l == [obs_list[i][obs_i] for i in range(model.n_samples)]
 
         # test HMM viterbi
         # validated with hmmlearn https://github.com/hmmlearn/hmmlearn
         X = model.viterbi()
         assert h.np.array_equal(X, [[0, 0, 0, 2, 2, 1]])
 
+        # test HMM forward and backward
+        # validated with hmmlearn https://github.com/hmmlearn/hmmlearn
+        X = model.fb()
+        assert (h.np.isclose(X, [[[0.9863564256586119, 0.947016400035409, 0.9765470122937462,
+                                   0.468146854918318, 0.22409094644118732, 0.0018187078598082282],
+                                  [0.013443971409058638, 0.00017004327644987995, 0.021800496713184837,
+                                   0.00015993874500272996, 0.0010737559422562381, 0.720341361823655],
+                                  [0.00019960293232954552, 0.05281355668814136, 0.0016524909930692353,
+                                   0.5316932063366795, 0.7748352976165566, 0.27783993031653687]]], rtol=1e-20)).all()
+
         ## multiple samples
         samples = []
         obs_list = []
         obs = h.np.array([self.obs_options[j] for j in [0, 2, 0, 2, 2, 1]])
         samples.append(h.Sample(str(len(samples)), obs))
         obs_list.append(obs)
         obs = h.np.array([self.obs_options[j] for j in [0, 2, 0, 2, 2, 2]])
@@ -198,20 +208,40 @@
         expected_i = 0
         for obs_i, obs_l in model.sample_iterator():
             assert expected_i == obs_i
             expected_i += 1
             assert obs_l == [obs_list[i][obs_i] for i in range(model.n_samples)]
 
         # test HMM viterbi
-        # validated with hmmlearn https://github.com/hmmlearn/hmmlearn
         X = model.viterbi()
         assert h.np.array_equal(
             X, [[0, 0, 0, 2, 2, 1], [0, 0, 0, 2, 2, 2], [0, 2, 2, 2, 2, 1]]
         )
 
+        # test HMM forward and backward
+        X = model.fb()
+        assert (h.np.isclose(X, [[[0.9863564256586119, 0.947016400035409, 0.9765470122937462,
+                                   0.468146854918318, 0.22409094644118732, 0.0018187078598082282],
+                                  [0.013443971409058638, 0.00017004327644987995, 0.021800496713184837,
+                                   0.00015993874500272996, 0.0010737559422562381, 0.720341361823655],
+                                  [0.00019960293232954552, 0.05281355668814136, 0.0016524909930692353,
+                                   0.5316932063366795, 0.7748352976165566, 0.27783993031653687]],
+                                 [[0.9864079621924704, 0.9484260150301439, 0.9794416128395157,
+                                   0.5722878256369257, 0.38901397807144283, 0.3272832130980188],
+                                  [0.013396180157748403, 0.00016550412090882575, 0.019216705820730078,
+                                   0.00015107607088531594, 0.00013966620627958175, 0.0004817097551396808],
+                                  [0.000195857649781077, 0.05140848084894727, 0.0013416813397544164,
+                                   0.42756109829218925, 0.6108463557222777, 0.6722350771468416]],
+                                 [[0.9661426440798778, 0.3877838884083842, 0.0026400370796284354,
+                                   0.08193398763283319, 0.0536477277207047, 0.000630716939589588],
+                                  [0.032169997078295216, 0.0008175936570938669, 0.37504952065151326,
+                                   0.000613340413191413, 0.001039049071595767, 0.6999106907563121],
+                                  [0.0016873588418266088, 0.6113985179345218, 0.6223104422688582,
+                                   0.9174526719539753, 0.9453132232076995, 0.2994585923040983]]], rtol=1e-20)).all()
+
     def test_invalid_hmm(self):
         ## single sample
         samples = []
         obs = h.np.array([self.obs_options[j] for j in [0, 2, 0, 2, 2, 1]])
         samples.append(h.Sample(str(len(samples)), obs))
         initial_prob = [0.6, 0.2, 0.2]
```

### Comparing `cahmml-1.0.1/setup.py` & `cahmml-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['cahmml', 'cahmml.test']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.23.5,<2.0.0', 'rich>=12.6.0,<13.0.0']
+['numpy>=1.23.5', 'rich>=12.6.0']
 
 setup_kwargs = {
     'name': 'cahmml',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Custom Lambda HMM Library',
     'long_description': None,
     'author': 'Ryan Eveloff, Denghui Chen',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

