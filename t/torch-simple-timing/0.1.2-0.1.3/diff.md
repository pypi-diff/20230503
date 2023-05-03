# Comparing `tmp/torch_simple_timing-0.1.2.tar.gz` & `tmp/torch_simple_timing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_simple_timing-0.1.2.tar", max compression
+gzip compressed data, was "torch_simple_timing-0.1.3.tar", max compression
```

## Comparing `torch_simple_timing-0.1.2.tar` & `torch_simple_timing-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.2/LICENSE
--rw-r--r--   0        0        0     3354 2023-04-13 15:09:59.550673 torch_simple_timing-0.1.2/README.md
--rw-r--r--   0        0        0      648 2023-04-13 15:06:02.423029 torch_simple_timing-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      841 2023-04-12 23:05:33.657687 torch_simple_timing-0.1.2/torch_simple_timing/__init__.py
--rw-r--r--   0        0        0     8293 2023-04-12 22:55:21.559088 torch_simple_timing-0.1.2/torch_simple_timing/clock.py
--rw-r--r--   0        0        0    13141 2023-04-13 15:05:18.652967 torch_simple_timing-0.1.2/torch_simple_timing/timer.py
--rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.2/torch_simple_timing/utils.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.2/setup.py
--rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4468 2023-05-01 19:11:11.141712 torch_simple_timing-0.1.3/README.md
+-rw-r--r--   0        0        0      686 2023-05-02 20:09:54.663258 torch_simple_timing-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4665 2023-05-02 20:09:29.781149 torch_simple_timing-0.1.3/torch_simple_timing/__init__.py
+-rw-r--r--   0        0        0     8857 2023-05-01 19:11:11.142954 torch_simple_timing-0.1.3/torch_simple_timing/clock.py
+-rw-r--r--   0        0        0    13141 2023-05-01 18:44:28.717396 torch_simple_timing-0.1.3/torch_simple_timing/timer.py
+-rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.3/torch_simple_timing/utils.py
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.3/setup.py
+-rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.3/PKG-INFO
```

### Comparing `torch_simple_timing-0.1.2/LICENSE` & `torch_simple_timing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.2/README.md` & `torch_simple_timing-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 000003a0: 682d 7369 6d70 6c65 2d74 696d 696e 672f  h-simple-timing/
 000003b0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
 000003c0: 7372 633d 2268 7474 7073 3a2f 2f62 6164  src="https://bad
 000003d0: 6765 2e66 7572 792e 696f 2f70 792f 746f  ge.fury.io/py/to
 000003e0: 7263 685f 7369 6d70 6c65 5f74 696d 696e  rch_simple_timin
 000003f0: 672e 7376 6722 2061 6c74 3d22 5079 5049  g.svg" alt="PyPI
 00000400: 2076 6572 7369 6f6e 2220 6865 6967 6874   version" height
-00000410: 3d22 3138 223e 0a20 2020 203c 2f61 3e0a  ="18">.    </a>.
+00000410: 3d22 3230 223e 0a20 2020 203c 2f61 3e0a  ="20">.    </a>.
 00000420: 3c2f 703e 0a3c 6272 2f3e 0a0a 0a23 2054  </p>.<br/>...# T
 00000430: 6f72 6368 2053 696d 706c 6520 5469 6d69  orch Simple Timi
 00000440: 6e67 0a0a 4120 7369 6d70 6c65 2079 6574  ng..A simple yet
 00000450: 2076 6572 7361 7469 6c65 2070 6163 6b61   versatile packa
 00000460: 6765 2074 6f20 7469 6d65 2043 5055 2f47  ge to time CPU/G
 00000470: 5055 2f4d 756c 7469 2d47 5055 206f 7073  PU/Multi-GPU ops
 00000480: 2e0a 0a31 2e20 222a 4920 7761 6e74 2074  ...1. "*I want t
@@ -203,8 +203,78 @@
 00000ca0: 600a 0a60 6060 0a65 706f 6368 2020 2020  `..```.epoch    
 00000cb0: 3a20 302e 3235 3036 3420 c2b1 2030 2e30  : 0.25064 .. 0.0
 00000cc0: 3237 3238 2028 6e3d 3130 290a 666f 7277  2728 (n=10).forw
 00000cd0: 6172 6420 203a 2030 2e30 3032 3236 20c2  ard  : 0.00226 .
 00000ce0: b120 302e 3030 3532 3620 286e 3d35 3029  . 0.00526 (n=50)
 00000cf0: 0a62 6163 6b77 6172 6420 3a20 302e 3030  .backward : 0.00
 00000d00: 3230 3920 c2b1 2030 2e30 3033 3837 2028  209 .. 0.00387 (
-00000d10: 6e3d 3530 290a 6060 600a                 n=50).```.
+00000d10: 6e3d 3530 290a 6060 600a 0a23 2323 2041  n=50).```..### A
+00000d20: 2064 6563 6f72 6174 6f72 0a0a 596f 7520   decorator..You 
+00000d30: 6361 6e20 616c 736f 2075 7365 2061 2064  can also use a d
+00000d40: 6563 6f72 6174 6f72 2074 6f20 7469 6d65  ecorator to time
+00000d50: 2066 756e 6374 696f 6e73 2077 6974 686f   functions witho
+00000d60: 7574 206d 7563 6820 6f76 6572 6865 6164  ut much overhead
+00000d70: 2069 6e20 796f 7572 2063 6f64 653a 0a0a   in your code:..
+00000d80: 6060 6070 7974 686f 6e0a 6672 6f6d 2074  ```python.from t
+00000d90: 6f72 6368 5f73 696d 706c 655f 7469 6d69  orch_simple_timi
+00000da0: 6e67 2069 6d70 6f72 7420 7469 6d65 6974  ng import timeit
+00000db0: 2c20 6765 745f 676c 6f62 616c 5f74 696d  , get_global_tim
+00000dc0: 6572 2c20 7265 7365 745f 676c 6f62 616c  er, reset_global
+00000dd0: 5f74 696d 6572 0a69 6d70 6f72 7420 746f  _timer.import to
+00000de0: 7263 680a 0a23 2055 7365 2074 6865 2066  rch..# Use the f
+00000df0: 756e 6374 696f 6e20 6e61 6d65 2061 7320  unction name as 
+00000e00: 7468 6520 7469 6d65 7220 6e61 6d65 0a40  the timer name.@
+00000e10: 7469 6d65 6974 2867 7075 3d54 7275 6529  timeit(gpu=True)
+00000e20: 0a64 6566 2074 7261 696e 2829 3a0a 2020  .def train():.  
+00000e30: 2020 7820 3d20 746f 7263 682e 7261 6e64    x = torch.rand
+00000e40: 2831 3030 302c 2031 3030 302c 2064 6576  (1000, 1000, dev
+00000e50: 6963 653d 2263 7564 6122 2069 6620 746f  ice="cuda" if to
+00000e60: 7263 682e 6375 6461 2e69 735f 6176 6169  rch.cuda.is_avai
+00000e70: 6c61 626c 6528 2920 656c 7365 2022 6370  lable() else "cp
+00000e80: 7522 290a 2020 2020 7265 7475 726e 2074  u").    return t
+00000e90: 6f72 6368 2e69 6e76 6572 7365 2878 2040  orch.inverse(x @
+00000ea0: 2078 290a 0a23 2055 7365 2061 2063 7573   x)..# Use a cus
+00000eb0: 746f 6d20 6e61 6d65 0a40 7469 6d65 6974  tom name.@timeit
+00000ec0: 2822 7465 7374 2229 0a64 6566 2074 6573  ("test").def tes
+00000ed0: 745f 6370 7528 293a 0a20 2020 2072 6574  t_cpu():.    ret
+00000ee0: 7572 6e20 746f 7263 682e 696e 7665 7273  urn torch.invers
+00000ef0: 6528 746f 7263 682e 7261 6e64 2831 3030  e(torch.rand(100
+00000f00: 302c 2031 3030 3029 2040 2074 6f72 6368  0, 1000) @ torch
+00000f10: 2e72 616e 6428 3130 3030 2c20 3130 3030  .rand(1000, 1000
+00000f20: 2929 0a0a 6966 205f 5f6e 616d 655f 5f20  ))..if __name__ 
+00000f30: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
+00000f40: 2020 2066 6f72 205f 2069 6e20 7261 6e67     for _ in rang
+00000f50: 6528 2865 706f 6368 7320 3a3d 2031 3029  e((epochs := 10)
+00000f60: 293a 0a20 2020 2020 2020 2074 7261 696e  ):.        train
+00000f70: 2829 0a0a 2020 2020 7465 7374 5f63 7075  ()..    test_cpu
+00000f80: 2829 0a0a 2020 2020 7469 6d65 7220 3d20  ()..    timer = 
+00000f90: 6765 745f 676c 6f62 616c 5f74 696d 6572  get_global_timer
+00000fa0: 2829 0a20 2020 2070 7269 6e74 2874 696d  ().    print(tim
+00000fb0: 6572 2e64 6973 706c 6179 2829 290a 0a20  er.display()).. 
+00000fc0: 2020 2072 6573 6574 5f67 6c6f 6261 6c5f     reset_global_
+00000fd0: 7469 6d65 7228 290a 6060 600a 0a50 7269  timer().```..Pri
+00000fe0: 6e74 733a 0a0a 6060 6074 6578 740a 7472  nts:..```text.tr
+00000ff0: 6169 6e20 3a20 302e 3034 3520 c2b1 2030  ain : 0.045 .. 0
+00001000: 2e30 3037 2028 6e3d 3130 290a 7465 7374  .007 (n=10).test
+00001010: 2020 3a20 302e 3034 3620 2020 2020 2020    : 0.046       
+00001020: 2020 286e 3d20 3129 0a60 6060 0a0a 4279    (n= 1).```..By
+00001030: 2064 6566 6175 6c74 2074 6865 2060 4074   default the `@t
+00001040: 696d 6569 7460 2064 6563 6f64 7261 746f  imeit` decodrato
+00001050: 7220 7461 6b65 7320 6174 206c 6561 7374  r takes at least
+00001060: 2061 2060 6e61 6d65 602c 2077 696c 6c20   a `name`, will 
+00001070: 7573 6520 6067 7075 3d46 616c 7365 6020  use `gpu=False` 
+00001080: 616e 6420 7573 6520 7468 6520 676c 6f62  and use the glob
+00001090: 616c 2074 696d 6572 2028 6074 6f72 6368  al timer (`torch
+000010a0: 5f73 696d 706c 655f 7469 6d69 6e67 2e54  _simple_timing.T
+000010b0: 494d 4552 6029 2e20 596f 7520 6361 6e20  IMER`). You can 
+000010c0: 7061 7373 2079 6f75 7220 6f77 6e20 7469  pass your own ti
+000010d0: 6d65 7220 7769 7468 2060 4074 696d 6569  mer with `@timei
+000010e0: 7428 6e61 6d65 2c20 7469 6d65 723d 7469  t(name, timer=ti
+000010f0: 6d65 7229 602e 0a0a 5365 6520 5b69 6e20  mer)`...See [in 
+00001100: 7468 6520 646f 6373 5d28 5b68 7474 7073  the docs]([https
+00001110: 3a2f 2f5d 2868 7474 7073 3a2f 2f74 6f72  ://](https://tor
+00001120: 6368 2d73 696d 706c 652d 7469 6d69 6e67  ch-simple-timing
+00001130: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001140: 656e 2f6c 6174 6573 742f 6175 746f 6170  en/latest/autoap
+00001150: 692f 746f 7263 685f 7369 6d70 6c65 5f74  i/torch_simple_t
+00001160: 696d 696e 672f 696e 6465 782e 6874 6d6c  iming/index.html
+00001170: 2929 2e0a                                ))..
```

### Comparing `torch_simple_timing-0.1.2/pyproject.toml` & `torch_simple_timing-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "torch-simple-timing"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple package to time CPU/GPU/Multi-GPU ops"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_simple_timing"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 torch = ">=1.11"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 ipython = "^8.12.0"
 sphinx = "^6.1.3"
 myst-parser = "^1.0.0"
 furo = "^2023.3.27"
 sphinx-copybutton = "^0.5.1"
 sphinx-autodoc-typehints = "^1.22"
 sphinx-autoapi = "^2.1.0"
 sphinx-math-dollar = "^1.2.1"
+black = "^23.3.0"
+flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `torch_simple_timing-0.1.2/torch_simple_timing/clock.py` & `torch_simple_timing-0.1.3/torch_simple_timing/clock.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,19 +57,22 @@
     print(clock_no_store.duration)
     print(clock_list_store.store)
     print(full_clock.store)
 
 
 """
 
+import warnings
 from time import time
-from typing import Dict, List, Optional, Hashable
-from torch_simple_timing.utils import synchronize
+from typing import Dict, Hashable, List, Optional
+
 import torch
 
+from torch_simple_timing.utils import synchronize
+
 
 class Clock:
     def __init__(
         self,
         name: Optional[str] = None,
         store: Optional[Dict[str, List]] = None,
         gpu: Optional[bool] = False,
@@ -116,15 +119,31 @@
                     raise TypeError(
                         "`name` must be hashable because it is "
                         + "used as a key in the store dict"
                     )
                 if self.name not in self.store:
                     self.store[self.name] = []
 
-    def __enter__(self):
+        self._check_gpu()
+
+    def _check_gpu(self) -> None:
+        """
+        Checks if GPU timing is requested and if a GPU is available.
+        Throws a warning if GPU timing is requested but no GPU is available.
+
+        Sets ``self.gpu`` to ``False`` if no GPU is available.
+        """
+        if self.gpu and not torch.cuda.is_available():
+            warnings.warn(
+                "GPU timing requested but no GPU found. Setting `gpu` to False.",
+                RuntimeWarning,
+            )
+            self.gpu = False
+
+    def __enter__(self) -> "Clock":
         """
         Starts the timer.
 
         Returns:
             self: The Clock instance.
         """
         return self.start()
```

### Comparing `torch_simple_timing-0.1.2/torch_simple_timing/timer.py` & `torch_simple_timing-0.1.3/torch_simple_timing/timer.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.2/torch_simple_timing/utils.py` & `torch_simple_timing-0.1.3/torch_simple_timing/utils.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.2/setup.py` & `torch_simple_timing-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.11']
 
 setup_kwargs = {
     'name': 'torch-simple-timing',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
-    'long_description': '<p align="center">\n<strong><a href="https://github.com/vict0rsch/torch_simple_timing" target="_blank">💻&nbsp;&nbsp;Code</a></strong>\n<strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>\n<strong><a href="https://torch-simple-timing.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>\n</p>\n\n<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.8%2B-blue\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://torch-simple-timing.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/torch-simple-timing/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a href="https://github.com/psf/black">\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n    <a href="https://pytorch.org">\n        <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>\n    </a>\n    <a href="https://pypi.org/project/torch-simple-timing/">\n        <img src="https://badge.fury.io/py/torch_simple_timing.svg" alt="PyPI version" height="18">\n    </a>\n</p>\n<br/>\n\n\n# Torch Simple Timing\n\nA simple yet versatile package to time CPU/GPU/Multi-GPU ops.\n\n1. "*I want to time operations once*"\n   1. That\'s what a `Clock` is for\n2. "*I want to time the same operations multiple times*"\n   1. That\'s what a `Timer` is for\n\nIn simple terms:\n\n* A `Clock` is an object (and context-manager) that will compute the ellapsed time between its `start()` (or `__enter__`) and `stop()` (or `__exit__`)\n* A `Timer` will internally manage clocks so that you can focus on readability and not data structures\n\n## Installation\n\n```\npip install torch_simple_timing\n```\n\n## How to use\n\n### A `Clock`\n\n```python\nfrom torch_simple_parsing import Clock\nimport torch\n\nt = torch.rand(2000, 2000)\ngpu = torch.cuda.is_available()\n\nwith Clock(gpu=gpu) as context_clock:\n    torch.inverse(t @ t.T)\n\nclock = Clock(gpu=gpu).start()\ntorch.inverse(t @ t.T)\nclock.stop()\n\nprint(context_clock.duration) # 0.29688501358032227\nprint(clock.duration)         # 0.292896032333374\n```\n\nMore examples, including bout how to easily share data structures using a `store` can be found in the [documentation](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/torch_simple_timing/clock/index.html).\n\n### A `Timer`\n\n```python\nfrom torch_simple_timing import Timer\nimport torch\n\ndevice = torch.device("cuda" if torch.cuda.is_available() else "cpu")\n\nX = torch.rand(5000, 5000, device=device)\nY = torch.rand(5000, 100, device=device)\nmodel = torch.nn.Linear(5000, 100).to(device)\noptimizer = torch.optim.Adam(model.parameters())\n\ngpu = device.type == "cuda"\ntimer = Timer(gpu=gpu)\n\nfor epoch in range(10):\n    timer.clock("epoch").start()\n    for b in range(50):\n        x = X[b*100: (b+1)*100]\n        y = Y[b*100: (b+1)*100]\n        optimizer.zero_grad()\n        with timer.clock("forward", ignore=epoch>0):\n            p = model(x)\n        loss = torch.nn.functional.cross_entropy(p, y)\n        with timer.clock("backward", ignore=epoch>0):\n            loss.backward()\n        optimizer.step()\n    timer.clock("epoch").stop()\n\nstats = timer.stats()\n# use stats for display and/or logging\n# wandb.summary.update(stats)\nprint(timer.display(stats=stats, precision=5))\n```\n\n```\nepoch    : 0.25064 ± 0.02728 (n=10)\nforward  : 0.00226 ± 0.00526 (n=50)\nbackward : 0.00209 ± 0.00387 (n=50)\n```\n',
+    'long_description': '<p align="center">\n<strong><a href="https://github.com/vict0rsch/torch_simple_timing" target="_blank">💻&nbsp;&nbsp;Code</a></strong>\n<strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>\n<strong><a href="https://torch-simple-timing.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>\n</p>\n\n<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.8%2B-blue\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://torch-simple-timing.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/torch-simple-timing/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a href="https://github.com/psf/black">\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n    <a href="https://pytorch.org">\n        <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>\n    </a>\n    <a href="https://pypi.org/project/torch-simple-timing/">\n        <img src="https://badge.fury.io/py/torch_simple_timing.svg" alt="PyPI version" height="20">\n    </a>\n</p>\n<br/>\n\n\n# Torch Simple Timing\n\nA simple yet versatile package to time CPU/GPU/Multi-GPU ops.\n\n1. "*I want to time operations once*"\n   1. That\'s what a `Clock` is for\n2. "*I want to time the same operations multiple times*"\n   1. That\'s what a `Timer` is for\n\nIn simple terms:\n\n* A `Clock` is an object (and context-manager) that will compute the ellapsed time between its `start()` (or `__enter__`) and `stop()` (or `__exit__`)\n* A `Timer` will internally manage clocks so that you can focus on readability and not data structures\n\n## Installation\n\n```\npip install torch_simple_timing\n```\n\n## How to use\n\n### A `Clock`\n\n```python\nfrom torch_simple_parsing import Clock\nimport torch\n\nt = torch.rand(2000, 2000)\ngpu = torch.cuda.is_available()\n\nwith Clock(gpu=gpu) as context_clock:\n    torch.inverse(t @ t.T)\n\nclock = Clock(gpu=gpu).start()\ntorch.inverse(t @ t.T)\nclock.stop()\n\nprint(context_clock.duration) # 0.29688501358032227\nprint(clock.duration)         # 0.292896032333374\n```\n\nMore examples, including bout how to easily share data structures using a `store` can be found in the [documentation](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/torch_simple_timing/clock/index.html).\n\n### A `Timer`\n\n```python\nfrom torch_simple_timing import Timer\nimport torch\n\ndevice = torch.device("cuda" if torch.cuda.is_available() else "cpu")\n\nX = torch.rand(5000, 5000, device=device)\nY = torch.rand(5000, 100, device=device)\nmodel = torch.nn.Linear(5000, 100).to(device)\noptimizer = torch.optim.Adam(model.parameters())\n\ngpu = device.type == "cuda"\ntimer = Timer(gpu=gpu)\n\nfor epoch in range(10):\n    timer.clock("epoch").start()\n    for b in range(50):\n        x = X[b*100: (b+1)*100]\n        y = Y[b*100: (b+1)*100]\n        optimizer.zero_grad()\n        with timer.clock("forward", ignore=epoch>0):\n            p = model(x)\n        loss = torch.nn.functional.cross_entropy(p, y)\n        with timer.clock("backward", ignore=epoch>0):\n            loss.backward()\n        optimizer.step()\n    timer.clock("epoch").stop()\n\nstats = timer.stats()\n# use stats for display and/or logging\n# wandb.summary.update(stats)\nprint(timer.display(stats=stats, precision=5))\n```\n\n```\nepoch    : 0.25064 ± 0.02728 (n=10)\nforward  : 0.00226 ± 0.00526 (n=50)\nbackward : 0.00209 ± 0.00387 (n=50)\n```\n\n### A decorator\n\nYou can also use a decorator to time functions without much overhead in your code:\n\n```python\nfrom torch_simple_timing import timeit, get_global_timer, reset_global_timer\nimport torch\n\n# Use the function name as the timer name\n@timeit(gpu=True)\ndef train():\n    x = torch.rand(1000, 1000, device="cuda" if torch.cuda.is_available() else "cpu")\n    return torch.inverse(x @ x)\n\n# Use a custom name\n@timeit("test")\ndef test_cpu():\n    return torch.inverse(torch.rand(1000, 1000) @ torch.rand(1000, 1000))\n\nif __name__ == "__main__":\n    for _ in range((epochs := 10)):\n        train()\n\n    test_cpu()\n\n    timer = get_global_timer()\n    print(timer.display())\n\n    reset_global_timer()\n```\n\nPrints:\n\n```text\ntrain : 0.045 ± 0.007 (n=10)\ntest  : 0.046         (n= 1)\n```\n\nBy default the `@timeit` decodrator takes at least a `name`, will use `gpu=False` and use the global timer (`torch_simple_timing.TIMER`). You can pass your own timer with `@timeit(name, timer=timer)`.\n\nSee [in the docs]([https://](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/torch_simple_timing/index.html)).\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['torch_simple_timing'] package_data = \ {'': ['*']} install_requires = \
 ['torch>=1.11'] setup_kwargs = { 'name': 'torch-simple-timing', 'version':
-'0.1.2', 'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
+'0.1.3', 'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
 'long_description': '
                       \nð»  Code\n  â¢  \nDocs  ð\n
 \n\n
   \n \n\t [\'Python\']\n\t\n\t\n_\t'_/>\n\t\n \n\t_[\'https://img.shields.io/
    badge/code%20style-black-black\']\n\t\n \n_[https://img.shields.io/badge/
  PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white]\n\n \n_[PyPI_version]\n\n
 \n
@@ -35,12 +35,26 @@
 b in range(50):\n x = X[b*100: (b+1)*100]\n y = Y[b*100: (b+1)*100]\n
 optimizer.zero_grad()\n with timer.clock("forward", ignore=epoch>0):\n p =
 model(x)\n loss = torch.nn.functional.cross_entropy(p, y)\n with timer.clock
 ("backward", ignore=epoch>0):\n loss.backward()\n optimizer.step()\n
 timer.clock("epoch").stop()\n\nstats = timer.stats()\n# use stats for display
 and/or logging\n# wandb.summary.update(stats)\nprint(timer.display(stats=stats,
 precision=5))\n```\n\n```\nepoch : 0.25064 Â± 0.02728 (n=10)\nforward : 0.00226
-Â± 0.00526 (n=50)\nbackward : 0.00209 Â± 0.00387 (n=50)\n```\n', 'author':
-'vict0rsch', 'author_email': 'vsch@pm.me', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+Â± 0.00526 (n=50)\nbackward : 0.00209 Â± 0.00387 (n=50)\n```\n\n### A
+decorator\n\nYou can also use a decorator to time functions without much
+overhead in your code:\n\n```python\nfrom torch_simple_timing import timeit,
+get_global_timer, reset_global_timer\nimport torch\n\n# Use the function name
+as the timer name\n@timeit(gpu=True)\ndef train():\n x = torch.rand(1000, 1000,
+device="cuda" if torch.cuda.is_available() else "cpu")\n return torch.inverse(x
+@ x)\n\n# Use a custom name\n@timeit("test")\ndef test_cpu():\n return
+torch.inverse(torch.rand(1000, 1000) @ torch.rand(1000, 1000))\n\nif __name__
+== "__main__":\n for _ in range((epochs := 10)):\n train()\n\n test_cpu()\n\n
+timer = get_global_timer()\n print(timer.display())\n\n reset_global_timer
+()\n```\n\nPrints:\n\n```text\ntrain : 0.045 Â± 0.007 (n=10)\ntest : 0.046 (n=
+1)\n```\n\nBy default the `@timeit` decodrator takes at least a `name`, will
+use `gpu=False` and use the global timer (`torch_simple_timing.TIMER`). You can
+pass your own timer with `@timeit(name, timer=timer)`.\n\nSee [in the docs](
+[https://](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/
+torch_simple_timing/index.html)).\n', 'author': 'vict0rsch', 'author_email':
+'vsch@pm.me', 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None',
+'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'python_requires': '>=3.8.1,<4.0.0', } setup(**setup_kwargs)
```

### Comparing `torch_simple_timing-0.1.2/PKG-INFO` & `torch_simple_timing-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,246 +1,313 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746f 7263  : 2.1.Name: torc
 00000020: 682d 7369 6d70 6c65 2d74 696d 696e 670a  h-simple-timing.
-00000030: 5665 7273 696f 6e3a 2030 2e31 2e32 0a53  Version: 0.1.2.S
+00000030: 5665 7273 696f 6e3a 2030 2e31 2e33 0a53  Version: 0.1.3.S
 00000040: 756d 6d61 7279 3a20 4120 7369 6d70 6c65  ummary: A simple
 00000050: 2070 6163 6b61 6765 2074 6f20 7469 6d65   package to time
 00000060: 2043 5055 2f47 5055 2f4d 756c 7469 2d47   CPU/GPU/Multi-G
 00000070: 5055 206f 7073 0a4c 6963 656e 7365 3a20  PU ops.License: 
 00000080: 4d49 540a 4175 7468 6f72 3a20 7669 6374  MIT.Author: vict
 00000090: 3072 7363 680a 4175 7468 6f72 2d65 6d61  0rsch.Author-ema
 000000a0: 696c 3a20 7673 6368 4070 6d2e 6d65 0a52  il: vsch@pm.me.R
 000000b0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000000c0: 3e3d 332e 382c 3c34 2e30 0a43 6c61 7373  >=3.8,<4.0.Class
-000000d0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000000e0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000000f0: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
-00000100: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000110: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000120: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-00000130: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000140: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000150: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-00000160: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000170: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000180: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000190: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
-000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
-000001d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001f0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
-00000200: 2d44 6973 743a 2074 6f72 6368 2028 3e3d  -Dist: torch (>=
-00000210: 312e 3131 290a 4465 7363 7269 7074 696f  1.11).Descriptio
-00000220: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000230: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
-00000240: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000250: 3e0a 3c73 7472 6f6e 673e 3c61 2068 7265  >.<strong><a hre
-00000260: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000270: 622e 636f 6d2f 7669 6374 3072 7363 682f  b.com/vict0rsch/
-00000280: 746f 7263 685f 7369 6d70 6c65 5f74 696d  torch_simple_tim
-00000290: 696e 6722 2074 6172 6765 743d 225f 626c  ing" target="_bl
-000002a0: 616e 6b22 3ef0 9f92 bb26 6e62 7370 3b26  ank">....&nbsp;&
-000002b0: 6e62 7370 3b43 6f64 653c 2f61 3e3c 2f73  nbsp;Code</a></s
-000002c0: 7472 6f6e 673e 0a3c 7374 726f 6e67 3e26  trong>.<strong>&
-000002d0: 6e62 7370 3b26 6e62 7370 3be2 80a2 266e  nbsp;&nbsp;...&n
-000002e0: 6273 703b 266e 6273 703b 3c2f 7374 726f  bsp;&nbsp;</stro
-000002f0: 6e67 3e0a 3c73 7472 6f6e 673e 3c61 2068  ng>.<strong><a h
-00000300: 7265 663d 2268 7474 7073 3a2f 2f74 6f72  ref="https://tor
-00000310: 6368 2d73 696d 706c 652d 7469 6d69 6e67  ch-simple-timing
-00000320: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000330: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000340: 223e 446f 6373 266e 6273 703b 266e 6273  ">Docs&nbsp;&nbs
-00000350: 703b f09f 9391 3c2f 613e 3c2f 7374 726f  p;....</a></stro
-00000360: 6e67 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  ng>.</p>..<p ali
-00000370: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
-00000380: 203c 613e 0a09 2020 2020 3c69 6d67 2073   <a>..    <img s
-00000390: 7263 3d27 6874 7470 733a 2f2f 696d 672e  rc='https://img.
-000003a0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-000003b0: 2f70 7974 686f 6e2d 332e 3825 3242 2d62  /python-3.8%2B-b
-000003c0: 6c75 6527 2061 6c74 3d27 5079 7468 6f6e  lue' alt='Python
-000003d0: 2720 2f3e 0a09 3c2f 613e 0a09 3c61 2068  ' />..</a>..<a h
-000003e0: 7265 663d 2768 7474 7073 3a2f 2f74 6f72  ref='https://tor
-000003f0: 6368 2d73 696d 706c 652d 7469 6d69 6e67  ch-simple-timing
-00000400: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000410: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-00000420: 3d6c 6174 6573 7427 3e0a 2020 2020 093c  =latest'>.    .<
-00000430: 696d 6720 7372 633d 2768 7474 7073 3a2f  img src='https:/
-00000440: 2f72 6561 6474 6865 646f 6373 2e6f 7267  /readthedocs.org
-00000450: 2f70 726f 6a65 6374 732f 746f 7263 682d  /projects/torch-
-00000460: 7369 6d70 6c65 2d74 696d 696e 672f 6261  simple-timing/ba
-00000470: 6467 652f 3f76 6572 7369 6f6e 3d6c 6174  dge/?version=lat
-00000480: 6573 7427 2061 6c74 3d27 446f 6375 6d65  est' alt='Docume
-00000490: 6e74 6174 696f 6e20 5374 6174 7573 2720  ntation Status' 
-000004a0: 2f3e 0a09 3c2f 613e 0a20 2020 203c 6120  />..</a>.    <a 
-000004b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000004c0: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-000004d0: 636b 223e 0a09 2020 2020 3c69 6d67 2073  ck">..    <img s
-000004e0: 7263 3d27 6874 7470 733a 2f2f 696d 672e  rc='https://img.
-000004f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000500: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
-00000510: 6163 6b2d 626c 6163 6b27 202f 3e0a 093c  ack-black' />..<
-00000520: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
-00000530: 2268 7474 7073 3a2f 2f70 7974 6f72 6368  "https://pytorch
-00000540: 2e6f 7267 223e 0a20 2020 2020 2020 203c  .org">.        <
-00000550: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000560: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000570: 6261 6467 652f 5079 546f 7263 682d 2532  badge/PyTorch-%2
-00000580: 3345 4534 4332 432e 7376 673f 6c6f 676f  3EE4C2C.svg?logo
-00000590: 3d50 7954 6f72 6368 266c 6f67 6f43 6f6c  =PyTorch&logoCol
-000005a0: 6f72 3d77 6869 7465 222f 3e0a 2020 2020  or=white"/>.    
-000005b0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
-000005c0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-000005d0: 7267 2f70 726f 6a65 6374 2f74 6f72 6368  rg/project/torch
-000005e0: 2d73 696d 706c 652d 7469 6d69 6e67 2f22  -simple-timing/"
-000005f0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00000600: 7263 3d22 6874 7470 733a 2f2f 6261 6467  rc="https://badg
-00000610: 652e 6675 7279 2e69 6f2f 7079 2f74 6f72  e.fury.io/py/tor
-00000620: 6368 5f73 696d 706c 655f 7469 6d69 6e67  ch_simple_timing
-00000630: 2e73 7667 2220 616c 743d 2250 7950 4920  .svg" alt="PyPI 
-00000640: 7665 7273 696f 6e22 2068 6569 6768 743d  version" height=
-00000650: 2231 3822 3e0a 2020 2020 3c2f 613e 0a3c  "18">.    </a>.<
-00000660: 2f70 3e0a 3c62 722f 3e0a 0a0a 2320 546f  /p>.<br/>...# To
-00000670: 7263 6820 5369 6d70 6c65 2054 696d 696e  rch Simple Timin
-00000680: 670a 0a41 2073 696d 706c 6520 7965 7420  g..A simple yet 
-00000690: 7665 7273 6174 696c 6520 7061 636b 6167  versatile packag
-000006a0: 6520 746f 2074 696d 6520 4350 552f 4750  e to time CPU/GP
-000006b0: 552f 4d75 6c74 692d 4750 5520 6f70 732e  U/Multi-GPU ops.
-000006c0: 0a0a 312e 2022 2a49 2077 616e 7420 746f  ..1. "*I want to
-000006d0: 2074 696d 6520 6f70 6572 6174 696f 6e73   time operations
-000006e0: 206f 6e63 652a 220a 2020 2031 2e20 5468   once*".   1. Th
-000006f0: 6174 2773 2077 6861 7420 6120 6043 6c6f  at's what a `Clo
-00000700: 636b 6020 6973 2066 6f72 0a32 2e20 222a  ck` is for.2. "*
-00000710: 4920 7761 6e74 2074 6f20 7469 6d65 2074  I want to time t
-00000720: 6865 2073 616d 6520 6f70 6572 6174 696f  he same operatio
-00000730: 6e73 206d 756c 7469 706c 6520 7469 6d65  ns multiple time
-00000740: 732a 220a 2020 2031 2e20 5468 6174 2773  s*".   1. That's
-00000750: 2077 6861 7420 6120 6054 696d 6572 6020   what a `Timer` 
-00000760: 6973 2066 6f72 0a0a 496e 2073 696d 706c  is for..In simpl
-00000770: 6520 7465 726d 733a 0a0a 2a20 4120 6043  e terms:..* A `C
-00000780: 6c6f 636b 6020 6973 2061 6e20 6f62 6a65  lock` is an obje
-00000790: 6374 2028 616e 6420 636f 6e74 6578 742d  ct (and context-
-000007a0: 6d61 6e61 6765 7229 2074 6861 7420 7769  manager) that wi
-000007b0: 6c6c 2063 6f6d 7075 7465 2074 6865 2065  ll compute the e
-000007c0: 6c6c 6170 7365 6420 7469 6d65 2062 6574  llapsed time bet
-000007d0: 7765 656e 2069 7473 2060 7374 6172 7428  ween its `start(
-000007e0: 2960 2028 6f72 2060 5f5f 656e 7465 725f  )` (or `__enter_
-000007f0: 5f60 2920 616e 6420 6073 746f 7028 2960  _`) and `stop()`
-00000800: 2028 6f72 2060 5f5f 6578 6974 5f5f 6029   (or `__exit__`)
-00000810: 0a2a 2041 2060 5469 6d65 7260 2077 696c  .* A `Timer` wil
-00000820: 6c20 696e 7465 726e 616c 6c79 206d 616e  l internally man
-00000830: 6167 6520 636c 6f63 6b73 2073 6f20 7468  age clocks so th
-00000840: 6174 2079 6f75 2063 616e 2066 6f63 7573  at you can focus
-00000850: 206f 6e20 7265 6164 6162 696c 6974 7920   on readability 
-00000860: 616e 6420 6e6f 7420 6461 7461 2073 7472  and not data str
-00000870: 7563 7475 7265 730a 0a23 2320 496e 7374  uctures..## Inst
-00000880: 616c 6c61 7469 6f6e 0a0a 6060 600a 7069  allation..```.pi
-00000890: 7020 696e 7374 616c 6c20 746f 7263 685f  p install torch_
-000008a0: 7369 6d70 6c65 5f74 696d 696e 670a 6060  simple_timing.``
-000008b0: 600a 0a23 2320 486f 7720 746f 2075 7365  `..## How to use
-000008c0: 0a0a 2323 2320 4120 6043 6c6f 636b 600a  ..### A `Clock`.
-000008d0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-000008e0: 746f 7263 685f 7369 6d70 6c65 5f70 6172  torch_simple_par
-000008f0: 7369 6e67 2069 6d70 6f72 7420 436c 6f63  sing import Cloc
-00000900: 6b0a 696d 706f 7274 2074 6f72 6368 0a0a  k.import torch..
-00000910: 7420 3d20 746f 7263 682e 7261 6e64 2832  t = torch.rand(2
-00000920: 3030 302c 2032 3030 3029 0a67 7075 203d  000, 2000).gpu =
-00000930: 2074 6f72 6368 2e63 7564 612e 6973 5f61   torch.cuda.is_a
-00000940: 7661 696c 6162 6c65 2829 0a0a 7769 7468  vailable()..with
-00000950: 2043 6c6f 636b 2867 7075 3d67 7075 2920   Clock(gpu=gpu) 
-00000960: 6173 2063 6f6e 7465 7874 5f63 6c6f 636b  as context_clock
-00000970: 3a0a 2020 2020 746f 7263 682e 696e 7665  :.    torch.inve
-00000980: 7273 6528 7420 4020 742e 5429 0a0a 636c  rse(t @ t.T)..cl
-00000990: 6f63 6b20 3d20 436c 6f63 6b28 6770 753d  ock = Clock(gpu=
-000009a0: 6770 7529 2e73 7461 7274 2829 0a74 6f72  gpu).start().tor
-000009b0: 6368 2e69 6e76 6572 7365 2874 2040 2074  ch.inverse(t @ t
-000009c0: 2e54 290a 636c 6f63 6b2e 7374 6f70 2829  .T).clock.stop()
-000009d0: 0a0a 7072 696e 7428 636f 6e74 6578 745f  ..print(context_
-000009e0: 636c 6f63 6b2e 6475 7261 7469 6f6e 2920  clock.duration) 
-000009f0: 2320 302e 3239 3638 3835 3031 3335 3830  # 0.296885013580
-00000a00: 3332 3232 370a 7072 696e 7428 636c 6f63  32227.print(cloc
-00000a10: 6b2e 6475 7261 7469 6f6e 2920 2020 2020  k.duration)     
-00000a20: 2020 2020 2320 302e 3239 3238 3936 3033      # 0.29289603
-00000a30: 3233 3333 3337 340a 6060 600a 0a4d 6f72  2333374.```..Mor
-00000a40: 6520 6578 616d 706c 6573 2c20 696e 636c  e examples, incl
-00000a50: 7564 696e 6720 626f 7574 2068 6f77 2074  uding bout how t
-00000a60: 6f20 6561 7369 6c79 2073 6861 7265 2064  o easily share d
-00000a70: 6174 6120 7374 7275 6374 7572 6573 2075  ata structures u
-00000a80: 7369 6e67 2061 2060 7374 6f72 6560 2063  sing a `store` c
-00000a90: 616e 2062 6520 666f 756e 6420 696e 2074  an be found in t
-00000aa0: 6865 205b 646f 6375 6d65 6e74 6174 696f  he [documentatio
-00000ab0: 6e5d 2868 7474 7073 3a2f 2f74 6f72 6368  n](https://torch
-00000ac0: 2d73 696d 706c 652d 7469 6d69 6e67 2e72  -simple-timing.r
-00000ad0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000ae0: 2f6c 6174 6573 742f 6175 746f 6170 692f  /latest/autoapi/
-00000af0: 746f 7263 685f 7369 6d70 6c65 5f74 696d  torch_simple_tim
-00000b00: 696e 672f 636c 6f63 6b2f 696e 6465 782e  ing/clock/index.
-00000b10: 6874 6d6c 292e 0a0a 2323 2320 4120 6054  html)...### A `T
-00000b20: 696d 6572 600a 0a60 6060 7079 7468 6f6e  imer`..```python
-00000b30: 0a66 726f 6d20 746f 7263 685f 7369 6d70  .from torch_simp
-00000b40: 6c65 5f74 696d 696e 6720 696d 706f 7274  le_timing import
-00000b50: 2054 696d 6572 0a69 6d70 6f72 7420 746f   Timer.import to
-00000b60: 7263 680a 0a64 6576 6963 6520 3d20 746f  rch..device = to
-00000b70: 7263 682e 6465 7669 6365 2822 6375 6461  rch.device("cuda
-00000b80: 2220 6966 2074 6f72 6368 2e63 7564 612e  " if torch.cuda.
-00000b90: 6973 5f61 7661 696c 6162 6c65 2829 2065  is_available() e
-00000ba0: 6c73 6520 2263 7075 2229 0a0a 5820 3d20  lse "cpu")..X = 
-00000bb0: 746f 7263 682e 7261 6e64 2835 3030 302c  torch.rand(5000,
-00000bc0: 2035 3030 302c 2064 6576 6963 653d 6465   5000, device=de
-00000bd0: 7669 6365 290a 5920 3d20 746f 7263 682e  vice).Y = torch.
-00000be0: 7261 6e64 2835 3030 302c 2031 3030 2c20  rand(5000, 100, 
-00000bf0: 6465 7669 6365 3d64 6576 6963 6529 0a6d  device=device).m
-00000c00: 6f64 656c 203d 2074 6f72 6368 2e6e 6e2e  odel = torch.nn.
-00000c10: 4c69 6e65 6172 2835 3030 302c 2031 3030  Linear(5000, 100
-00000c20: 292e 746f 2864 6576 6963 6529 0a6f 7074  ).to(device).opt
-00000c30: 696d 697a 6572 203d 2074 6f72 6368 2e6f  imizer = torch.o
-00000c40: 7074 696d 2e41 6461 6d28 6d6f 6465 6c2e  ptim.Adam(model.
-00000c50: 7061 7261 6d65 7465 7273 2829 290a 0a67  parameters())..g
-00000c60: 7075 203d 2064 6576 6963 652e 7479 7065  pu = device.type
-00000c70: 203d 3d20 2263 7564 6122 0a74 696d 6572   == "cuda".timer
-00000c80: 203d 2054 696d 6572 2867 7075 3d67 7075   = Timer(gpu=gpu
-00000c90: 290a 0a66 6f72 2065 706f 6368 2069 6e20  )..for epoch in 
-00000ca0: 7261 6e67 6528 3130 293a 0a20 2020 2074  range(10):.    t
-00000cb0: 696d 6572 2e63 6c6f 636b 2822 6570 6f63  imer.clock("epoc
-00000cc0: 6822 292e 7374 6172 7428 290a 2020 2020  h").start().    
-00000cd0: 666f 7220 6220 696e 2072 616e 6765 2835  for b in range(5
-00000ce0: 3029 3a0a 2020 2020 2020 2020 7820 3d20  0):.        x = 
-00000cf0: 585b 622a 3130 303a 2028 622b 3129 2a31  X[b*100: (b+1)*1
-00000d00: 3030 5d0a 2020 2020 2020 2020 7920 3d20  00].        y = 
-00000d10: 595b 622a 3130 303a 2028 622b 3129 2a31  Y[b*100: (b+1)*1
-00000d20: 3030 5d0a 2020 2020 2020 2020 6f70 7469  00].        opti
-00000d30: 6d69 7a65 722e 7a65 726f 5f67 7261 6428  mizer.zero_grad(
-00000d40: 290a 2020 2020 2020 2020 7769 7468 2074  ).        with t
-00000d50: 696d 6572 2e63 6c6f 636b 2822 666f 7277  imer.clock("forw
-00000d60: 6172 6422 2c20 6967 6e6f 7265 3d65 706f  ard", ignore=epo
-00000d70: 6368 3e30 293a 0a20 2020 2020 2020 2020  ch>0):.         
-00000d80: 2020 2070 203d 206d 6f64 656c 2878 290a     p = model(x).
-00000d90: 2020 2020 2020 2020 6c6f 7373 203d 2074          loss = t
-00000da0: 6f72 6368 2e6e 6e2e 6675 6e63 7469 6f6e  orch.nn.function
-00000db0: 616c 2e63 726f 7373 5f65 6e74 726f 7079  al.cross_entropy
-00000dc0: 2870 2c20 7929 0a20 2020 2020 2020 2077  (p, y).        w
-00000dd0: 6974 6820 7469 6d65 722e 636c 6f63 6b28  ith timer.clock(
-00000de0: 2262 6163 6b77 6172 6422 2c20 6967 6e6f  "backward", igno
-00000df0: 7265 3d65 706f 6368 3e30 293a 0a20 2020  re=epoch>0):.   
-00000e00: 2020 2020 2020 2020 206c 6f73 732e 6261           loss.ba
-00000e10: 636b 7761 7264 2829 0a20 2020 2020 2020  ckward().       
-00000e20: 206f 7074 696d 697a 6572 2e73 7465 7028   optimizer.step(
-00000e30: 290a 2020 2020 7469 6d65 722e 636c 6f63  ).    timer.cloc
-00000e40: 6b28 2265 706f 6368 2229 2e73 746f 7028  k("epoch").stop(
-00000e50: 290a 0a73 7461 7473 203d 2074 696d 6572  )..stats = timer
-00000e60: 2e73 7461 7473 2829 0a23 2075 7365 2073  .stats().# use s
-00000e70: 7461 7473 2066 6f72 2064 6973 706c 6179  tats for display
-00000e80: 2061 6e64 2f6f 7220 6c6f 6767 696e 670a   and/or logging.
-00000e90: 2320 7761 6e64 622e 7375 6d6d 6172 792e  # wandb.summary.
-00000ea0: 7570 6461 7465 2873 7461 7473 290a 7072  update(stats).pr
-00000eb0: 696e 7428 7469 6d65 722e 6469 7370 6c61  int(timer.displa
-00000ec0: 7928 7374 6174 733d 7374 6174 732c 2070  y(stats=stats, p
-00000ed0: 7265 6369 7369 6f6e 3d35 2929 0a60 6060  recision=5)).```
-00000ee0: 0a0a 6060 600a 6570 6f63 6820 2020 203a  ..```.epoch    :
-00000ef0: 2030 2e32 3530 3634 20c2 b120 302e 3032   0.25064 .. 0.02
-00000f00: 3732 3820 286e 3d31 3029 0a66 6f72 7761  728 (n=10).forwa
-00000f10: 7264 2020 3a20 302e 3030 3232 3620 c2b1  rd  : 0.00226 ..
-00000f20: 2030 2e30 3035 3236 2028 6e3d 3530 290a   0.00526 (n=50).
-00000f30: 6261 636b 7761 7264 203a 2030 2e30 3032  backward : 0.002
-00000f40: 3039 20c2 b120 302e 3030 3338 3720 286e  09 .. 0.00387 (n
-00000f50: 3d35 3029 0a60 6060 0a0a                 =50).```..
+000000c0: 3e3d 332e 382e 312c 3c34 2e30 2e30 0a43  >=3.8.1,<4.0.0.C
+000000d0: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000000e0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000000f0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000100: 650a 436c 6173 7369 6669 6572 3a20 5072  e.Classifier: Pr
+00000110: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000120: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000130: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
+00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000160: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+00000170: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000180: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000190: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
+000001d0: 6573 2d44 6973 743a 2074 6f72 6368 2028  es-Dist: torch (
+000001e0: 3e3d 312e 3131 290a 4465 7363 7269 7074  >=1.11).Descript
+000001f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000200: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000210: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000220: 7222 3e0a 3c73 7472 6f6e 673e 3c61 2068  r">.<strong><a h
+00000230: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000240: 6875 622e 636f 6d2f 7669 6374 3072 7363  hub.com/vict0rsc
+00000250: 682f 746f 7263 685f 7369 6d70 6c65 5f74  h/torch_simple_t
+00000260: 696d 696e 6722 2074 6172 6765 743d 225f  iming" target="_
+00000270: 626c 616e 6b22 3ef0 9f92 bb26 6e62 7370  blank">....&nbsp
+00000280: 3b26 6e62 7370 3b43 6f64 653c 2f61 3e3c  ;&nbsp;Code</a><
+00000290: 2f73 7472 6f6e 673e 0a3c 7374 726f 6e67  /strong>.<strong
+000002a0: 3e26 6e62 7370 3b26 6e62 7370 3be2 80a2  >&nbsp;&nbsp;...
+000002b0: 266e 6273 703b 266e 6273 703b 3c2f 7374  &nbsp;&nbsp;</st
+000002c0: 726f 6e67 3e0a 3c73 7472 6f6e 673e 3c61  rong>.<strong><a
+000002d0: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
+000002e0: 6f72 6368 2d73 696d 706c 652d 7469 6d69  orch-simple-timi
+000002f0: 6e67 2e72 6561 6474 6865 646f 6373 2e69  ng.readthedocs.i
+00000300: 6f2f 2220 7461 7267 6574 3d22 5f62 6c61  o/" target="_bla
+00000310: 6e6b 223e 446f 6373 266e 6273 703b 266e  nk">Docs&nbsp;&n
+00000320: 6273 703b f09f 9391 3c2f 613e 3c2f 7374  bsp;....</a></st
+00000330: 726f 6e67 3e0a 3c2f 703e 0a0a 3c70 2061  rong>.</p>..<p a
+00000340: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000350: 2020 203c 613e 0a09 2020 2020 3c69 6d67     <a>..    <img
+00000360: 2073 7263 3d27 6874 7470 733a 2f2f 696d   src='https://im
+00000370: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000380: 6765 2f70 7974 686f 6e2d 332e 3825 3242  ge/python-3.8%2B
+00000390: 2d62 6c75 6527 2061 6c74 3d27 5079 7468  -blue' alt='Pyth
+000003a0: 6f6e 2720 2f3e 0a09 3c2f 613e 0a09 3c61  on' />..</a>..<a
+000003b0: 2068 7265 663d 2768 7474 7073 3a2f 2f74   href='https://t
+000003c0: 6f72 6368 2d73 696d 706c 652d 7469 6d69  orch-simple-timi
+000003d0: 6e67 2e72 6561 6474 6865 646f 6373 2e69  ng.readthedocs.i
+000003e0: 6f2f 656e 2f6c 6174 6573 742f 3f62 6164  o/en/latest/?bad
+000003f0: 6765 3d6c 6174 6573 7427 3e0a 2020 2020  ge=latest'>.    
+00000400: 093c 696d 6720 7372 633d 2768 7474 7073  .<img src='https
+00000410: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
+00000420: 7267 2f70 726f 6a65 6374 732f 746f 7263  rg/projects/torc
+00000430: 682d 7369 6d70 6c65 2d74 696d 696e 672f  h-simple-timing/
+00000440: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000450: 6174 6573 7427 2061 6c74 3d27 446f 6375  atest' alt='Docu
+00000460: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000470: 2720 2f3e 0a09 3c2f 613e 0a20 2020 203c  ' />..</a>.    <
+00000480: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000490: 6769 7468 7562 2e63 6f6d 2f70 7366 2f62  github.com/psf/b
+000004a0: 6c61 636b 223e 0a09 2020 2020 3c69 6d67  lack">..    <img
+000004b0: 2073 7263 3d27 6874 7470 733a 2f2f 696d   src='https://im
+000004c0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000004d0: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+000004e0: 626c 6163 6b2d 626c 6163 6b27 202f 3e0a  black-black' />.
+000004f0: 093c 2f61 3e0a 2020 2020 3c61 2068 7265  .</a>.    <a hre
+00000500: 663d 2268 7474 7073 3a2f 2f70 7974 6f72  f="https://pytor
+00000510: 6368 2e6f 7267 223e 0a20 2020 2020 2020  ch.org">.       
+00000520: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000530: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000540: 6f2f 6261 6467 652f 5079 546f 7263 682d  o/badge/PyTorch-
+00000550: 2532 3345 4534 4332 432e 7376 673f 6c6f  %23EE4C2C.svg?lo
+00000560: 676f 3d50 7954 6f72 6368 266c 6f67 6f43  go=PyTorch&logoC
+00000570: 6f6c 6f72 3d77 6869 7465 222f 3e0a 2020  olor=white"/>.  
+00000580: 2020 3c2f 613e 0a20 2020 203c 6120 6872    </a>.    <a hr
+00000590: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000005a0: 2e6f 7267 2f70 726f 6a65 6374 2f74 6f72  .org/project/tor
+000005b0: 6368 2d73 696d 706c 652d 7469 6d69 6e67  ch-simple-timing
+000005c0: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
+000005d0: 2073 7263 3d22 6874 7470 733a 2f2f 6261   src="https://ba
+000005e0: 6467 652e 6675 7279 2e69 6f2f 7079 2f74  dge.fury.io/py/t
+000005f0: 6f72 6368 5f73 696d 706c 655f 7469 6d69  orch_simple_timi
+00000600: 6e67 2e73 7667 2220 616c 743d 2250 7950  ng.svg" alt="PyP
+00000610: 4920 7665 7273 696f 6e22 2068 6569 6768  I version" heigh
+00000620: 743d 2232 3022 3e0a 2020 2020 3c2f 613e  t="20">.    </a>
+00000630: 0a3c 2f70 3e0a 3c62 722f 3e0a 0a0a 2320  .</p>.<br/>...# 
+00000640: 546f 7263 6820 5369 6d70 6c65 2054 696d  Torch Simple Tim
+00000650: 696e 670a 0a41 2073 696d 706c 6520 7965  ing..A simple ye
+00000660: 7420 7665 7273 6174 696c 6520 7061 636b  t versatile pack
+00000670: 6167 6520 746f 2074 696d 6520 4350 552f  age to time CPU/
+00000680: 4750 552f 4d75 6c74 692d 4750 5520 6f70  GPU/Multi-GPU op
+00000690: 732e 0a0a 312e 2022 2a49 2077 616e 7420  s...1. "*I want 
+000006a0: 746f 2074 696d 6520 6f70 6572 6174 696f  to time operatio
+000006b0: 6e73 206f 6e63 652a 220a 2020 2031 2e20  ns once*".   1. 
+000006c0: 5468 6174 2773 2077 6861 7420 6120 6043  That's what a `C
+000006d0: 6c6f 636b 6020 6973 2066 6f72 0a32 2e20  lock` is for.2. 
+000006e0: 222a 4920 7761 6e74 2074 6f20 7469 6d65  "*I want to time
+000006f0: 2074 6865 2073 616d 6520 6f70 6572 6174   the same operat
+00000700: 696f 6e73 206d 756c 7469 706c 6520 7469  ions multiple ti
+00000710: 6d65 732a 220a 2020 2031 2e20 5468 6174  mes*".   1. That
+00000720: 2773 2077 6861 7420 6120 6054 696d 6572  's what a `Timer
+00000730: 6020 6973 2066 6f72 0a0a 496e 2073 696d  ` is for..In sim
+00000740: 706c 6520 7465 726d 733a 0a0a 2a20 4120  ple terms:..* A 
+00000750: 6043 6c6f 636b 6020 6973 2061 6e20 6f62  `Clock` is an ob
+00000760: 6a65 6374 2028 616e 6420 636f 6e74 6578  ject (and contex
+00000770: 742d 6d61 6e61 6765 7229 2074 6861 7420  t-manager) that 
+00000780: 7769 6c6c 2063 6f6d 7075 7465 2074 6865  will compute the
+00000790: 2065 6c6c 6170 7365 6420 7469 6d65 2062   ellapsed time b
+000007a0: 6574 7765 656e 2069 7473 2060 7374 6172  etween its `star
+000007b0: 7428 2960 2028 6f72 2060 5f5f 656e 7465  t()` (or `__ente
+000007c0: 725f 5f60 2920 616e 6420 6073 746f 7028  r__`) and `stop(
+000007d0: 2960 2028 6f72 2060 5f5f 6578 6974 5f5f  )` (or `__exit__
+000007e0: 6029 0a2a 2041 2060 5469 6d65 7260 2077  `).* A `Timer` w
+000007f0: 696c 6c20 696e 7465 726e 616c 6c79 206d  ill internally m
+00000800: 616e 6167 6520 636c 6f63 6b73 2073 6f20  anage clocks so 
+00000810: 7468 6174 2079 6f75 2063 616e 2066 6f63  that you can foc
+00000820: 7573 206f 6e20 7265 6164 6162 696c 6974  us on readabilit
+00000830: 7920 616e 6420 6e6f 7420 6461 7461 2073  y and not data s
+00000840: 7472 7563 7475 7265 730a 0a23 2320 496e  tructures..## In
+00000850: 7374 616c 6c61 7469 6f6e 0a0a 6060 600a  stallation..```.
+00000860: 7069 7020 696e 7374 616c 6c20 746f 7263  pip install torc
+00000870: 685f 7369 6d70 6c65 5f74 696d 696e 670a  h_simple_timing.
+00000880: 6060 600a 0a23 2320 486f 7720 746f 2075  ```..## How to u
+00000890: 7365 0a0a 2323 2320 4120 6043 6c6f 636b  se..### A `Clock
+000008a0: 600a 0a60 6060 7079 7468 6f6e 0a66 726f  `..```python.fro
+000008b0: 6d20 746f 7263 685f 7369 6d70 6c65 5f70  m torch_simple_p
+000008c0: 6172 7369 6e67 2069 6d70 6f72 7420 436c  arsing import Cl
+000008d0: 6f63 6b0a 696d 706f 7274 2074 6f72 6368  ock.import torch
+000008e0: 0a0a 7420 3d20 746f 7263 682e 7261 6e64  ..t = torch.rand
+000008f0: 2832 3030 302c 2032 3030 3029 0a67 7075  (2000, 2000).gpu
+00000900: 203d 2074 6f72 6368 2e63 7564 612e 6973   = torch.cuda.is
+00000910: 5f61 7661 696c 6162 6c65 2829 0a0a 7769  _available()..wi
+00000920: 7468 2043 6c6f 636b 2867 7075 3d67 7075  th Clock(gpu=gpu
+00000930: 2920 6173 2063 6f6e 7465 7874 5f63 6c6f  ) as context_clo
+00000940: 636b 3a0a 2020 2020 746f 7263 682e 696e  ck:.    torch.in
+00000950: 7665 7273 6528 7420 4020 742e 5429 0a0a  verse(t @ t.T)..
+00000960: 636c 6f63 6b20 3d20 436c 6f63 6b28 6770  clock = Clock(gp
+00000970: 753d 6770 7529 2e73 7461 7274 2829 0a74  u=gpu).start().t
+00000980: 6f72 6368 2e69 6e76 6572 7365 2874 2040  orch.inverse(t @
+00000990: 2074 2e54 290a 636c 6f63 6b2e 7374 6f70   t.T).clock.stop
+000009a0: 2829 0a0a 7072 696e 7428 636f 6e74 6578  ()..print(contex
+000009b0: 745f 636c 6f63 6b2e 6475 7261 7469 6f6e  t_clock.duration
+000009c0: 2920 2320 302e 3239 3638 3835 3031 3335  ) # 0.2968850135
+000009d0: 3830 3332 3232 370a 7072 696e 7428 636c  8032227.print(cl
+000009e0: 6f63 6b2e 6475 7261 7469 6f6e 2920 2020  ock.duration)   
+000009f0: 2020 2020 2020 2320 302e 3239 3238 3936        # 0.292896
+00000a00: 3033 3233 3333 3337 340a 6060 600a 0a4d  032333374.```..M
+00000a10: 6f72 6520 6578 616d 706c 6573 2c20 696e  ore examples, in
+00000a20: 636c 7564 696e 6720 626f 7574 2068 6f77  cluding bout how
+00000a30: 2074 6f20 6561 7369 6c79 2073 6861 7265   to easily share
+00000a40: 2064 6174 6120 7374 7275 6374 7572 6573   data structures
+00000a50: 2075 7369 6e67 2061 2060 7374 6f72 6560   using a `store`
+00000a60: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
+00000a70: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
+00000a80: 696f 6e5d 2868 7474 7073 3a2f 2f74 6f72  ion](https://tor
+00000a90: 6368 2d73 696d 706c 652d 7469 6d69 6e67  ch-simple-timing
+00000aa0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000ab0: 656e 2f6c 6174 6573 742f 6175 746f 6170  en/latest/autoap
+00000ac0: 692f 746f 7263 685f 7369 6d70 6c65 5f74  i/torch_simple_t
+00000ad0: 696d 696e 672f 636c 6f63 6b2f 696e 6465  iming/clock/inde
+00000ae0: 782e 6874 6d6c 292e 0a0a 2323 2320 4120  x.html)...### A 
+00000af0: 6054 696d 6572 600a 0a60 6060 7079 7468  `Timer`..```pyth
+00000b00: 6f6e 0a66 726f 6d20 746f 7263 685f 7369  on.from torch_si
+00000b10: 6d70 6c65 5f74 696d 696e 6720 696d 706f  mple_timing impo
+00000b20: 7274 2054 696d 6572 0a69 6d70 6f72 7420  rt Timer.import 
+00000b30: 746f 7263 680a 0a64 6576 6963 6520 3d20  torch..device = 
+00000b40: 746f 7263 682e 6465 7669 6365 2822 6375  torch.device("cu
+00000b50: 6461 2220 6966 2074 6f72 6368 2e63 7564  da" if torch.cud
+00000b60: 612e 6973 5f61 7661 696c 6162 6c65 2829  a.is_available()
+00000b70: 2065 6c73 6520 2263 7075 2229 0a0a 5820   else "cpu")..X 
+00000b80: 3d20 746f 7263 682e 7261 6e64 2835 3030  = torch.rand(500
+00000b90: 302c 2035 3030 302c 2064 6576 6963 653d  0, 5000, device=
+00000ba0: 6465 7669 6365 290a 5920 3d20 746f 7263  device).Y = torc
+00000bb0: 682e 7261 6e64 2835 3030 302c 2031 3030  h.rand(5000, 100
+00000bc0: 2c20 6465 7669 6365 3d64 6576 6963 6529  , device=device)
+00000bd0: 0a6d 6f64 656c 203d 2074 6f72 6368 2e6e  .model = torch.n
+00000be0: 6e2e 4c69 6e65 6172 2835 3030 302c 2031  n.Linear(5000, 1
+00000bf0: 3030 292e 746f 2864 6576 6963 6529 0a6f  00).to(device).o
+00000c00: 7074 696d 697a 6572 203d 2074 6f72 6368  ptimizer = torch
+00000c10: 2e6f 7074 696d 2e41 6461 6d28 6d6f 6465  .optim.Adam(mode
+00000c20: 6c2e 7061 7261 6d65 7465 7273 2829 290a  l.parameters()).
+00000c30: 0a67 7075 203d 2064 6576 6963 652e 7479  .gpu = device.ty
+00000c40: 7065 203d 3d20 2263 7564 6122 0a74 696d  pe == "cuda".tim
+00000c50: 6572 203d 2054 696d 6572 2867 7075 3d67  er = Timer(gpu=g
+00000c60: 7075 290a 0a66 6f72 2065 706f 6368 2069  pu)..for epoch i
+00000c70: 6e20 7261 6e67 6528 3130 293a 0a20 2020  n range(10):.   
+00000c80: 2074 696d 6572 2e63 6c6f 636b 2822 6570   timer.clock("ep
+00000c90: 6f63 6822 292e 7374 6172 7428 290a 2020  och").start().  
+00000ca0: 2020 666f 7220 6220 696e 2072 616e 6765    for b in range
+00000cb0: 2835 3029 3a0a 2020 2020 2020 2020 7820  (50):.        x 
+00000cc0: 3d20 585b 622a 3130 303a 2028 622b 3129  = X[b*100: (b+1)
+00000cd0: 2a31 3030 5d0a 2020 2020 2020 2020 7920  *100].        y 
+00000ce0: 3d20 595b 622a 3130 303a 2028 622b 3129  = Y[b*100: (b+1)
+00000cf0: 2a31 3030 5d0a 2020 2020 2020 2020 6f70  *100].        op
+00000d00: 7469 6d69 7a65 722e 7a65 726f 5f67 7261  timizer.zero_gra
+00000d10: 6428 290a 2020 2020 2020 2020 7769 7468  d().        with
+00000d20: 2074 696d 6572 2e63 6c6f 636b 2822 666f   timer.clock("fo
+00000d30: 7277 6172 6422 2c20 6967 6e6f 7265 3d65  rward", ignore=e
+00000d40: 706f 6368 3e30 293a 0a20 2020 2020 2020  poch>0):.       
+00000d50: 2020 2020 2070 203d 206d 6f64 656c 2878       p = model(x
+00000d60: 290a 2020 2020 2020 2020 6c6f 7373 203d  ).        loss =
+00000d70: 2074 6f72 6368 2e6e 6e2e 6675 6e63 7469   torch.nn.functi
+00000d80: 6f6e 616c 2e63 726f 7373 5f65 6e74 726f  onal.cross_entro
+00000d90: 7079 2870 2c20 7929 0a20 2020 2020 2020  py(p, y).       
+00000da0: 2077 6974 6820 7469 6d65 722e 636c 6f63   with timer.cloc
+00000db0: 6b28 2262 6163 6b77 6172 6422 2c20 6967  k("backward", ig
+00000dc0: 6e6f 7265 3d65 706f 6368 3e30 293a 0a20  nore=epoch>0):. 
+00000dd0: 2020 2020 2020 2020 2020 206c 6f73 732e             loss.
+00000de0: 6261 636b 7761 7264 2829 0a20 2020 2020  backward().     
+00000df0: 2020 206f 7074 696d 697a 6572 2e73 7465     optimizer.ste
+00000e00: 7028 290a 2020 2020 7469 6d65 722e 636c  p().    timer.cl
+00000e10: 6f63 6b28 2265 706f 6368 2229 2e73 746f  ock("epoch").sto
+00000e20: 7028 290a 0a73 7461 7473 203d 2074 696d  p()..stats = tim
+00000e30: 6572 2e73 7461 7473 2829 0a23 2075 7365  er.stats().# use
+00000e40: 2073 7461 7473 2066 6f72 2064 6973 706c   stats for displ
+00000e50: 6179 2061 6e64 2f6f 7220 6c6f 6767 696e  ay and/or loggin
+00000e60: 670a 2320 7761 6e64 622e 7375 6d6d 6172  g.# wandb.summar
+00000e70: 792e 7570 6461 7465 2873 7461 7473 290a  y.update(stats).
+00000e80: 7072 696e 7428 7469 6d65 722e 6469 7370  print(timer.disp
+00000e90: 6c61 7928 7374 6174 733d 7374 6174 732c  lay(stats=stats,
+00000ea0: 2070 7265 6369 7369 6f6e 3d35 2929 0a60   precision=5)).`
+00000eb0: 6060 0a0a 6060 600a 6570 6f63 6820 2020  ``..```.epoch   
+00000ec0: 203a 2030 2e32 3530 3634 20c2 b120 302e   : 0.25064 .. 0.
+00000ed0: 3032 3732 3820 286e 3d31 3029 0a66 6f72  02728 (n=10).for
+00000ee0: 7761 7264 2020 3a20 302e 3030 3232 3620  ward  : 0.00226 
+00000ef0: c2b1 2030 2e30 3035 3236 2028 6e3d 3530  .. 0.00526 (n=50
+00000f00: 290a 6261 636b 7761 7264 203a 2030 2e30  ).backward : 0.0
+00000f10: 3032 3039 20c2 b120 302e 3030 3338 3720  0209 .. 0.00387 
+00000f20: 286e 3d35 3029 0a60 6060 0a0a 2323 2320  (n=50).```..### 
+00000f30: 4120 6465 636f 7261 746f 720a 0a59 6f75  A decorator..You
+00000f40: 2063 616e 2061 6c73 6f20 7573 6520 6120   can also use a 
+00000f50: 6465 636f 7261 746f 7220 746f 2074 696d  decorator to tim
+00000f60: 6520 6675 6e63 7469 6f6e 7320 7769 7468  e functions with
+00000f70: 6f75 7420 6d75 6368 206f 7665 7268 6561  out much overhea
+00000f80: 6420 696e 2079 6f75 7220 636f 6465 3a0a  d in your code:.
+00000f90: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00000fa0: 746f 7263 685f 7369 6d70 6c65 5f74 696d  torch_simple_tim
+00000fb0: 696e 6720 696d 706f 7274 2074 696d 6569  ing import timei
+00000fc0: 742c 2067 6574 5f67 6c6f 6261 6c5f 7469  t, get_global_ti
+00000fd0: 6d65 722c 2072 6573 6574 5f67 6c6f 6261  mer, reset_globa
+00000fe0: 6c5f 7469 6d65 720a 696d 706f 7274 2074  l_timer.import t
+00000ff0: 6f72 6368 0a0a 2320 5573 6520 7468 6520  orch..# Use the 
+00001000: 6675 6e63 7469 6f6e 206e 616d 6520 6173  function name as
+00001010: 2074 6865 2074 696d 6572 206e 616d 650a   the timer name.
+00001020: 4074 696d 6569 7428 6770 753d 5472 7565  @timeit(gpu=True
+00001030: 290a 6465 6620 7472 6169 6e28 293a 0a20  ).def train():. 
+00001040: 2020 2078 203d 2074 6f72 6368 2e72 616e     x = torch.ran
+00001050: 6428 3130 3030 2c20 3130 3030 2c20 6465  d(1000, 1000, de
+00001060: 7669 6365 3d22 6375 6461 2220 6966 2074  vice="cuda" if t
+00001070: 6f72 6368 2e63 7564 612e 6973 5f61 7661  orch.cuda.is_ava
+00001080: 696c 6162 6c65 2829 2065 6c73 6520 2263  ilable() else "c
+00001090: 7075 2229 0a20 2020 2072 6574 7572 6e20  pu").    return 
+000010a0: 746f 7263 682e 696e 7665 7273 6528 7820  torch.inverse(x 
+000010b0: 4020 7829 0a0a 2320 5573 6520 6120 6375  @ x)..# Use a cu
+000010c0: 7374 6f6d 206e 616d 650a 4074 696d 6569  stom name.@timei
+000010d0: 7428 2274 6573 7422 290a 6465 6620 7465  t("test").def te
+000010e0: 7374 5f63 7075 2829 3a0a 2020 2020 7265  st_cpu():.    re
+000010f0: 7475 726e 2074 6f72 6368 2e69 6e76 6572  turn torch.inver
+00001100: 7365 2874 6f72 6368 2e72 616e 6428 3130  se(torch.rand(10
+00001110: 3030 2c20 3130 3030 2920 4020 746f 7263  00, 1000) @ torc
+00001120: 682e 7261 6e64 2831 3030 302c 2031 3030  h.rand(1000, 100
+00001130: 3029 290a 0a69 6620 5f5f 6e61 6d65 5f5f  0))..if __name__
+00001140: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
+00001150: 2020 2020 666f 7220 5f20 696e 2072 616e      for _ in ran
+00001160: 6765 2828 6570 6f63 6873 203a 3d20 3130  ge((epochs := 10
+00001170: 2929 3a0a 2020 2020 2020 2020 7472 6169  )):.        trai
+00001180: 6e28 290a 0a20 2020 2074 6573 745f 6370  n()..    test_cp
+00001190: 7528 290a 0a20 2020 2074 696d 6572 203d  u()..    timer =
+000011a0: 2067 6574 5f67 6c6f 6261 6c5f 7469 6d65   get_global_time
+000011b0: 7228 290a 2020 2020 7072 696e 7428 7469  r().    print(ti
+000011c0: 6d65 722e 6469 7370 6c61 7928 2929 0a0a  mer.display())..
+000011d0: 2020 2020 7265 7365 745f 676c 6f62 616c      reset_global
+000011e0: 5f74 696d 6572 2829 0a60 6060 0a0a 5072  _timer().```..Pr
+000011f0: 696e 7473 3a0a 0a60 6060 7465 7874 0a74  ints:..```text.t
+00001200: 7261 696e 203a 2030 2e30 3435 20c2 b120  rain : 0.045 .. 
+00001210: 302e 3030 3720 286e 3d31 3029 0a74 6573  0.007 (n=10).tes
+00001220: 7420 203a 2030 2e30 3436 2020 2020 2020  t  : 0.046      
+00001230: 2020 2028 6e3d 2031 290a 6060 600a 0a42     (n= 1).```..B
+00001240: 7920 6465 6661 756c 7420 7468 6520 6040  y default the `@
+00001250: 7469 6d65 6974 6020 6465 636f 6472 6174  timeit` decodrat
+00001260: 6f72 2074 616b 6573 2061 7420 6c65 6173  or takes at leas
+00001270: 7420 6120 606e 616d 6560 2c20 7769 6c6c  t a `name`, will
+00001280: 2075 7365 2060 6770 753d 4661 6c73 6560   use `gpu=False`
+00001290: 2061 6e64 2075 7365 2074 6865 2067 6c6f   and use the glo
+000012a0: 6261 6c20 7469 6d65 7220 2860 746f 7263  bal timer (`torc
+000012b0: 685f 7369 6d70 6c65 5f74 696d 696e 672e  h_simple_timing.
+000012c0: 5449 4d45 5260 292e 2059 6f75 2063 616e  TIMER`). You can
+000012d0: 2070 6173 7320 796f 7572 206f 776e 2074   pass your own t
+000012e0: 696d 6572 2077 6974 6820 6040 7469 6d65  imer with `@time
+000012f0: 6974 286e 616d 652c 2074 696d 6572 3d74  it(name, timer=t
+00001300: 696d 6572 2960 2e0a 0a53 6565 205b 696e  imer)`...See [in
+00001310: 2074 6865 2064 6f63 735d 285b 6874 7470   the docs]([http
+00001320: 733a 2f2f 5d28 6874 7470 733a 2f2f 746f  s://](https://to
+00001330: 7263 682d 7369 6d70 6c65 2d74 696d 696e  rch-simple-timin
+00001340: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
+00001350: 2f65 6e2f 6c61 7465 7374 2f61 7574 6f61  /en/latest/autoa
+00001360: 7069 2f74 6f72 6368 5f73 696d 706c 655f  pi/torch_simple_
+00001370: 7469 6d69 6e67 2f69 6e64 6578 2e68 746d  timing/index.htm
+00001380: 6c29 292e 0a0a                           l))...
```

