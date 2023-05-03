# Comparing `tmp/djangocms_xliff-1.2.0.tar.gz` & `tmp/djangocms_xliff-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_xliff-1.2.0.tar", max compression
+gzip compressed data, was "djangocms_xliff-1.3.0.tar", max compression
```

## Comparing `djangocms_xliff-1.2.0.tar` & `djangocms_xliff-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/LICENSE
--rw-r--r--   0        0        0     7132 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/README.md
--rw-r--r--   0        0        0       22 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/__init__.py
--rw-r--r--   0        0        0      216 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/apps.py
--rw-r--r--   0        0        0     2186 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/cms_toolbars.py
--rw-r--r--   0        0        0      186 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/exceptions.py
--rw-r--r--   0        0        0     1276 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/exports.py
--rw-r--r--   0        0        0     7317 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/extractors.py
--rw-r--r--   0        0        0      801 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/forms.py
--rw-r--r--   0        0        0     3642 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/imports.py
--rw-r--r--   0        0        0     4022 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5560 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/__init__.py
--rw-r--r--   0        0        0     1804 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_export.py
--rw-r--r--   0        0        0     1704 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_import.py
--rw-r--r--   0        0        0     1623 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_page_plugins.py
--rw-r--r--   0        0        0     5662 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/parsers.py
--rw-r--r--   0        0        0     1148 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/renderer.py
--rw-r--r--   0        0        0     1494 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/settings.py
--rw-r--r--   0        0        0      193 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/base.html
--rw-r--r--   0        0        0      151 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/error.html
--rw-r--r--   0        0        0      522 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/index.html
--rw-r--r--   0        0        0     1000 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
--rw-r--r--   0        0        0     1389 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html
--rw-r--r--   0        0        0     1116 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/success.html
--rw-r--r--   0        0        0      447 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/upload.html
--rw-r--r--   0        0        0     2152 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/types.py
--rw-r--r--   0        0        0      589 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/urls.py
--rw-r--r--   0        0        0     3652 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/utils.py
--rw-r--r--   0        0        0     6931 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/views.py
--rw-r--r--   0        0        0     1364 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7132 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/apps.py
+-rw-r--r--   0        0        0     2515 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/cms_toolbars.py
+-rw-r--r--   0        0        0      186 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/exports.py
+-rw-r--r--   0        0        0     9102 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/extractors.py
+-rw-r--r--   0        0        0      801 2023-05-03 13:02:46.514256 djangocms_xliff-1.3.0/djangocms_xliff/forms.py
+-rw-r--r--   0        0        0     4297 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/imports.py
+-rw-r--r--   0        0        0     4022 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5560 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_export.py
+-rw-r--r--   0        0        0     1704 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_import.py
+-rw-r--r--   0        0        0     1623 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_page_plugins.py
+-rw-r--r--   0        0        0     5662 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/parsers.py
+-rw-r--r--   0        0        0     1148 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/renderer.py
+-rw-r--r--   0        0        0     1534 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/settings.py
+-rw-r--r--   0        0        0      193 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/base.html
+-rw-r--r--   0        0        0      151 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/error.html
+-rw-r--r--   0        0        0      522 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/index.html
+-rw-r--r--   0        0        0     1000 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
+-rw-r--r--   0        0        0     1389 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html
+-rw-r--r--   0        0        0     1116 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/success.html
+-rw-r--r--   0        0        0      447 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/upload.html
+-rw-r--r--   0        0        0     2152 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/types.py
+-rw-r--r--   0        0        0      589 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/urls.py
+-rw-r--r--   0        0        0     3919 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/utils.py
+-rw-r--r--   0        0        0     6935 2023-05-03 13:02:46.518256 djangocms_xliff-1.3.0/djangocms_xliff/views.py
+-rw-r--r--   0        0        0     1364 2023-05-03 13:02:46.522256 djangocms_xliff-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.0/PKG-INFO
```

### Comparing `djangocms_xliff-1.2.0/LICENSE` & `djangocms_xliff-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/README.md` & `djangocms_xliff-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/cms_toolbars.py` & `djangocms_xliff-1.3.0/djangocms_xliff/cms_toolbars.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def populate(self):
         super().populate()
         obj = self.get_object()
         if obj and self.user_has_permissions(obj=obj):
             self.update_language_menu(obj=obj)
 
     def get_object(self):
-        return self.toolbar.obj
+        return self.toolbar.obj or self.request.current_page
 
     def user_has_permissions(self, obj) -> bool:
         return False
 
     def update_language_menu(self, obj):
         language_menu = self.toolbar.get_menu(LANGUAGE_MENU_IDENTIFIER)
         if not language_menu:
@@ -51,17 +51,24 @@
             reverse_xliff(viewname="djangocms_xliff:upload"),
         )
 
 
 @toolbar_pool.register
 class XliffPageToolbar(XliffToolbar):
     def user_has_permissions(self, obj) -> bool:
-        if obj and type(obj) == Page and len(obj.get_languages()) > 1:
+        if hasattr(obj, "_wrapped"):  # request.current_page returns a SimpleLazyObject
+            obj = obj._wrapped
+
+        if self.toolbar.edit_mode_active and obj and type(obj) == Page and len(obj.get_languages()) > 1:
             return page_permissions.user_can_change_page(user=self.request.user, page=obj, site=self.current_site)
         return False
 
 
 class XliffModelToolbar(XliffToolbar):
+    """
+    Inherit from this class to add xliff import and export functionality to your custom models
+    """
+
     def user_has_permissions(self, obj) -> bool:
-        if obj and type(obj) != Page:
+        if self.toolbar.edit_mode_active and obj and type(obj) != Page:
             return self.request.user.has_perm(f"change_{obj._meta.model_name}")
         return False
```

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/exports.py` & `djangocms_xliff-1.3.0/djangocms_xliff/exports.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/extractors.py` & `djangocms_xliff-1.3.0/djangocms_xliff/extractors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+from contextlib import suppress
 from functools import partial
 from typing import Generator, List, Tuple, Type
 
+from cms.extensions import extension_pool
 from cms.models import CMSPlugin, Page, Placeholder, PlaceholderField, StaticPlaceholder
 from django.db.models import (
     CharField,
     Field,
     Model,
     OneToOneField,
     SlugField,
@@ -21,15 +23,15 @@
     FIELDS,
     MODEL_METADATA_FIELDS,
     TITLE_METADATA_FIELDS,
     UNIT_ID_METADATA_ID,
     VALIDATORS,
 )
 from djangocms_xliff.types import Unit, XliffObj
-from djangocms_xliff.utils import get_type_with_path
+from djangocms_xliff.utils import get_plugin_id_for_extension_obj, get_type_with_path
 
 logger = logging.getLogger(__name__)
 
 
 def has_translatable_type(field: Field) -> bool:
     return type(field) in [CharField, TextField, URLField, SlugField, *FIELDS]
 
@@ -153,21 +155,21 @@
     excluded_fields = MODEL_METADATA_FIELDS.get(obj_type, {}).get("exclude", [])
     for excluded_field in excluded_fields:
         fields.pop(excluded_field, None)
 
     return target_obj, fields
 
 
-def extract_metadata_from_obj(obj: XliffObj, language: str) -> List[Unit]:
+def extract_metadata_from_obj(
+    obj: XliffObj, language: str, plugin_id: str, plugin_type: str, plugin_name: str
+) -> List[Unit]:
     with translation.override(language):
         target_obj, fields = get_metadata_fields(obj)
 
-        model_unit = partial(
-            Unit, plugin_id=UNIT_ID_METADATA_ID, plugin_type=UNIT_ID_METADATA_ID, plugin_name=UNIT_ID_METADATA_ID
-        )
+        model_unit = partial(Unit, plugin_id=plugin_id, plugin_type=plugin_type, plugin_name=plugin_name)
 
         units = []
         for field_name, field_verbose_name in fields.items():
             target_obj_field = target_obj._meta.get_field(field_name)
 
             if not is_field_to_translate(target_obj_field, target_obj):
                 continue
@@ -190,14 +192,44 @@
                         source=target_obj_field.value_from_object(target_obj),
                         max_length=target_obj_field.max_length,
                     )
                 )
         return units
 
 
+def extract_extension_data_from_obj(obj, language: str) -> List[Unit]:
+    plugin_id = get_plugin_id_for_extension_obj(obj)
+    return extract_metadata_from_obj(
+        obj=obj,
+        language=language,
+        plugin_id=plugin_id,
+        plugin_type=obj._meta.object_name,
+        plugin_name=obj._meta.verbose_name,
+    )
+
+
+def extract_extension_data_from_page(obj: XliffObj, language: str) -> List[Unit]:
+    with translation.override(language):
+        units = []
+        for title_extension_class in extension_pool.title_extensions:
+            with suppress(title_extension_class.DoesNotExist):
+                instance = title_extension_class.objects.get(
+                    extended_object__page=obj, extended_object__language=language
+                )
+                units.extend(extract_extension_data_from_obj(obj=instance, language=language))
+
+        # In rare cases it makes sense to use translated fields on page extensions
+        for page_extension_class in extension_pool.page_extensions:
+            with suppress(page_extension_class.DoesNotExist):
+                instance = page_extension_class.objects.get(extended_object=obj)
+                units.extend(extract_extension_data_from_obj(obj=instance, language=language))
+
+        return units
+
+
 def extract_units_from_obj(obj: XliffObj, language: str, include_metadata=True) -> List[Unit]:
     plugin_units = []
 
     for placeholder in get_placeholders(obj):
         logger.debug(
             f"Placeholder: {placeholder.pk}, is_static={placeholder.is_static}, "
             f"is_editable={placeholder.is_editable}, label={placeholder.get_label()}"
@@ -205,10 +237,22 @@
         plugin_units.extend(extract_units_from_placeholder(placeholder, language))
 
     if len(plugin_units) == 0:
         raise XliffExportError(_("No plugins found. You need to copy plugins from an existing page"))
 
     metadata_units = []
     if include_metadata:
-        metadata_units.extend(extract_metadata_from_obj(obj, language))
+        metadata_units.extend(
+            extract_metadata_from_obj(
+                obj=obj,
+                language=language,
+                plugin_id=UNIT_ID_METADATA_ID,
+                plugin_type=UNIT_ID_METADATA_ID,
+                plugin_name=UNIT_ID_METADATA_ID,
+            )
+        )
+
+    extension_data_units = []
+    if type(obj) == Page:
+        extension_data_units.extend(extract_extension_data_from_page(obj, language))
 
-    return [*metadata_units, *plugin_units]
+    return [*metadata_units, *extension_data_units, *plugin_units]
```

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/forms.py` & `djangocms_xliff-1.3.0/djangocms_xliff/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/imports.py` & `djangocms_xliff-1.3.0/djangocms_xliff/imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 from typing import List
 
 from cms.models import CMSPlugin, Page
 from django.utils import translation
 from django.utils.translation import gettext as _
 
 from djangocms_xliff.exceptions import XliffImportError
-from djangocms_xliff.settings import FIELD_IMPORTERS, UNIT_ID_METADATA_ID
+from djangocms_xliff.settings import (
+    FIELD_IMPORTERS,
+    UNIT_ID_DELIMITER,
+    UNIT_ID_EXTENSION_DATA_ID,
+    UNIT_ID_METADATA_ID,
+)
 from djangocms_xliff.types import Unit, XliffContext, XliffObj
-from djangocms_xliff.utils import get_lang_name
+from djangocms_xliff.utils import get_lang_name, get_obj
 
 logger = logging.getLogger(__name__)
 
 
 def save_xliff_units_for_metadata(units: List[Unit], obj: XliffObj, target_language: str) -> None:
     with translation.override(target_language):
         if type(obj) == Page:
@@ -23,14 +28,25 @@
             target = unit.target
 
             setattr(obj, field_name, target)
 
         obj.save()
 
 
+def save_xliff_units_for_extension_data(units: List[Unit], target_language: str) -> None:
+    with translation.override(target_language):
+        for unit in units:
+            content_type_id, instance_id, field_name = unit.field_name.split(UNIT_ID_DELIMITER)
+            obj = get_obj(int(content_type_id), int(instance_id))
+
+            target = unit.target
+            setattr(obj, field_name, target)
+            obj.save()
+
+
 def save_xliff_units_for_cms_plugin(units: List[Unit], plugin_id: str) -> None:
     try:
         cms_plugin = CMSPlugin.objects.get(pk=plugin_id)
     except CMSPlugin.DoesNotExist:
         logger.debug(f"Found plugin with id: {plugin_id} in xliff, but not in database")
         return
 
@@ -48,14 +64,16 @@
     instance.save()
 
 
 def save_xliff_context(xliff_context: XliffContext) -> None:
     for plugin_id, units in xliff_context.grouped_units:
         if plugin_id == UNIT_ID_METADATA_ID:
             save_xliff_units_for_metadata(units, xliff_context.obj, xliff_context.target_language)
+        elif plugin_id.startswith(UNIT_ID_EXTENSION_DATA_ID):
+            save_xliff_units_for_extension_data(units, xliff_context.target_language)
         else:
             save_xliff_units_for_cms_plugin(units, plugin_id)
 
 
 def validate_page_with_xliff_context(obj: XliffObj, xliff_context: XliffContext, current_language: str):
     obj_id = obj.id
     xliff_obj_id = xliff_context.obj_id
```

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo` & `djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po` & `djangocms_xliff-1.3.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_export.py` & `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_export.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_import.py` & `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_import.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_page_plugins.py` & `djangocms_xliff-1.3.0/djangocms_xliff/management/commands/xliff_page_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/parsers.py` & `djangocms_xliff-1.3.0/djangocms_xliff/parsers.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/renderer.py` & `djangocms_xliff-1.3.0/djangocms_xliff/renderer.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/settings.py` & `djangocms_xliff-1.3.0/djangocms_xliff/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     V1_2 = "1.2"
 
 
 XLIFF_NAMESPACES = {XliffVersion.V1_2: {"": "urn:oasis:names:tc:xliff:document:1.2"}}
 
 UNIT_ID_DELIMITER = "__"
 UNIT_ID_METADATA_ID = "METADATA"
+UNIT_ID_EXTENSION_DATA_ID = "EXTENSION"
 
 TEMPLATES_FOLDER = "djangocms_xliff"
 TEMPLATES_FOLDER_EXPORT = f"{TEMPLATES_FOLDER}/export"
 TEMPLATES_FOLDER_IMPORT = f"{TEMPLATES_FOLDER}/import"
 
 FIELDS = [import_string(field_class) for field_class in getattr(settings, "DJANGOCMS_XLIFF_FIELDS", ())]
```

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/index.html` & `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff` & `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html` & `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/success.html` & `djangocms_xliff-1.3.0/djangocms_xliff/templates/djangocms_xliff/import/success.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/types.py` & `djangocms_xliff-1.3.0/djangocms_xliff/types.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/urls.py` & `djangocms_xliff-1.3.0/djangocms_xliff/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/utils.py` & `djangocms_xliff-1.3.0/djangocms_xliff/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from django.contrib.contenttypes.models import ContentType
 from django.utils import translation
 from django.utils.timezone import localtime, now
 
 from djangocms_xliff.exceptions import XliffConfigurationError, XliffError
 from djangocms_xliff.settings import (
     TEMPLATES_FOLDER_EXPORT,
+    UNIT_ID_DELIMITER,
+    UNIT_ID_EXTENSION_DATA_ID,
     XLIFF_NAMESPACES,
     XliffVersion,
 )
 from djangocms_xliff.types import Unit, XliffObj
 
 
 def get_xliff_version(version: str) -> XliffVersion:
@@ -106,7 +108,12 @@
     from djangocms_xliff.settings import MODEL_METADATA_FIELDS
 
     obj_type = type(obj)
     try:
         return MODEL_METADATA_FIELDS[obj_type]
     except KeyError:
         raise XliffError(f"Can't find model {obj_type} in MODEL_METADATA_FIELDS config")
+
+
+def get_plugin_id_for_extension_obj(obj) -> str:
+    content_type_id = ContentType.objects.get_for_model(obj).id
+    return UNIT_ID_DELIMITER.join([UNIT_ID_EXTENSION_DATA_ID, str(content_type_id), str(obj.id)])
```

### Comparing `djangocms_xliff-1.2.0/djangocms_xliff/views.py` & `djangocms_xliff-1.3.0/djangocms_xliff/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         return self.render_template(form, current_language)
 
     def post(self, request, content_type_id: int, obj_id: int, current_language: str, *args, **kwargs):
         form = self.form_class(current_language, request.POST)
         if not form.is_valid():
             return self.render_template(form, current_language)
 
-        obj = get_obj(content_type_id, obj_id)
         try:
+            obj = get_obj(content_type_id, obj_id)
             xliff_str, file_name = export_content_as_xliff(
                 obj=obj,
                 source_language=form.cleaned_data["source_language"],
                 target_language=current_language,
             )
         except XliffError as e:
             return self.error_response(e)
```

### Comparing `djangocms_xliff-1.2.0/pyproject.toml` & `djangocms_xliff-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-xliff"
-version = "1.2.0"
+version = "1.3.0"
 description = "XLIFF Import and Export for the Django CMS"
 authors = ["Energie 360 <onlineservice@energie360.ch>"]
 maintainers = ["Energie 360 <onlineservice@energie360.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://energie360.ch"
 repository = "https://github.com/energie360/djangocms-xliff"
```

### Comparing `djangocms_xliff-1.2.0/PKG-INFO` & `djangocms_xliff-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-xliff
-Version: 1.2.0
+Version: 1.3.0
 Summary: XLIFF Import and Export for the Django CMS
 Home-page: https://energie360.ch
 License: MIT
 Keywords: django,django-cms,xliff,import,export
 Author: Energie 360
 Author-email: onlineservice@energie360.ch
 Maintainer: Energie 360
```

