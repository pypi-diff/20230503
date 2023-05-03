# Comparing `tmp/name_genie-0.0.1.tar.gz` & `tmp/name_genie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_genie-0.0.1.tar", max compression
+gzip compressed data, was "name_genie-0.0.2.tar", max compression
```

## Comparing `name_genie-0.0.1.tar` & `name_genie-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2023-05-02 18:11:10.353020 name_genie-0.0.1/LICENSE
--rw-r--r--   0        0        0      158 2023-05-02 18:11:10.353020 name_genie-0.0.1/README.md
--rw-r--r--   0        0        0      227 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/alchemy.py
--rw-r--r--   0        0        0     1709 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/book.py
--rw-r--r--   0        0        0     1098 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/clan.py
--rw-r--r--   0        0        0    22083 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/common.py
--rw-r--r--   0        0        0     1396 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/creature.py
--rw-r--r--   0        0        0     1377 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/dao.py
--rw-r--r--   0        0        0     1519 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/material.py
--rw-r--r--   0        0        0     1974 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/name.py
--rw-r--r--   0        0        0     1484 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/nation.py
--rw-r--r--   0        0        0     1097 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/place.py
--rw-r--r--   0        0        0     2166 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/skill.py
--rw-r--r--   0        0        0     1793 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/talisman.py
--rw-r--r--   0        0        0      119 2023-05-02 18:11:10.353020 name_genie-0.0.1/name_genie/util.py
--rw-r--r--   0        0        0      443 2023-05-02 18:11:10.353020 name_genie-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 name_genie-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 18:33:14.667909 name_genie-0.0.2/LICENSE
+-rw-r--r--   0        0        0      158 2023-05-02 18:33:14.667909 name_genie-0.0.2/README.md
+-rw-r--r--   0        0        0      348 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/alchemy.py
+-rw-r--r--   0        0        0     1731 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/book.py
+-rw-r--r--   0        0        0     1120 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/clan.py
+-rw-r--r--   0        0        0    22083 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/common.py
+-rw-r--r--   0        0        0     1418 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/creature.py
+-rw-r--r--   0        0        0     1399 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/dao.py
+-rw-r--r--   0        0        0     1541 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/material.py
+-rw-r--r--   0        0        0     1996 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/name.py
+-rw-r--r--   0        0        0     1506 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/nation.py
+-rw-r--r--   0        0        0     1119 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/place.py
+-rw-r--r--   0        0        0     2188 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/skill.py
+-rw-r--r--   0        0        0     1815 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/talisman.py
+-rw-r--r--   0        0        0      119 2023-05-02 18:33:14.667909 name_genie-0.0.2/name_genie/util.py
+-rw-r--r--   0        0        0      443 2023-05-02 18:33:14.667909 name_genie-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 name_genie-0.0.2/PKG-INFO
```

### Comparing `name_genie-0.0.1/LICENSE` & `name_genie-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `name_genie-0.0.1/name_genie/alchemy.py` & `name_genie-0.0.2/name_genie/alchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_alchemy_suffix,data_shared_action, data_shared_color, data_shared_dao, data_shared_element, data_shared_number
-from util import to_str
+from name_genie.common import data_alchemy_suffix,data_shared_action, data_shared_color, data_shared_dao, data_shared_element, data_shared_number
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_alchemies']
 
 
 stems = data_shared_action + data_shared_color + data_shared_dao + data_shared_element + data_shared_number
```

### Comparing `name_genie-0.0.1/name_genie/book.py` & `name_genie-0.0.2/name_genie/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_book_state, data_book_suffix, data_book_interfix, data_shared_dao, data_shared_element, data_shared_creature, data_shared_thing, data_shared_adj, data_shared_number, data_shared_gesture, data_shared_action
-from util import to_str
+from name_genie.common import data_book_state, data_book_suffix, data_book_interfix, data_shared_dao, data_shared_element, data_shared_creature, data_shared_thing, data_shared_adj, data_shared_number, data_shared_gesture, data_shared_action
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_books']
 
 
 stems = data_shared_dao + data_shared_element + data_shared_creature + data_shared_thing + data_shared_adj + data_shared_number + data_shared_gesture + data_shared_action
```

### Comparing `name_genie-0.0.1/name_genie/clan.py` & `name_genie-0.0.2/name_genie/clan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_clan_suffix, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
-from util import to_str
+from name_genie.common import data_clan_suffix, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_clans']
 
 stems = data_shared_action + data_shared_adj + data_shared_creature + data_shared_dao + data_shared_element + data_shared_gesture + data_shared_thing
```

### Comparing `name_genie-0.0.1/name_genie/common.py` & `name_genie-0.0.2/name_genie/common.py`

 * *Files identical despite different names*

### Comparing `name_genie-0.0.1/name_genie/creature.py` & `name_genie-0.0.2/name_genie/creature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_creature_interfix, data_creature_suffix, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
-from util import to_str
+from name_genie.common import data_creature_interfix, data_creature_suffix, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_creatures']
 
 stems = data_shared_action + data_shared_adj + data_shared_creature + data_shared_dao + data_shared_element + data_shared_gesture + data_shared_thing
```

### Comparing `name_genie-0.0.1/name_genie/dao.py` & `name_genie-0.0.2/name_genie/dao.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_dao_stem, data_dao_male_suffix, data_dao_female_suffix, data_shared_dao, data_shared_thing, data_shared_adj, data_shared_number
-from util import to_str
+from name_genie.common import data_dao_stem, data_dao_male_suffix, data_dao_female_suffix, data_shared_dao, data_shared_thing, data_shared_adj, data_shared_number
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_daos']
 
 
 stems = data_dao_stem + data_shared_dao + data_shared_thing + data_shared_adj + data_shared_number
 suffixes = data_dao_male_suffix + data_dao_female_suffix
```

### Comparing `name_genie-0.0.1/name_genie/material.py` & `name_genie-0.0.2/name_genie/material.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_material_state, data_material_suffix, data_shared_dao, data_shared_element, data_shared_color, data_shared_creature, data_shared_thing, data_shared_adj, data_shared_number, data_shared_gesture, data_shared_action
-from util import to_str
+from name_genie.common import data_material_state, data_material_suffix, data_shared_dao, data_shared_element, data_shared_color, data_shared_creature, data_shared_thing, data_shared_adj, data_shared_number, data_shared_gesture, data_shared_action
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_materials']
 
 
 stems = data_shared_dao + data_shared_element + data_shared_color + data_shared_creature + data_shared_thing + data_shared_adj + data_shared_number + data_shared_gesture + data_shared_action
```

### Comparing `name_genie-0.0.1/name_genie/name.py` & `name_genie-0.0.2/name_genie/name.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_name_prefix, data_name_interfix, data_name_male_suffix, data_name_female_suffix
-from util import to_str
+from name_genie.common import data_name_prefix, data_name_interfix, data_name_male_suffix, data_name_female_suffix
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_names']
 
 
 interfixes = data_name_male_suffix + data_name_female_suffix + data_name_interfix
```

### Comparing `name_genie-0.0.1/name_genie/nation.py` & `name_genie-0.0.2/name_genie/nation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_nation_interfix, data_nation_suffix, data_shared_place
-from util import to_str
+from name_genie.common import data_nation_interfix, data_nation_suffix, data_shared_place
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_nations']
 
 
 def get_nations(count: int = 10,
                 length: int | None = None,
```

### Comparing `name_genie-0.0.1/name_genie/place.py` & `name_genie-0.0.2/name_genie/place.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_place_suffix, data_shared_place
-from util import to_str
+from name_genie.common import data_place_suffix, data_shared_place
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_places']
 
 
 def get_places(count: int = 10,
                length: int | None = None,
```

### Comparing `name_genie-0.0.1/name_genie/skill.py` & `name_genie-0.0.2/name_genie/skill.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_skill_numfix, data_skill_prefix, data_skill_suffix, data_shared_number, data_shared_clan, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
-from util import to_str
+from name_genie.common import data_skill_numfix, data_skill_prefix, data_skill_suffix, data_shared_number, data_shared_clan, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_skills']
 
 stems = data_shared_number + data_shared_clan + data_shared_action + data_shared_adj + data_shared_creature + data_shared_dao + data_shared_element + data_shared_gesture + data_shared_thing
```

### Comparing `name_genie-0.0.1/name_genie/talisman.py` & `name_genie-0.0.2/name_genie/talisman.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from common import data_talisman_state, data_talisman_interfix, data_talisman_suffix, data_shared_number, data_shared_clan, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
-from util import to_str
+from name_genie.common import data_talisman_state, data_talisman_interfix, data_talisman_suffix, data_shared_number, data_shared_clan, data_shared_action, data_shared_adj, data_shared_creature, data_shared_dao, data_shared_element, data_shared_gesture, data_shared_thing
+from name_genie.util import to_str
 import random
 
 __all__ = ['get_talismans']
 
 stems = data_shared_number + data_shared_clan + data_shared_action + data_shared_adj + data_shared_creature + data_shared_dao + data_shared_element + data_shared_gesture + data_shared_thing
```

### Comparing `name_genie-0.0.1/PKG-INFO` & `name_genie-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-genie
-Version: 0.0.1
+Version: 0.0.2
 Summary: 一个用于生成名字的工具
 Home-page: https://github.com/name-genie/name-genie-python
 License: MIT
 Author: lhlyu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

