# Comparing `tmp/genluhn-0.3.0.tar.gz` & `tmp/genluhn-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genluhn-0.3.0.tar", last modified: Tue Oct  5 12:36:35 2021, max compression
+gzip compressed data, was "genluhn-0.3.1.tar", last modified: Wed May  3 17:16:18 2023, max compression
```

## Comparing `genluhn-0.3.0.tar` & `genluhn-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-10-05 12:36:35.447082 genluhn-0.3.0/
--rw-r--r--   0 jmfernandez (10012) users      (100)    26530 2021-05-10 11:31:13.000000 genluhn-0.3.0/LICENSE.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       58 2021-09-29 11:06:48.000000 genluhn-0.3.0/MANIFEST.in
--rw-r--r--   0 jmfernandez (10012) users      (100)     2429 2021-10-05 12:36:35.447082 genluhn-0.3.0/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)     1746 2021-05-10 20:58:33.000000 genluhn-0.3.0/README.md
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-10-05 12:36:35.446082 genluhn-0.3.0/genluhn/
--rw-r--r--   0 jmfernandez (10012) users      (100)     4645 2021-05-10 20:55:21.000000 genluhn-0.3.0/genluhn/__init__.py
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-10-05 12:36:35.447082 genluhn-0.3.0/genluhn.egg-info/
--rw-r--r--   0 jmfernandez (10012) users      (100)     2429 2021-10-05 12:36:35.000000 genluhn-0.3.0/genluhn.egg-info/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)      201 2021-10-05 12:36:35.000000 genluhn-0.3.0/genluhn.egg-info/SOURCES.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        1 2021-10-05 12:36:35.000000 genluhn-0.3.0/genluhn.egg-info/dependency_links.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        8 2021-10-05 12:36:35.000000 genluhn-0.3.0/genluhn.egg-info/top_level.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 genluhn-0.3.0/pyproject.toml
--rw-r--r--   0 jmfernandez (10012) users      (100)       38 2021-10-05 12:36:35.447082 genluhn-0.3.0/setup.cfg
--rw-r--r--   0 jmfernandez (10012) users      (100)     2645 2021-10-05 12:29:36.000000 genluhn-0.3.0/setup.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-03 17:16:18.992776 genluhn-0.3.1/
+-rw-r--r--   0 jmfernandez (10012) users      (100)    26530 2021-05-10 11:31:13.000000 genluhn-0.3.1/LICENSE.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       63 2021-10-05 12:39:48.000000 genluhn-0.3.1/MANIFEST.in
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2409 2023-05-03 17:16:18.992776 genluhn-0.3.1/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1746 2021-05-10 20:58:33.000000 genluhn-0.3.1/README.md
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-03 17:16:18.992776 genluhn-0.3.1/genluhn/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     5059 2023-05-03 17:10:20.000000 genluhn-0.3.1/genluhn/__init__.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)        0 2023-05-03 17:13:08.000000 genluhn-0.3.1/genluhn/py.typed
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-03 17:16:18.992776 genluhn-0.3.1/genluhn.egg-info/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2409 2023-05-03 17:16:18.000000 genluhn-0.3.1/genluhn.egg-info/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)      218 2023-05-03 17:16:18.000000 genluhn-0.3.1/genluhn.egg-info/SOURCES.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        1 2023-05-03 17:16:18.000000 genluhn-0.3.1/genluhn.egg-info/dependency_links.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        8 2023-05-03 17:16:18.000000 genluhn-0.3.1/genluhn.egg-info/top_level.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 genluhn-0.3.1/pyproject.toml
+-rw-r--r--   0 jmfernandez (10012) users      (100)       38 2023-05-03 17:16:18.992776 genluhn-0.3.1/setup.cfg
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2587 2023-05-03 17:15:37.000000 genluhn-0.3.1/setup.py
```

### Comparing `genluhn-0.3.0/LICENSE.txt` & `genluhn-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genluhn-0.3.0/PKG-INFO` & `genluhn-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: genluhn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generalized Luhn algorithm to any numeric base
 Home-page: https://github.com/inab/genluhn
 Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
 Author-email: jose.m.fernandez@bsc.es
 License: LGPL-2.1
 Project-URL: Bug Tracker, https://github.com/inab/genluhn/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -33,9 +32,7 @@
 
 genluhn.validate('5326-9057-e12f-e2b7-4ba0-7c89-2560-a2', 16, 14)
 # It returns False
 ```
 
 
 Accessory methods of this library are `intToDigits`, `strToDigits` and `bytesToDigits`, which are used when either an integer, or a string or a byteslike object have to be translated to a list of digits in the given numerical base.
-
-
```

### Comparing `genluhn-0.3.0/README.md` & `genluhn-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `genluhn-0.3.0/genluhn/__init__.py` & `genluhn-0.3.1/genluhn/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # genluhn, a library to compute and validate Luhn check digit on any base
-# Copyright (C) 2021 Barcelona Supercomputinh Center, José M. Fernández
+# Copyright (C) 2021-2023 Barcelona Supercomputinh Center, José M. Fernández
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
@@ -14,131 +14,168 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-__author__ = 'José M. Fernández <https://orcid.org/0000-0002-4806-5140>'
-__copyright__ = '© 2021 Barcelona Supercomputing Center (BSC), ES'
-__license__ = 'LGPL-2.1'
+__author__ = "José M. Fernández <https://orcid.org/0000-0002-4806-5140>"
+__copyright__ = "© 2021-2023 Barcelona Supercomputing Center (BSC), ES"
+__license__ = "LGPL-2.1"
 
 # https://www.python.org/dev/peps/pep-0396/
-__version__ = '0.3.0'
+__version__ = "0.3.1"
 
-from typing import List, NewType, Union
+from typing import (
+	cast,
+	TYPE_CHECKING,
+)
+
+if TYPE_CHECKING:
+	from typing import (
+		MutableSequence,
+		NewType,
+		Sequence,
+		Union,
+	)
 
-Digit = NewType('Digit', int)
-Digits = List[Digit]
+	Digit = NewType("Digit", int)
+	Digits = Sequence[Digit]
 
-def intToDigits(number:int, base:int) -> Digits:
+
+def intToDigits(number: "int", base: "int") -> "Digits":
 	"""
 	This method translates any integer to the digits notation
 	"""
-	
+
 	# We are only going to deal with positive numbers
 	if number < 0:
 		number = -number
-	
-	digits = []
+
+	digits: "MutableSequence[Digit]" = []
 	while number >= base:
-		digits.append(int(number % base))
-		digits //= base
-	digits.append(number)
-	
+		digits.append(cast("Digit", int(number % base)))
+		number //= base
+	digits.append(cast("Digit", number))
+
 	# Now, reverse it before returning it
 	digits.reverse()
-	
+
 	return digits
 
-MAX_STRTODIGITS_BASE = ord('z') - ord('a') + 1 + ord('9') - ord('0') + 1
 
-def strToDigits(numstr:str, base:int) -> Digits:
+MAX_STRTODIGITS_BASE = ord("z") - ord("a") + 1 + ord("9") - ord("0") + 1
+
+
+def strToDigits(numstr: "str", base: "int") -> "Digits":
 	"""
 	This method translates from a string notation to a list of digits.
 	It removes dashes from the string, which are usually separators.
 	This method only works with bases from 1 to 36
 	"""
-	
+
 	if base > MAX_STRTODIGITS_BASE:
-		raise ValueError('In str representations, base can be at most {}'.format(MAX_STRTODIGITS_BASE))
-		
+		raise ValueError(
+			"In str representations, base can be at most {}".format(
+				MAX_STRTODIGITS_BASE
+			)
+		)
+
 	# First, normalize the string, by removing dashes and translating
 	# it to lower case
-	numstr = numstr.replace('-','').lower()
-	
+	numstr = numstr.replace("-", "").lower()
+
 	# Then, translate and check base validity
-	digits = []
-	ord0 = ord('0')
+	digits: "MutableSequence[Digit]" = []
+	ord0 = ord("0")
 	# Tweak
-	orda = ord('a') - 10
-	for iletter,letter in enumerate(numstr):
+	orda = ord("a") - 10
+	for iletter, letter in enumerate(numstr):
 		digit = None
 		ordletter = ord(letter)
-		if letter >= '0' and letter <= '9':
+		if letter >= "0" and letter <= "9":
 			digit = ordletter - ord0
-		elif letter >= 'a' and letter <= 'z':
+		elif letter >= "a" and letter <= "z":
 			digit = ordletter - orda
-		
+
 		if (digit is None) or digit >= base:
-			raise ValueError("Invalid symbol '{}' at position {} for base {}".format(letter, iletter, base))
-		
-		digits.append(digit)
-	
+			raise ValueError(
+				"Invalid symbol '{}' at position {} for base {}".format(
+					letter, iletter, base
+				)
+			)
+
+		digits.append(cast("Digit", digit))
+
 	return digits
 
-def bytesToDigits(byteslike:Union[bytes, bytearray], base:int) -> Digits:
+
+def bytesToDigits(byteslike: "Union[bytes, bytearray]", base: "int") -> "Digits":
 	"""
 	This method translates from a byte notation to a list of digits.
 	This method only works with bases 16 and 256
 	"""
-	
-	if base==256:
-		return list(byteslike)
-	elif base==16:
-		digits = []
+
+	if base == 256:
+		return cast("Digits", list(byteslike))
+	elif base == 16:
+		digits: "MutableSequence[Digit]" = []
 		for bytelike in byteslike:
-			digits.append((bytelike & 0xF0) >> 4)
-			digits.append(bytelike & 0x0F)
+			digits.append(cast("Digit", (bytelike & 0xF0) >> 4))
+			digits.append(cast("Digit", bytelike & 0x0F))
 		return digits
 	else:
-		raise ValueError('In bytes representations, base can be either 16 or 256')
+		raise ValueError("In bytes representations, base can be either 16 or 256")
+
 
-def compute(digits:Union[str, int, bytes, bytearray, Digits], base:int) -> Digit:
+def compute(
+	digits: "Union[str, int, bytes, bytearray, Digits]", base: "int"
+) -> "Digit":
 	"""
 	The input are either a list of integers, representing the digits
 	of a number in a custom base, or a string representing the base
 	(for instance, in hexadecimal textual notation) or an arbitrary
 	large integer, which must be interpreted in the given base
 	"""
-	
+
 	if not isinstance(base, int) or base < 1:
-		raise ValueError('base must be an integer greater than 0')
-	
+		raise ValueError("base must be an integer greater than 0")
+
 	theDigits = None
 	if isinstance(digits, int):
 		theDigits = intToDigits(digits, base)
 	elif isinstance(digits, str):
 		theDigits = strToDigits(digits, base)
 	elif isinstance(digits, (bytes, bytearray)):
 		theDigits = bytesToDigits(digits, base)
-	elif isinstance(digits, (list,tuple)):
+	elif isinstance(digits, (list, tuple)):
 		for idigit, digit in enumerate(digits):
 			if digit < 0 or digit >= base:
-				raise ValueError("Invalid digit '{}' at position {} for base {}".format(digit, idigit, base))
-				
+				raise ValueError(
+					"Invalid digit '{}' at position {} for base {}".format(
+						digit, idigit, base
+					)
+				)
+
 		theDigits = digits
 	else:
 		raise ValueError("digits must be either an int, a str, or an array of int")
-	
+
 	sumidx = len(theDigits) % 2
-	
+
 	# Half is summed
 	partial = sum(theDigits[sumidx::2])
 	# Half is doubled, digit summed and summed
-	partial += sum(map(lambda d: sum(divmod(2*d, base)), theDigits[(1-sumidx)::2]))
-	partial *= (base-1)
-		
-	return partial % base
+	partial += sum(
+		map(lambda d: sum(divmod(2 * d, base)), theDigits[(1 - sumidx) :: 2])
+	)
+	partial *= base - 1
+
+	return cast("Digit", partial % base)
+
 
-def validate(digits:Union[str, int, bytes, bytearray, Digits], base:int, checkdigit:Digit) -> bool:
-	return compute(digits, base) == checkdigit
+def validate(
+	digits: "Union[str, int, bytes, bytearray, Digits]",
+	base: "int",
+	checkdigit: "Digit",
+) -> "bool":
+	return compute(digits, base) == checkdigit
```

### Comparing `genluhn-0.3.0/genluhn.egg-info/PKG-INFO` & `genluhn-0.3.1/genluhn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: genluhn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generalized Luhn algorithm to any numeric base
 Home-page: https://github.com/inab/genluhn
 Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
 Author-email: jose.m.fernandez@bsc.es
 License: LGPL-2.1
 Project-URL: Bug Tracker, https://github.com/inab/genluhn/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -33,9 +32,7 @@
 
 genluhn.validate('5326-9057-e12f-e2b7-4ba0-7c89-2560-a2', 16, 14)
 # It returns False
 ```
 
 
 Accessory methods of this library are `intToDigits`, `strToDigits` and `bytesToDigits`, which are used when either an integer, or a string or a byteslike object have to be translated to a list of digits in the given numerical base.
-
-
```

