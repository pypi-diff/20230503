# Comparing `tmp/nobus-0.1.4.tar.gz` & `tmp/nobus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobus-0.1.4.tar", max compression
+gzip compressed data, was "nobus-0.1.5.tar", max compression
```

## Comparing `nobus-0.1.4.tar` & `nobus-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.4/LICENSE
--rw-r--r--   0        0        0     1081 2023-04-22 16:46:49.568611 nobus-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.4/nobus/__init__.py
--rw-r--r--   0        0        0    11566 2023-04-23 09:14:45.535948 nobus-0.1.4/nobus/safeattr.py
--rw-r--r--   0        0        0      256 2023-04-23 09:17:34.713283 nobus-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 nobus-0.1.4/setup.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 nobus-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-22 15:17:25.200487 nobus-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1255 2023-04-23 09:31:08.833625 nobus-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 15:22:41.911187 nobus-0.1.5/nobus/__init__.py
+-rw-r--r--   0        0        0    12604 2023-05-01 16:13:38.715804 nobus-0.1.5/nobus/safeattr.py
+-rw-r--r--   0        0        0      256 2023-05-03 09:47:26.444447 nobus-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 nobus-0.1.5/setup.py
+-rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 nobus-0.1.5/PKG-INFO
```

### Comparing `nobus-0.1.4/LICENSE` & `nobus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nobus-0.1.4/README.md` & `nobus-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # nobus
 "Nobody But Us" modules for Python
 
-## What is nobus
+# What is nobus
 [NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。
 
 `nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。
 
 現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。
 
 そのうち関数型プログラミングモジュールの `kette` を統合する予定です。
 
 本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。
 
 * Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)
 * Twitter: [@wsuzume](https://twitter.com/wsuzume)
 
-## Usage
+# Usage
+## install
 ```
 $ pip install nobus
 ```
+
+## safeattr.py
+いまのところは[この Zenn の記事](https://zenn.dev/wsuzume/articles/fd6bb1d6b792d7)をドキュメント代わりにしてください。
```

### Comparing `nobus-0.1.4/nobus/safeattr.py` & `nobus-0.1.5/nobus/safeattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,116 +12,131 @@
         return self._function(x)
 
 def typechecker(function):
     return TypeChecker(function)
 
 class Typed:
     @staticmethod
-    def _typecheck(value, type_, optional):
+    def _typecheck(value, type_, f, optional):
         if value is None:
             if optional:
                 # optional で None なら OK
-                return
+                return None
             # optional じゃないのに value が None である 
             raise TypeError(f"value is None even though it is not optional.")
         
+        # f が None でなければ変換
+        if f is not None:
+            value = f(value)
+
         # 以降は value が None ではない
         if (type_ is not None):
             # 型が指定されてるならチェックを入れる
             if isinstance(type_, TypeChecker):
                 if type_(value):
-                    return
+                    return value
                 raise TypeError(f"typechecking by '{type_}' returned False.")
 
             if isinstance(value, type_):
-                return True
+                return value
             raise TypeError(f"value must be instance of {type_} but actual type {type(value)}.")
 
-        return
+        return value
     
     def typecheck(self, value):
-        self._typecheck(value, self.type, self.optional)
-        return value
+        return self._typecheck(value, self.type, self.f, self.optional)
 
-    def __init__(self, value, type_=None, optional=False):
+    def __init__(self, value, type_=None, *, f=None, optional=False):
         self._type = type_
+        self._f = f
         self._optional = optional
 
         self._value = self.typecheck(value)
 
     def __repr__(self):
         xs = f"{self.__class__.__name__}(value={self.value.__repr__()}"
         if self.type is not None:
             xs += f", type_={self.type}"
+        if self.f is not None:
+            xs += f", f={self.f.__name__}"
         xs += f", optional={self.optional.__repr__()}"
         xs += ")"
         return xs
         
     @property
     def value(self):
         return self._value
     
     @property
     def type(self):
         return self._type
     
     @property
+    def f(self):
+        return self._f
+
+    @property
     def optional(self):
         return self._optional
     
     @value.setter
     def value(self, value):
         # value が Typed で、自身の型とマッチしない場合はエラー
         if isinstance(value, Typed) and (value.type is not None):
             if (self.type is not None) and (self.type != value.type):
                 raise TypeError(f"value must be instance of {self.type} but actual type {value.type}.")
         
         if isinstance(value, Typed):
+            # Typed の場合は unwrap する
+            # f で変換済みとみなす
             value = value.value
+        elif self.f is not None:
+            # 変換が定義されている場合は適用する
+            value = self.f(value)
 
         # value に対して型チェック
         self._value = self.typecheck(value)
     
 class Immutable(Typed):
-    def __init__(self, value, type_=None, optional=False):
-        super().__init__(value, type_, optional)
+    def __init__(self, value, type_=None, *, f=None, optional=False):
+        super().__init__(value, type_, f=f, optional=optional)
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
         raise AttributeError(f"immutable attribute 'value' cannot be rewritten.")
 
 class Protected(Typed):
-    def __init__(self, value, type_=None, optional=False):
-        super().__init__(value, type_, optional)
+    def __init__(self, value, type_=None, *, f=None, optional=False):
+        super().__init__(value, type_, f=f, optional=optional)
 
-def typed(value, type_=None, optional=False):
-    return Typed(value, type_, optional)
+def typed(value, type_=None, *, f=None, optional=False):
+    return Typed(value, type_, f=f, optional=optional)
 
-def immutable(value, type_=None, optional=False):
-    return Immutable(value, type_, optional)
+def immutable(value, type_=None, *, f=None, optional=False):
+    return Immutable(value, type_, f=f, optional=optional)
 
-def protected(value, type_=None, optional=False):
-    return Protected(value, type_, optional)    
+def protected(value, type_=None, *, f=None, optional=False):
+    return Protected(value, type_, f=f, optional=optional)    
 
 class SafeAttrABC(ABC):
     @staticmethod
-    def typed(x, type_=None, optional=False):
-        return Typed(x, type_, optional)
+    def typed(x, type_=None, *, f=None, optional=False):
+        return Typed(x, type_, f=f, optional=optional)
     
     @staticmethod
-    def immutable(x, type_=None, optional=False):
-        return Immutable(x, type_, optional)
+    def immutable(x, type_=None, *, f=None, optional=False):
+        return Immutable(x, type_, f=f, optional=optional)
 
     @staticmethod
-    def protected(x, type_=None, optional=False):
-        return Protected(x, type_, optional)
+    def protected(x, type_=None, *, f=None, optional=False):
+        return Protected(x, type_, f=f, optional=optional)
     
     def _safeattr_derive(self):
         if self.is_safeattr_derived_class:
             return
         
         cls = self.__class__
         super().__setattr__('_is_safeattr_derived_class', True)
@@ -260,21 +275,26 @@
         setattr(self.__class__, name, property(getter_of(name), setter_of(name)))
         
         # メソッドの引数を優先して返す
         def selector_of(name):
             def arg_override(self, x=None, f=None, typecheck=True):
                 if x is None:
                     return getattr(self, name)
-                
+
+                attr = getattr(self, '_safeattr_' + name)
                 if f is not None:
+                    # 型キャストが指定されていれば適用
                     x = f(x)
+                elif attr.f is not None:
+                    # 定義時に指定されたキャストあれば適用
+                    x = attr.f(x)
                 
+                # 必要なキャストは行われているはずなので f=None でよい
                 if typecheck:
-                    attr = getattr(self, '_safeattr_' + name)
-                    return attr.typecheck(x)
+                    return attr._typecheck(x, attr.type, f=None, optional=attr.optional)
                     
                 return x
                 
             return arg_override
         
         # arg_override を追加する
         super().__setattr__('arg_' + name, MethodType(selector_of(name), self))
```

### Comparing `nobus-0.1.4/setup.py` & `nobus-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['nobus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'nobus',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
-    'long_description': '# nobus\n"Nobody But Us" modules for Python\n\n## What is nobus\n[NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。\n\n`nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。\n\n現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。\n\nそのうち関数型プログラミングモジュールの `kette` を統合する予定です。\n\n本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。\n\n* Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)\n* Twitter: [@wsuzume](https://twitter.com/wsuzume)\n\n## Usage\n```\n$ pip install nobus\n```\n',
+    'long_description': '# nobus\n"Nobody But Us" modules for Python\n\n# What is nobus\n[NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。\n\n`nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。\n\n現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。\n\nそのうち関数型プログラミングモジュールの `kette` を統合する予定です。\n\n本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。\n\n* Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)\n* Twitter: [@wsuzume](https://twitter.com/wsuzume)\n\n# Usage\n## install\n```\n$ pip install nobus\n```\n\n## safeattr.py\nいまのところは[この Zenn の記事](https://zenn.dev/wsuzume/articles/fd6bb1d6b792d7)をドキュメント代わりにしてください。\n',
     'author': 'Josh Nobus',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nobus-0.1.4/PKG-INFO` & `nobus-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobus
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: MIT
 Author: Josh Nobus
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,26 +12,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # nobus
 "Nobody But Us" modules for Python
 
-## What is nobus
+# What is nobus
 [NOBUS（Nobody But Us）](https://en.wikipedia.org/wiki/NOBUS)は「我々（United States）だけが利用できる脆弱性」を意味するアメリカ国家安全保証局（NSA）の標語です。
 
 `nobus` モジュールはごく一部の変人しか使わないであろう、Python の特殊メソッドをフル活用したクラスハッキングを詰め込んだモジュールです。
 
 現在は Python のクラスアトリビュートに対して型チェックと immutable / protected 属性を追加する `safeattr` モジュールが実装されています。
 
 そのうち関数型プログラミングモジュールの `kette` を統合する予定です。
 
 本当に暇なときしか整備できないのでドキュメントはそのうち整備します。基本的に Zenn の記事をドキュメント代わりにしてください。
 
 * Zenn: [Josh Nobus (@wsuzume)](https://zenn.dev/wsuzume)
 * Twitter: [@wsuzume](https://twitter.com/wsuzume)
 
-## Usage
+# Usage
+## install
 ```
 $ pip install nobus
 ```
 
+## safeattr.py
+いまのところは[この Zenn の記事](https://zenn.dev/wsuzume/articles/fd6bb1d6b792d7)をドキュメント代わりにしてください。
+
```

