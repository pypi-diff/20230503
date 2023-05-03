# Comparing `tmp/synapgrad-0.3.0-py3-none-any.whl.zip` & `tmp/synapgrad-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 29510 bytes, number of entries: 21
+Zip file size: 29772 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
--rw-rw-rw-  2.0 fat    30938 b- defN 23-May-01 14:04 synapgrad/engine.py
+-rw-rw-rw-  2.0 fat    32179 b- defN 23-May-03 18:05 synapgrad/engine.py
 -rw-rw-rw-  2.0 fat      442 b- defN 23-May-01 13:33 synapgrad/nn/__init__.py
 -rw-rw-rw-  2.0 fat     3538 b- defN 23-Apr-20 01:42 synapgrad/nn/activations.py
 -rw-rw-rw-  2.0 fat     7831 b- defN 23-Apr-19 17:14 synapgrad/nn/functional.py
 -rw-rw-rw-  2.0 fat     2879 b- defN 23-Apr-20 12:52 synapgrad/nn/initializations.py
--rw-rw-rw-  2.0 fat    17780 b- defN 23-May-01 13:30 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat    18237 b- defN 23-May-03 18:16 synapgrad/nn/layers.py
 -rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-20 01:41 synapgrad/nn/losses.py
 -rw-rw-rw-  2.0 fat     2654 b- defN 23-Apr-19 20:19 synapgrad/nn/modules.py
 -rw-rw-rw-  2.0 fat      989 b- defN 23-May-01 11:50 synapgrad/nn/neurons.py
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
 -rw-rw-rw-  2.0 fat     5293 b- defN 23-Apr-20 01:43 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
 -rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-21 08:50 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4664 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1696 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/RECORD
-21 files, 102309 bytes uncompressed, 26770 bytes compressed:  73.8%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4756 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1696 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/RECORD
+21 files, 104099 bytes uncompressed, 27032 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.3.0.dist-info/LICENSE
+Filename: synapgrad-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.3.0.dist-info/METADATA
+Filename: synapgrad-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.3.0.dist-info/WHEEL
+Filename: synapgrad-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.3.0.dist-info/top_level.txt
+Filename: synapgrad-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.3.0.dist-info/RECORD
+Filename: synapgrad-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/engine.py

```diff
@@ -278,26 +278,48 @@
                 tensor._grad += grad
 
         out._backward = _backward
         
         return out
     
     
+    @staticmethod
+    def ones(shape, dtype=None, requires_grad=False, name=None):
+        return Tensor(np.ones(shape), dtype=dtype, requires_grad=requires_grad, name=name)
+    
+    
+    @staticmethod
+    def zeros(shape, dtype=None, requires_grad=False, name=None):
+        return Tensor(np.zeros(shape), dtype=dtype, requires_grad=requires_grad, name=name)
+    
+    
     def add(self, t2:'Tensor') -> 'Tensor':
         return self + t2
     
     
     def mul(self, t2:'Tensor') -> 'Tensor':
         return self * t2
     
     
     def matmul(self, t2:'Tensor') -> 'Tensor':
         return self @ t2
     
     
+    def reshape(self, shape:tuple) -> 'Tensor':
+        out = Tensor(self.data.reshape(shape), (self,), '<Reshape>', requires_grad=self.requires_grad)
+        
+        def _backward():
+            if self.requires_grad:
+                self._grad += out._grad.reshape(self.shape)
+            
+        out._backward = _backward
+        
+        return out
+    
+    
     def view(self, *shape:tuple) -> 'Tensor':
         out = Tensor(self.data.reshape(shape), (self,), '<View>', requires_grad=self.requires_grad)
         
         def _backward():
             if self.requires_grad:
                 self._grad += out._grad.reshape(self.shape)
             
@@ -500,15 +522,20 @@
     
     
     def sum(self, dim:int=None, keepdims=False) -> 'Tensor':
         out = Tensor(self.data.sum(axis=dim, keepdims=keepdims), (self,), '<Sum>', requires_grad=self.requires_grad)
         
         def _backward():
             if self.requires_grad:
-                self._grad += out._grad
+                out_grad = out._grad
+                if not keepdims and dim is not None:
+                    s = list(self.shape)
+                    for d in dim: s[d] = 1
+                    out_grad = out._grad.reshape(s) 
+                self._grad += np.ones(self.shape) * out_grad
             
         out._backward = _backward
         
         return out
     
     
     def mean(self, dim:int=None, keepdims=False) -> 'Tensor':
@@ -519,15 +546,20 @@
                 if dim is None:
                     size = self.data.size
                 elif isinstance(dim, int):
                     size = self.data.shape[dim]
                 elif isinstance(dim, tuple):
                     size = 1
                     for d in dim: size *= self.data.shape[d]
-                self._grad += (np.ones(self.shape) / size) * out._grad
+                out_grad = out._grad
+                if not keepdims and dim is not None:
+                    s = list(self.shape)
+                    for d in dim: s[d] = 1
+                    out_grad = out._grad.reshape(s) 
+                self._grad += (np.ones(self.shape) / size) * out_grad
             
         out._backward = _backward
         
         return out
 
     
     def max(self, dim:int=None, keepdims=False, return_indices=None, return_selected=False) -> tuple['Tensor',...]:
```

## synapgrad/nn/layers.py

```diff
@@ -11,21 +11,21 @@
         super().__init__()
         self.input_size = input_size
         self.output_size = output_size
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((output_size, input_size), weight_init_method).astype(np.float32)
         self.weight = Tensor(weight_values, requires_grad=True)
-        self.bias = Tensor(np.zeros((output_size,), dtype=np.float32), requires_grad=True)
+        self.bias = Tensor.zeros((output_size,), dtype=np.float32, requires_grad=True)
         
     def forward(self, x:Tensor) -> Tensor:
         assert x.shape[1] == self.input_size, f"Expected input size '{self.input_size}' but received '{x.shape[1]}'"
 
-        out = (x @ self.weight.transpose(0,-1)) + self.bias
-        
+        out = (x @ self.weight.transpose(0,1)) + self.bias
+
         return out
     
     def parameters(self) -> list[Tensor]:
         return [self.weight, self.bias]
     
     def __repr__(self) -> str:
         return f"Linear(input_size={self.input_size}, neurons={len(self.output_size)})"
@@ -220,29 +220,29 @@
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((out_channels, in_channels, *kernel_size), weight_init_method).astype(np.float32)
         self.weight = Tensor(weight_values, requires_grad=True)
-        self.bias = Tensor(np.zeros((out_channels,), dtype=np.float32), requires_grad=True)
+        self.bias = Tensor.zeros((out_channels,), dtype=np.float32, requires_grad=True)
     
     def forward(self, x: Tensor) -> Tensor:
         N, C, H, W = x.shape
         lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
         lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
         
         unfolded = Unfold(kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
                            padding=self.padding, pad_value=0)(x)
         
         weight = self.weight.view(self.weight.shape[0], -1).transpose(0,1) 
         mult = unfolded.transpose(1,2) @ weight
         convolved = (mult) + self.bias
         out = convolved.transpose(1,2).view(N, self.out_channels, lH, lW)
-
+                
         return out
         
     def parameters(self) -> list['Tensor']:
         return [self.weight, self.bias]
     
     def __repr__(self) -> str:
         return (f"Conv2d(in_channels={self.in_channels}, out_channels={self.out_channels}, " + 
@@ -290,25 +290,25 @@
             raise ValueError(f"'{mode}' is not a valid mode, expected one of {valid_modes}")
         self.mode = mode
         
         if dtype is None:
             dtype = np.float32
         
         if self.track_running_stats:
-            self.running_mean = Tensor(np.zeros(num_features, dtype=dtype))
-            self.running_var = Tensor(np.ones(num_features, dtype=dtype))
+            self.running_mean = Tensor.zeros(num_features, dtype=dtype, name='running_mean')
+            self.running_var = Tensor.ones(num_features, dtype=dtype, name='running_var')
         else:
             self.running_mean = None
             self.running_var = None
         
         if affine:
             # gamma
-            self.weight = Tensor(np.ones(num_features), requires_grad=True, dtype=dtype, name="gamma")
+            self.weight = Tensor.ones(num_features, requires_grad=True, dtype=dtype, name="gamma")
             # beta
-            self.bias = Tensor(np.zeros(num_features), requires_grad=True, dtype=dtype, name="beta")
+            self.bias = Tensor.zeros(num_features, requires_grad=True, dtype=dtype, name="beta")
                 
     def forward(self, x: Tensor) -> Tensor:
         if self.mode == '2d':
             if len(x.shape) == 4:
                 N, C, H, W = x.shape
                 n = N*H*W # num_samples
                 dims = (0,2,3)
@@ -326,42 +326,54 @@
                 dims = (0,)
                 view_shape = (1,C)
             else: raise RuntimeError(f"Expected 2D or 3D tensor, but got {len(x.shape)}D")
         assert C == self.num_features, f"Expected {self.num_features} channels, got {C}."
         
         if self.training or not self.track_running_stats:
             # Compute the mean of each channel
-            mu = x.mean(dim=dims, keepdims=True)
+            mu = x.mean(dim=dims)
             # Compute the variance of each channel
-            var_sum = ((x-mu)**2).sum(dim=dims, keepdims=True)
+            var_sum = ((x-mu.reshape(view_shape))**2).sum(dim=dims)
             var = var_sum / n
-            std = (var + self.eps).sqrt()
-            
-            # Normalize the input tensor
-            x_norm = (x - mu) / std
             
+            x_norm = self.__normalize(x, mu, var)
+
             # Update the running average of mean and variance
             if self.training and self.track_running_stats:
-                r_mu = (self.momentum * mu.data.reshape(-1) + (1 - self.momentum) * self.running_mean.data)
+                r_mu = (self.momentum * mu.data + (1 - self.momentum) * self.running_mean.data)
                 self.running_mean = Tensor(r_mu)
                 
-                unbiased_var = var_sum.data.reshape(-1) / (n - 1)
+                unbiased_var = var_sum.data / (n - 1)
                 r_var = (self.momentum * unbiased_var + (1 - self.momentum) * self.running_var.data)
-                self.running_var = Tensor(r_var.squeeze())
+                self.running_var = Tensor(r_var)
         else:
-            x_norm = (x - self.running_mean.view(*view_shape)) / (self.running_var.view(*view_shape) + self.eps).sqrt()
+            x_norm = self.__normalize(x, self.running_mean, self.running_var)
 
         # Scale and shift the normalization
         if self.affine:
-            out = self.weight.view(*view_shape) * x_norm + self.bias.view(*view_shape)
+            out = (x_norm * self.weight.reshape(view_shape)) + self.bias.reshape(view_shape)
         else:
             out = x_norm
         
         return out
+    
+    def __normalize(self, x:Tensor, mean:Tensor, var:Tensor, channel_dim=1) -> Tensor:
+        """Normalize a Tensor with mean and variance over the channel dimension
 
+            Args:
+                x (Tensor): Input
+                mean (Tensor): Computed batch mean
+                var (Tensor): Computed batch var
+            
+            Returns:
+                Tensor: Normalized tensor
+        """
+        shape = [1,]*len(x.shape); shape[channel_dim] = x.shape[channel_dim]
+        return (x - mean.reshape(shape)) / ((var + self.eps).reshape(shape).sqrt())
+        
     def parameters(self) -> list[Tensor]:
         return [self.weight, self.bias] if self.affine else []
 
 
 class BatchNorm1d(BatchNorm):
     """
     Reference:
```

## Comparing `synapgrad-0.3.0.dist-info/LICENSE` & `synapgrad-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synapgrad-0.3.0.dist-info/METADATA` & `synapgrad-0.3.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapgrad
-Version: 0.3.0
+Version: 0.3.1
 Summary: An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 Home-page: https://github.com/pgmesa/synapgrad
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -77,25 +77,25 @@
 - [x] 3. CNN for handwritten digits classification (MNIST dataset)
 
 Example 1 (synapgrad MLP solution)     |  Example 2 and 3
 :-------------------------:|:-------------------------:
 ![Image 1](/assets/example_moons.png) | ![Image 2](/assets/example_mnist.png) 
 
 ## Comparisons with other frameworks
-In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd).
+In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd). All trainings have been runned on a laptop with an Intel Core i7 10th generation processor.
 
 | Training Example | synapgrad | torch | micrograd |
 |     :---:        |  :---:  |  :---:  |   :---:   |  
 | 1 | 1.7 s | 1.5 s | 1 min 43 s |
-| 2 | 2 min 30 s | 53 s | - |
+| 2 | 2 min 8 s | 53 s | - |
 | 3 |  25 min 10 s  |  2 min 5 s  | - |
 | 2 (without batchnorm) | 52 s |  31 s | - |
 | 3 (without batchnorm) |  16 min 7 s  |  1 min 52 s  | - |
 
-As can be observed, conv2d and batchnorm are currently much more optimized in Pytorch. I will attempt to optimize these layers in a future version.
+As can be observed, conv2d and batchnorm are currently much better optimized in Pytorch. I may attempt to optimize these layers in a future version.
 
 ## Graph Visualization
 In the `examples/trace_graph.ipynb` notebook there is an example of how to display the graph that synapgrad creates in the background as operations are chained.
 
 ```python
 import synapgrad
 from synapgrad import nn, utils
```

## Comparing `synapgrad-0.3.0.dist-info/RECORD` & `synapgrad-0.3.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 synapgrad/__init__.py,sha256=rzU1koPmJ4_LyMdxWzho4Qd-qWUqh16aKSgmF5HBOEw,72
-synapgrad/engine.py,sha256=fttCUYh5ZLB5uJ6MzvCp63aPQpW_P7OeZKtrXVL_664,30938
+synapgrad/engine.py,sha256=nMvbz8hdQ49SzrJe5qX98p-YYa2SnE1jj5Jj3Nr7ELg,32179
 synapgrad/nn/__init__.py,sha256=kJVBFgfaX-9Rsg0QDV3lKjPaRNuWVn2RgCkb-mAvXhM,442
 synapgrad/nn/activations.py,sha256=TEUzX6IvnYlnWkmCyLQMxTDENH-cukG8R0R26ikV5QA,3538
 synapgrad/nn/functional.py,sha256=jICas3UKdjRsxh4xZBTl4nNMfswrrEmqRoOKzu4Qgjw,7831
 synapgrad/nn/initializations.py,sha256=WjgU7KfSQh_aMXBXrj5KOyaz6C3y-tPbmsodFiu6uRc,2879
-synapgrad/nn/layers.py,sha256=OOSg5Dcz3O3RHFGztODfv6aXjWOXUcMW9JWL8jCycZU,17780
+synapgrad/nn/layers.py,sha256=MI9erbQ1UQB2D-SlXd3ceiMoIaD7bLFPm8woahUq5SU,18237
 synapgrad/nn/losses.py,sha256=N7uLz_ILdv_LQ_MGLH3xCfyC9FPyEWz7zVO51Di0XJY,6809
 synapgrad/nn/modules.py,sha256=y_F6iUE5t0rlXGwvOtsSVttqgJ3OPMkdx5MbDxceVYc,2654
 synapgrad/nn/neurons.py,sha256=oQNtsfpAE-CYymK45Wz-ORsuiOzk6CAg5ZcCLYnjl6A,989
 synapgrad/optim/__init__.py,sha256=8X56jD7Dcyw-Hdux1K7_YK9_oc3BuNPk9YwC7gSNWaE,46
 synapgrad/optim/optimizers.py,sha256=Y5ryseve_Virrpsl2ynSt2npq2O0-kyIj_Tj0jfKko0,5293
 synapgrad/utils/__init__.py,sha256=eCwZrBr9yWO92hufOIWwAFhwrA_JuMCsmHeDL7PSAtE,154
 synapgrad/utils/data.py,sha256=cwSsVZwEbB6BU9tWrf5aIeZo9u5KNgar7rVYa6WV328,3403
 synapgrad/utils/graph.py,sha256=FOkPCSYcmOaoPRhdoXweUQRvoxH0n3x4nASGLr7HQjw,1345
 synapgrad/utils/train.py,sha256=V3j4iqSW9sjSfIz9bski95Ni25KuYzIAkjqD4o3-Tjg,10586
-synapgrad-0.3.0.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
-synapgrad-0.3.0.dist-info/METADATA,sha256=xo0yor_rizRPwrTbqEkbeyd291m40qqxZNIpQOKzoNw,4664
-synapgrad-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-synapgrad-0.3.0.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
-synapgrad-0.3.0.dist-info/RECORD,,
+synapgrad-0.3.1.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
+synapgrad-0.3.1.dist-info/METADATA,sha256=3bXzYfFAagKRkV_Hk_dEAwjDqg0k3Z7A5uan4NvI5M0,4756
+synapgrad-0.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+synapgrad-0.3.1.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
+synapgrad-0.3.1.dist-info/RECORD,,
```

