# Comparing `tmp/dufuz-0.0.1-py3-none-any.whl.zip` & `tmp/dufuz-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,20 @@
-Zip file size: 7478 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      106 b- defN 23-May-02 11:51 dufuz/__init__.py
+Zip file size: 11676 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat      106 b- defN 23-May-03 15:34 dufuz/__init__.py
+-rw-rw-rw-  2.0 fat      489 b- defN 23-May-03 15:41 dufuz/__main__.py
 -rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-28 07:27 dufuz/defuzzify.py
--rw-rw-rw-  2.0 fat     1917 b- defN 23-May-02 11:58 dufuz/dfn.py
+-rw-rw-rw-  2.0 fat     2298 b- defN 23-May-03 08:40 dufuz/dfn.py
 -rw-rw-rw-  2.0 fat      653 b- defN 23-Apr-29 09:10 dufuz/monitor.py
 -rw-rw-rw-  2.0 fat      339 b- defN 23-Apr-28 07:11 dufuz/tnorm.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-May-02 11:51 dufuz/core/__init__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-May-02 11:51 dufuz/core/domain.py
--rw-rw-rw-  2.0 fat     6298 b- defN 23-May-02 11:51 dufuz/core/environment.py
--rw-rw-rw-  2.0 fat     3545 b- defN 23-Apr-30 11:13 dufuz/core/number.py
--rw-rw-rw-  2.0 fat     2059 b- defN 23-May-02 12:07 dufuz-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 12:07 dufuz-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-02 12:07 dufuz-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      961 b- defN 23-May-02 12:07 dufuz-0.0.1.dist-info/RECORD
-13 files, 17869 bytes uncompressed, 5900 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat     1150 b- defN 23-May-02 12:15 dufuz/core/domain.py
+-rw-rw-rw-  2.0 fat     7073 b- defN 23-May-03 08:09 dufuz/core/environment.py
+-rw-rw-rw-  2.0 fat     3545 b- defN 23-May-03 00:48 dufuz/core/number.py
+-rw-rw-rw-  2.0 fat       49 b- defN 23-May-02 21:48 dufuz/interpreter/__init__.py
+-rw-rw-rw-  2.0 fat     9475 b- defN 23-May-03 15:15 dufuz/interpreter/interpret.py
+-rw-rw-rw-  2.0 fat     1000 b- defN 23-May-03 14:43 dufuz/interpreter/lexer.py
+-rw-rw-rw-  2.0 fat     4038 b- defN 23-May-03 14:49 dufuz/interpreter/parser.py
+-rw-rw-rw-  2.0 fat      880 b- defN 23-May-03 16:14 dufuz-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 16:14 dufuz-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 16:14 dufuz-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1371 b- defN 23-May-03 16:14 dufuz-0.1.0.dist-info/RECORD
+18 files, 33372 bytes uncompressed, 9460 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: dufuz/__init__.py
 Comment: 
 
+Filename: dufuz/__main__.py
+Comment: 
+
 Filename: dufuz/defuzzify.py
 Comment: 
 
 Filename: dufuz/dfn.py
 Comment: 
 
 Filename: dufuz/monitor.py
@@ -21,20 +24,32 @@
 
 Filename: dufuz/core/environment.py
 Comment: 
 
 Filename: dufuz/core/number.py
 Comment: 
 
-Filename: dufuz-0.0.1.dist-info/METADATA
+Filename: dufuz/interpreter/__init__.py
+Comment: 
+
+Filename: dufuz/interpreter/interpret.py
+Comment: 
+
+Filename: dufuz/interpreter/lexer.py
+Comment: 
+
+Filename: dufuz/interpreter/parser.py
+Comment: 
+
+Filename: dufuz-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: dufuz-0.0.1.dist-info/WHEEL
+Filename: dufuz-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: dufuz-0.0.1.dist-info/top_level.txt
+Filename: dufuz-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dufuz-0.0.1.dist-info/RECORD
+Filename: dufuz-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dufuz/dfn.py

```diff
@@ -1,8 +1,8 @@
-from dufuz.core import Environment, Domain
+from dufuz.core import Environment, Domain, Number
 from dufuz.tnorm import lukasiewicz
 import torch
 
 
 class DiscreteEnvironment(Environment):
     def __init__(self,
                  device='cuda',
@@ -15,33 +15,42 @@
         super().__init__(device=device, tnorm=tnorm)
         self.tol = tol
         self.breadth = breadth
         self.lower = lower
         self.upper = upper
         self.strategy = strategy
 
-    def number(self, value, form=lambda x: abs(x)):
+    def number(self, value, form=None, breadth=None):
+        if breadth is None:
+            breadth = self.breadth
+        if isinstance(value, dict):
+            assert form is None
+            return Number(list(value.values()), Domain(list(value.keys()), self))
+        if form is None:
+            form = lambda x: abs(x)
         if isinstance(value, list):
             return [self.number(element, form) for element in value]
         # TODO: implement the following with torch
         ret = {value: 1}
         offset = 0
         prob = 1
-        while offset+self.tol < self.breadth:
+        while offset+self.tol < breadth:
             offset += self.tol
-            prob -= self.tol/self.breadth
+            prob -= self.tol/breadth
             ret[value+offset] = form(prob)
             ret[value-offset] = form(prob)
-        return Domain(list(ret.keys()), self).set(ret)
+        return Number(list(ret.values()), Domain(list(ret.keys()), self))
 
     def discretize(self, values, numbers):
+        if numbers.dtype == torch.bool:
+            return values, numbers
         values, numbers = super().discretize(values, numbers)
         numbers = numbers if hasattr(numbers, "numpy") else torch.tensor(numbers, device=self.device)
         if self.lower and self.upper and self.strategy == "modulo":
             # makes the number filed a closed finite set
             numbers = torch.where(numbers < self.upper, numbers, numbers+(-self.upper+self.lower))
             numbers = torch.where(numbers > self.lower, numbers, numbers+(-self.lower+self.upper))
         elif (self.lower or self.upper) and self.strategy == "clip":
             numbers = torch.clip(numbers, self.lower, self.upper)
 
-        rounded_numbers = torch.round(numbers/self.tol)*self.tol
+        rounded_numbers = torch.floor(numbers/self.tol+0.5)*self.tol
         return values, rounded_numbers
```

## dufuz/core/domain.py

```diff
@@ -1,10 +1,9 @@
 import torch
 from dufuz.core.number import Number
-import numpy as np
 
 
 class Domain:
     def __init__(self, elements, env):
         self._elements = elements
         self._pos = None
         self.elements = elements if hasattr(elements, "numpy") else torch.tensor(elements, device=env.device)
@@ -19,12 +18,13 @@
             self._pos = {k: i for i, k in enumerate(elements.cpu().numpy() if hasattr(elements, "numpy") else elements)}
         return self._pos
 
     def size(self):
         return self.elements.size()
 
     def set(self, values):
-        # this is the equilvanet non-tf implementation
+        raise Exception("Domain.set should not be called. Use Environment.number() with a dictionary instead.")
+        import numpy as np
         spread = np.zeros(shape=self.elements.shape)
         for k, v in values.items():
             spread[self.pos[k]] = v
         return Number(torch.tensor(spread, device=self.env.device), self)
```

## dufuz/core/environment.py

```diff
@@ -45,18 +45,19 @@
         # squeeze
         values = torch.reshape(retvals, shape=[-1])
         elements = torch.reshape(elements, shape=[-1])
         # postprocess
         values, elements = self.discretize(values, elements)
         values, elements = self.reduce(values, elements)
         # find non-zero positions and gather respective values (memberships) and elements (method outputs)
-        positions = (values != 0)# > 1.E-12)
-        if positions.size() != values.size():
-            values = torch.masked_select(values, positions)
-            elements = torch.masked_select(elements, positions)
+        if elements.dtype != torch.bool:
+            positions = (values != 0)# > 1.E-12)
+            if positions.size() != values.size():
+                values = torch.masked_select(values, positions)
+                elements = torch.masked_select(elements, positions)
         for monitor in self.monitors:
             monitor.notify(elements.nelement(), None)
         return Number(values, Domain(elements, self))
 
     def reduce(self, values, elements):
         #values = torch.reshape(values, shape=[-1])
         #elements = torch.reshape(elements, shape=[-1])
@@ -103,40 +104,58 @@
     def eq(self, a, b):
         return self.apply(operator.eq, a, b)#self.And(self.apply(operator.ge, a, b), self.apply(operator.le, a, b))
 
     def complement(self, a):
         return Number(1-a.values, a.domain)
 
     def Not(self, a):
-        return 1-a #Number(a.values, Domain(1-a.domain.elements, a.domain.env))
+        return self.apply(torch.logical_not, a)#Number(1-a.values, a.domain)
 
     def And(self, a, b):
         return self.apply(operator.mul, a, b)
 
     def Or(self, a, b):
-        return self.apply(lambda x, y: x + y - x * y, a, b)
+        return self.combine(a, b)#self.apply(lambda x, y: x + y - x * y, a, b)
 
     def combine(self, number1, number2):
         if number1 is None:
             return number2
         if number2 is None:
             return number1
         values = torch.concat([number1.values, number2.values])
         elements = torch.concat([number1.domain.elements, number2.domain.elements])
         values, elements = self.reduce(values, elements)
         return Number(values, Domain(elements, self))
 
+    def setlist(self, values, item, value):
+        if not isinstance(value, Number):
+            value = Number([1], Domain([value], self))
+        if not isinstance(item, Number):
+            item = Number([1], Domain([item], self))
+        else:
+            item = self.apply(torch.round, item)
+        for i, membership in item.todict().items():
+            #if membership == 0:
+            #    continue
+            i = int(i)
+            if i < 0 or i >= len(values):
+                continue
+            membership = Number([membership], Domain([1], self))
+            values[i] = self.If(membership, value, values[i])
+
     def getlist(self, values, item, default=None):
         if not isinstance(item, Number):
             item = Number([1], Domain([item], self))
+        else:
+            item = self.apply(torch.round, item)
         result = None
         for i, membership in item.todict().items():
             #if membership == 0:
             #    continue
-            i = int(round(i))
+            i = int(i)
             if i < 0 or i >= len(values):
                 continue
             membership = Number([membership], Domain([1], self))
             result = self.combine(self.apply(operator.mul, values[i], membership), result)
         if result is None:
             if default is None:
                 return None
```

## Comparing `dufuz-0.0.1.dist-info/RECORD` & `dufuz-0.1.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 dufuz/__init__.py,sha256=qzOmaC1-_4aR1uexA7AUrGjVYKkwTeHmcmuBHq5JRvI,106
+dufuz/__main__.py,sha256=9YfPArh8Ud4FcseRCLNyqF5SuRjZsSvnqZOe5_HCsjQ,489
 dufuz/defuzzify.py,sha256=1QUztb6NRRXHe_5Ilv3m3-Ds4_E9X3wO6nAOE5KeuRk,704
-dufuz/dfn.py,sha256=i9BtARREaijJAuLqnN5WlgpR6etgKoO26hf9DAPWuZ8,1917
+dufuz/dfn.py,sha256=_iHuiW41O5E4yunbVsCBTlb6Kekc9mFTTTUBdmm1KX8,2298
 dufuz/monitor.py,sha256=PpTckJVU1MdqZMBmOzIKYSJByNtFmzo30Hj30rmHWkA,653
 dufuz/tnorm.py,sha256=1P2mKnsdFfeo6hM5cXpg1CN5G9wokzdVsKcPa56FJk0,339
 dufuz/core/__init__.py,sha256=d5UUP4Ul9gVsEjDy3ukyWPYEy-1lfHRyxbH_MbSq9gU,104
-dufuz/core/domain.py,sha256=en1pK2xWxDq4fmoRAMVCTkDcoLvJvU9PZHRkNeq80yk,1085
-dufuz/core/environment.py,sha256=uj1kzjhQmfuS4E8hh3bkgRa01vEzUkWg0B52mO_TpYM,6298
+dufuz/core/domain.py,sha256=31OmdzQ036neaUtpRZ7Sfa2GSbcGZABi1DacpCN1KHA,1150
+dufuz/core/environment.py,sha256=KOTcUkkSGIOON8bUWMldjjHoqLBp7LoljBbbI21dhsM,7073
 dufuz/core/number.py,sha256=JFtr9t3mrX3_8gfRQABxYw_xP8pmqDvTICJnPHwjVHY,3545
-dufuz-0.0.1.dist-info/METADATA,sha256=b7YemDdD6svRW24UGc2LC4ySBS8jY5_Ue2O3PSmBYeE,2059
-dufuz-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dufuz-0.0.1.dist-info/top_level.txt,sha256=uOCyq9ewMXY6duF8r0nDnXUzV3tAbqwAyt1x2L0EAHY,6
-dufuz-0.0.1.dist-info/RECORD,,
+dufuz/interpreter/__init__.py,sha256=A8zHBTrxIcsDCogfkoHKBez9fNMvQurRCW2LsIqoZZ8,49
+dufuz/interpreter/interpret.py,sha256=2nhdgs4W6QdyBhrbPC-09p0GLYKJsr0AMWU1nZQ9hgA,9475
+dufuz/interpreter/lexer.py,sha256=gdI9JT-GkiyARO3DzSSJ2MfEHSqr-1iMRfAF7cSKvgY,1000
+dufuz/interpreter/parser.py,sha256=OUX86H0nXIwINWOOYKL3bWVha6PuFDxZbpdoKiT1hNg,4038
+dufuz-0.1.0.dist-info/METADATA,sha256=wQXgd74c7ZqhzCh237ziHclmwMty43HfI2XzFliDULU,880
+dufuz-0.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dufuz-0.1.0.dist-info/top_level.txt,sha256=uOCyq9ewMXY6duF8r0nDnXUzV3tAbqwAyt1x2L0EAHY,6
+dufuz-0.1.0.dist-info/RECORD,,
```

