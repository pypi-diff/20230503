# Comparing `tmp/envidat-utils-1.2.4.tar.gz` & `tmp/envidat-utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envidat-utils-1.2.4.tar", last modified: Wed Oct 19 16:07:12 2022, max compression
+gzip compressed data, was "envidat-utils-1.4.0.tar", last modified: Wed May  3 18:12:35 2023, max compression
```

## Comparing `envidat-utils-1.2.4.tar` & `envidat-utils-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-rw-rw-   0 root         (0) root         (0)     3429 2022-10-19 16:06:44.934644 envidat-utils-1.2.4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1063 2022-10-19 16:06:44.934644 envidat-utils-1.2.4/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)     1662 2022-10-19 16:06:44.934644 envidat-utils-1.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6663 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/api/v1.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2319 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/bibtex_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    24576 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/datacite_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    13209 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/dcat_ap_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    27406 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/dif_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    24550 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/iso_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2022-10-19 16:06:44.938644 envidat-utils-1.2.4/envidat/converters/ris_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/converters/xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     9021 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37859 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/s3/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/s3/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3288 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/envidat/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44871 2022-10-19 16:06:44.942644 envidat-utils-1.2.4/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-10-19 16:06:44.946644 envidat-utils-1.2.4/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14075 2022-10-19 16:06:44.946644 envidat-utils-1.2.4/tests/test_bucket_io.py
--rw-rw-rw-   0 root         (0) root         (0)     4088 2022-10-19 16:06:44.946644 envidat-utils-1.2.4/tests/test_bucket_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    16761 2022-10-19 16:06:44.946644 envidat-utils-1.2.4/tests/test_converters.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2022-10-19 16:06:44.946644 envidat-utils-1.2.4/tests/test_metadata.py
--rw-------   0 root         (0) root         (0)     2400 2022-10-19 16:07:12.091952 envidat-utils-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     9547 2023-05-03 13:23:42.890763 envidat-utils-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/LICENCE
+-rw-r--r--   0        0        0     1662 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/README.md
+-rw-r--r--   0        0        0       67 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-03 13:23:42.890763 envidat-utils-1.4.0/envidat/__version__.py
+-rw-r--r--   0        0        0       37 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/api/__init__.py
+-rw-r--r--   0        0        0     9122 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/api/v1.py
+-rw-r--r--   0        0        0     3161 2023-03-14 10:34:09.273358 envidat-utils-1.4.0/envidat/config/config_converters.json
+-rw-r--r--   0        0        0       69 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/__init__.py
+-rw-r--r--   0        0        0     2319 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/bibtex_converter.py
+-rw-r--r--   0        0        0    48992 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/converters/datacite_converter.py
+-rw-r--r--   0        0        0    13207 2023-05-03 16:14:00.341772 envidat-utils-1.4.0/envidat/converters/dcat_ap_converter.py
+-rw-r--r--   0        0        0    27401 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/dif_converter.py
+-rw-r--r--   0        0        0    24536 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/iso_converter.py
+-rw-r--r--   0        0        0     2622 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/ris_converter.py
+-rw-r--r--   0        0        0     1486 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/xml_converter.py
+-rw-r--r--   0        0        0       73 2023-04-04 10:16:28.915663 envidat-utils-1.4.0/envidat/doi/__init__.py
+-rw-r--r--   0        0        0     6881 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/doi/datacite_publisher.py
+-rw-r--r--   0        0        0    10657 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/doi/datacite_updater.py
+-rw-r--r--   0        0        0     8529 2023-05-03 16:14:00.341772 envidat-utils-1.4.0/envidat/metadata.py
+-rw-r--r--   0        0        0       20 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/s3/__init__.py
+-rw-r--r--   0        0        0    42309 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/envidat/s3/bucket.py
+-rw-r--r--   0        0        0     3118 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/s3/exceptions.py
+-rw-r--r--   0        0        0     6662 2023-05-03 18:09:51.816011 envidat-utils-1.4.0/envidat/utils.py
+-rw-r--r--   0        0        0     2173 2023-05-03 18:09:51.816011 envidat-utils-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    22302 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      177 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/test_api.py
+-rw-r--r--   0        0        0    14075 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/test_bucket_io.py
+-rw-r--r--   0        0        0     5101 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/tests/test_bucket_utils.py
+-rw-r--r--   0        0        0    16141 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/test_converters.py
+-rw-r--r--   0        0        0     3794 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 envidat-utils-1.4.0/PKG-INFO
```

### Comparing `envidat-utils-1.2.4/LICENCE` & `envidat-utils-1.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.2.4/README.md` & `envidat-utils-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.2.4/envidat/converters/bibtex_converter.py` & `envidat-utils-1.4.0/envidat/converters/bibtex_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.2.4/envidat/converters/dcat_ap_converter.py` & `envidat-utils-1.4.0/envidat/converters/dcat_ap_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from dateutil.parser import parse as parse_date
 from xmltodict import parse, unparse
 
 log = logging.getLogger(__name__)
 
 
 def convert_dcat_ap(metadata_records: Union[dict, list[dict]]) -> str:
-    """
-    Generate output string in DCAT-AP format.
+    """Generate output string in DCAT-AP format.
 
     Accepts a single metadata entry, or list of entries.
 
     Note:
         Converter is only valid for the metadata schema for EnviDat.
 
     Args:
@@ -320,22 +319,22 @@
 
         distribution_list += [distribution]
 
     return distribution_list
 
 
 def wrap_packages_dcat_ap_xml(dcat_xml_packages: list) -> str:
-    """
-    Add required DCAT-AP catalog XML tags for full DCAT-AP XML.
+    """Add required DCAT-AP catalog XML tags for full DCAT-AP XML.
 
     Args:
         dcat_xml_packages (list[str,dict]): All DCAT-AP formatted packages to include.
             In string XML or dictionary format.
 
-    Note: this is a required final step for producing a DCAT-AP CH format XML.
+    Note:
+        This is a required final step for producing a DCAT-AP CH format XML.
     """
     catalog_dict = OrderedDict()
 
     # header
     catalog_dict["@xmlns:dct"] = "http://purl.org/dc/terms/"
     catalog_dict["@xmlns:dc"] = "http://purl.org/dc/elements/1.1/"
     catalog_dict["@xmlns:dcat"] = "http://www.w3.org/ns/dcat#"
```

### Comparing `envidat-utils-1.2.4/envidat/converters/dif_converter.py` & `envidat-utils-1.4.0/envidat/converters/dif_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,16 +648,15 @@
             resource_restriction = resource_restriction.lower()
             if resource_restriction not in resource_restrictions:
                 resource_restrictions += [resource_restriction]
     return resource_restrictions
 
 
 def get_dif_language_code(code):
-    """
-    Translate codes to language full word.
+    """Translate codes to language full word.
 
     https://gcmd.nasa.gov/DocumentBuilder/defaultDif10/guide/data_set_language.html
 
     Options: English; Afrikaans; Arabic; Bosnia; Bulgarian; Chinese; Croation; Czech;
     Danish; Dutch; Estonian; Finnish; French; German; Hebrew; Hungarian; Indonesian;
     Italian; Japanese; Korean; Latvian; Lithuanian; Norwegian; Polish; Portuguese;
     Romanian; Russian; Slovak; Spanish; Ukrainian; Vietnamese
```

### Comparing `envidat-utils-1.2.4/envidat/converters/iso_converter.py` & `envidat-utils-1.4.0/envidat/converters/iso_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,16 +516,15 @@
     extras_dict = {}
     for extra in extras:
         extras_dict[extra.get("key")] = extra.get("value")
     return extras_dict
 
 
 def get_iso_language_code(code: str) -> str:
-    """
-    Translate to language to 3-letter code.
+    """Translate to language to 3-letter code.
 
     http://www.loc.gov/standards/iso639-2/ISO-639-2_utf-8.txt
     """
     lookup_dict = {"en": "eng", "de": "ger", "it": "ita", "fr": "fre", "ro": "roh"}
     return lookup_dict.get(code, "eng").title()
 
 
@@ -554,16 +553,15 @@
         if key_lower == tag_lower:
             tag_key = key
             break
     return data_dict.get(tag_key)
 
 
 def get_publication_date(data_dict: dict) -> str:
-    """
-    Take date of type available or the publication year.
+    """Take date of type available or the publication year.
 
     Returns:
         str: Publication date from dataset, in string format.
     """
     publication_date = ""
     try:
         dates = json.loads(data_dict.get("date", "[]"))
@@ -639,18 +637,18 @@
             "#text": function,
         }
     }
     return online_resource_dataset
 
 
 def is_url(url_str):
-    """
-    Check if string is URL.
+    """Check if string is URL.
 
     Replicates functionality of CKAN method ckan.lib.helpers.is_url()
+
     Returns:
         bool: True if argument parses as a http, https or ftp URL,
               else returns False.
     """
     parts = urlparse(url_str)
     scheme = parts.scheme
     if scheme in ["http", "https", "ftp"]:
```

### Comparing `envidat-utils-1.2.4/envidat/converters/ris_converter.py` & `envidat-utils-1.4.0/envidat/converters/ris_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.2.4/envidat/converters/xml_converter.py` & `envidat-utils-1.4.0/envidat/converters/xml_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 from envidat.api.v1 import get_metadata_json_with_resources
 
 log = logging.getLogger(__name__)
 
 
 def convert_xml(package: dict) -> str:
-    """
-    Convert EnviDat record to XML format.
+    """Convert EnviDat record to XML format.
 
     Args:
         package (dict): Package JSON from API.
 
     Returns:
         str: XML formatted string.
 
@@ -30,16 +29,15 @@
 
     except Exception as e:
         log.error("ERROR: Cannot convert EnviDat packages to XML format.")
         log.error(e)
 
 
 def convert_xml_all_resources() -> str:
-    """
-    Convert EnviDat JSON records to XML format.
+    """Convert EnviDat JSON records to XML format.
 
     Returns:
         str: XML formatted string.
 
     Note:
         Only valid for metadata schema of EnviDat.
     """
```

### Comparing `envidat-utils-1.2.4/envidat/metadata.py` & `envidat-utils-1.4.0/envidat/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import json
 import logging
 from typing import Literal, NoReturn, Union
 
 from envidat.api.v1 import (
     get_metadata_list_with_resources,
-    get_metadata_name_doi,
     get_package,
 )
 from envidat.converters.bibtex_converter import convert_bibtex
 from envidat.converters.datacite_converter import convert_datacite
 from envidat.converters.dcat_ap_converter import convert_dcat_ap
 from envidat.converters.dif_converter import convert_dif
 from envidat.converters.iso_converter import convert_iso
@@ -37,21 +36,20 @@
     def __init__(
         self,
         input_data: Union[str, dict],
         convert: Literal[
             "str", "xml", "iso", "bibtex", "dif", "datacite", "ris", "dcat-ap"
         ] = None,
     ) -> NoReturn:
-        """
-        Init the Record object.
+        """Init the Record object.
 
         Only one argument should be passed for data format.
 
         Args:
-            input_data [str, dict]: Data input, in JSON or dict form.
+            input_data ([str, dict]): Data input, in JSON or dict form.
                 Can also accept a package name to extract a record from the API.
             convert (str):
                 Options: Convert the content immediately to specified type.
                     "str", "xml", "iso", "bibtex", "dif", "datacite", "ris", "dcat-ap"
 
         """
         if isinstance(input_data, dict):
@@ -83,48 +81,44 @@
                 "iso": self.to_iso,
                 "bibtex": self.to_bibtex,
                 "dif": self.to_dif,
                 "datacite": self.to_datacite,
                 "ris": self.to_ris,
                 "dcat-ap": self.to_dcat_ap,
             }
-            if convert == "datacite":
-                name_doi_map = get_metadata_name_doi()
-                self.content = mapping[convert](name_doi_map)
-            else:
-                self.content = mapping[convert]()
+            self.content = mapping[convert]()
 
     def get_content(self):
-        """
-        Get current content of Record.
+        """Get current content of Record.
 
         Returns:
             str: Metadata record, default dict format, else converted (JSON, XML, etc).
         """
         return self.content
 
     def validate(self) -> bool:
-        """
-        Validate metadata record.
+        """Validate metadata record.
 
         Returns:
             bool: True if valid, raises error if not.
         """
         metadata_keys = [
             "author",
             "author_email",
             "creator_user_id",
             "date",
             "doi",
+            # "extras", NOT ALWAYS PRESENT
             "funding",
             "id",
             "isopen",
-            "language",
+            # "language", NOT ALWAYS PRESENT
             "license_id",
             "license_title",
+            # "license_url", NOT ALWAYS PRESENT
             "maintainer",
             "maintainer_email",
             "metadata_created",
             "metadata_modified",
             "name",
             "notes",
             "num_resources",
@@ -158,103 +152,93 @@
             log.error(f"Content is not a valid dictionary of metadata: {self.content}")
             raise ValueError("Content is not a valid dictionary of metadata.")
 
         missing_keys = list(set(metadata_keys) - set(self.content.keys()))
         if missing_keys:
             log.error(f"Metadata entry is missing fields: {missing_keys}")
             raise ValueError(
-                "Content does not have all required fields for a metadata entry."
+                "Content does not have all required fields for a metadata entry. "
+                f"Missing: {missing_keys}"
             )
 
         return True
 
     def to_json(self) -> str:
-        """
-        Convert content to JSON string.
+        """Convert content to JSON string.
 
         Returns:
             str: JSON string of metadata record.
         """
         return json.loads(self.content)
 
     def to_xml(self) -> str:
-        """
-        Convert content to XML format.
+        """Convert content to XML format.
 
         Returns:
             str: XML formatted string of metadata record.
         """
         return convert_xml(self.content)
 
     def to_iso(self) -> str:
-        """
-        Convert content to ISO format.
+        """Convert content to ISO format.
 
         Returns:
             str: ISO formatted string of metadata record.
         """
         return convert_iso(self.content)
 
     def to_ris(self) -> str:
-        """
-        Convert content to RIS format.
+        """Convert content to RIS format.
 
         Returns:
             str: RIS formatted string of metadata record.
         """
         return convert_ris(self.content)
 
     def to_bibtex(self) -> str:
-        """
-        Convert content to BibTeX format.
+        """Convert content to BibTeX format.
 
         Returns:
             str: BibTeX formatted string of metadata record.
         """
         return convert_bibtex(self.content)
 
     def to_dif(self) -> str:
-        """
-        Convert content to GCMD DIF 10.2 format.
+        """Convert content to GCMD DIF 10.2 format.
 
         Returns:
             str: GCMD DIF 10.2 formatted string of metadata record.
         """
         return convert_dif(self.content)
 
-    def to_datacite(self, name_doi_map: dict) -> str:
-        """
-        Convert content to DataCite format.
-
-        Args:
-            name_doi_map (dict): Mapping of dataset name to DOI, format name:doi.
+    def to_datacite(self) -> str:
+        """Convert content to DataCite format.
 
         Returns:
             str: DataCite formatted string of metadata record.
         """
-        return convert_datacite(self.content, name_doi_map)
+        return convert_datacite(self.content)
 
     def to_dcat_ap(self) -> str:
-        """
-        Convert content to DCAT-AP CH format.
+        """Convert content to DCAT-AP CH format.
 
         Returns:
             str: DCAT-AP CH formatted string of metadata record.
         """
         return convert_dcat_ap(self.content)
 
 
+# TODO implement error handling
 def get_all_metadata_record_list(
     convert: Literal[
         "str", "xml", "iso", "bibtex", "dif", "datacite", "ris", "dcat-ap"
     ] = None,
     content_only: bool = False,
 ) -> Union[list, str]:
-    """
-    Return all EnviDat metadata entries as Record objects.
+    """Return all EnviDat metadata entries as Record objects.
 
     Defaults to standard Record, content in json format.
 
     Args:
         convert (str): Convert the content immediately to specified type.
             Options: "str", "xml", "iso", "bibtex", "dif", "datacite", "ris", "dcat-ap"
         content_only (bool): Extract content from Record objects.
@@ -267,18 +251,14 @@
     metadata = get_metadata_list_with_resources()
 
     # DCAT-AP special case, return as single XML
     if convert == "dcat-ap":
         loaded_metadata = [Record(entry).content for entry in metadata]
         return convert_dcat_ap(loaded_metadata)
 
-    # Only get metadata:doi mapping once
-    if convert == "datacite":
-        name_doi_map = get_metadata_name_doi()
-
     record_list = []
 
     for metadata_entry in metadata:
         record = Record(metadata_entry)
 
         if convert:
             mapping = {
@@ -288,18 +268,15 @@
                 "bibtex": record.to_bibtex,
                 "dif": record.to_dif,
                 "datacite": record.to_datacite,
                 "ris": record.to_ris,
                 # dcat-ap handled separately above
             }
 
-            if convert == "datacite":
-                record.content = mapping[convert](name_doi_map)
-            else:
-                record.content = mapping[convert]()
+            record.content = mapping[convert]()
 
         if content_only:
             record_list.append(record.content)
         else:
             record_list.append(record)
 
     return record_list
```

### Comparing `envidat-utils-1.2.4/envidat/s3/bucket.py` & `envidat-utils-1.4.0/envidat/s3/bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,27 +21,25 @@
 if "DEBUG_BOTO" not in os.environ:
     logging.getLogger("boto3").setLevel(logging.CRITICAL)
     logging.getLogger("botocore").setLevel(logging.CRITICAL)
     logging.getLogger("s3transfer").setLevel(logging.CRITICAL)
 
 
 class MetaBucket:
-    """
-    Parent class of Bucket, to include classmethods in docs.
+    """Parent class of Bucket, to include classmethods in docs.
 
     Note:
         This class should not be used & instead methods should b
         called via the Bucket class.
     """
 
     def config(
         cls, access_key: str, secret_key: str, endpoint: str = None, region: str = ""
     ) -> NoReturn:
-        """
-        Config the bucket connection parameters before init.
+        """Config the bucket connection parameters before init.
 
         Args:
             access_key (str): AWS_ACCESS_KEY_ID.
             secret_key (str): AWS_SECRET_ACCESS_KEY.
             endpoint (str): Endpoint for the S3, if not AWS.
                 Defaults to None.
             region (str): AWS_REGION.
@@ -54,16 +52,15 @@
         """
         cls._AWS_ACCESS_KEY_ID = access_key
         cls._AWS_SECRET_ACCESS_KEY = secret_key
         cls._AWS_ENDPOINT = endpoint
         cls._AWS_REGION = region
 
     def get_boto3_resource() -> NoReturn:
-        """
-        Get boto3 resource object directly, for further use.
+        """Get boto3 resource object directly, for further use.
 
         Note:
             Usage: Bucket.get_boto3_resource()
         """
         log.debug("Accessing boto3 resource.")
         return boto3.resource(
             "s3",
@@ -71,16 +68,15 @@
             aws_secret_access_key=Bucket._AWS_SECRET_ACCESS_KEY,
             endpoint_url=Bucket._AWS_ENDPOINT,
             region_name=Bucket._AWS_REGION,
             config=Config(signature_version="s3v4"),
         )
 
     def get_boto3_client() -> NoReturn:
-        """
-        Get boto3 client object directly, for further use.
+        """Get boto3 client object directly, for further use.
 
         Note:
             Usage: Bucket.get_boto3_client()
         """
         log.debug("Accessing boto3 client.")
         return boto3.client(
             "s3",
@@ -88,16 +84,15 @@
             aws_secret_access_key=Bucket._AWS_SECRET_ACCESS_KEY,
             endpoint_url=Bucket._AWS_ENDPOINT,
             region_name=Bucket._AWS_REGION,
             config=Config(signature_version="s3v4"),
         )
 
     def list_buckets(cls) -> list[str]:
-        """
-        Get a list of all buckets from endpoint.
+        """Get a list of all buckets from endpoint.
 
         Note:
             Usage: Bucket.list_buckets()
         """
         resource = cls.get_boto3_resource()
         buckets = [bucket.name for bucket in resource.buckets.all()]
         log.info(f"All buckets at {Bucket._AWS_ENDPOINT}: {buckets}")
@@ -197,14 +192,16 @@
             raise exceptions.NoSuchBucket(self.bucket_name)
         elif error_code == "NoSuchKey":
             raise exceptions.NoSuchKey(key, self.bucket_name)
         elif error_code == "BucketAlreadyExists":
             raise exceptions.BucketAlreadyExists(self.bucket_name)
         elif error_code == "NoSuchCORSConfiguration":
             raise exceptions.NoSuchCORSConfiguration(self.bucket_name)
+        elif error_code == "CORSAccessDenied":
+            raise exceptions.CORSAccessDenied(self.bucket_name)
         else:
             raise exceptions.UnknownBucketException(self.bucket_name, e)
 
     def _raise_file_not_found(self, file_path: str, is_dir: bool = False) -> NoReturn:
         """Raise error if expected file not found on disk.
 
         Args:
@@ -254,14 +251,16 @@
                 ObjectLockEnabledForBucket=False,
             )
             log.debug("Bucket created successfully")
 
             if self.is_public:
                 log.info("Setting CORS config for bucket to allow all origins.")
                 self.set_cors_config(allow_all=True)
+                log.info("Setting public-read for all objects in bucket.")
+                self.set_public_read()
 
             return bucket
         except ClientError as e:
             self._handle_boto3_client_error(e)
 
     def get(
         self,
@@ -595,16 +594,15 @@
 
     def download_dir(
         self,
         s3_path: str,
         local_dir: Union[str, Path],
         file_type: str = "",
     ) -> bool:
-        """
-        Download an entire S3 path, including subpaths, to a local directory.
+        """Download an entire S3 path, including subpaths, to a local directory.
 
         Args:
             s3_path (str): The path within the bucket to download.
             local_dir (Union[str, Path]): Directory to download files into.
             file_type (str): Download files with extension only, e.g. txt.
 
         Returns:
@@ -630,16 +628,15 @@
         return status_dict
 
     def download_all(
         self,
         local_dir: Union[str, Path],
         file_type: str = "",
     ) -> bool:
-        """
-        Download an entire S3 bucket, including subpaths, to a local directory.
+        """Download an entire S3 bucket, including subpaths, to a local directory.
 
         Args:
             local_dir (Union[str, Path]): Directory to download files into.
             file_type (str): Download files with extension only, e.g. txt.
 
         Returns:
             dict: key:value pair of s3_key:download_status.
@@ -652,16 +649,15 @@
     def upload_dir(
         self,
         local_dir: Union[str, Path],
         s3_path: str = "/",
         file_type: str = "",
         contents_only: bool = False,
     ) -> bool:
-        """
-        Upload the content of a local directory to a bucket path.
+        """Upload the content of a local directory to a bucket path.
 
         Args:
             local_dir (Union[str, Path]): Directory to upload files from.
             s3_path (str, optional): The path within the bucket to upload to.
                 If omitted, the bucket root is used.
             file_type (str, optional): Upload files with extension only, e.g. txt.
             contents_only (bool): Used to copy only the directory contents to the
@@ -700,16 +696,15 @@
         return status_dict
 
     def delete_dir(
         self,
         s3_path: str,
         file_type: str = "",
     ) -> bool:
-        """
-        Delete an entire S3 path, including subpaths.
+        """Delete an entire S3 path, including subpaths.
 
         USE WITH CAUTION!
 
         Args:
             s3_path (str): The path within the bucket to delete.
             file_type (str): Delete files with extension only, e.g. txt.
 
@@ -796,16 +791,15 @@
                 log.error(f"Copying file {key} failed. Aborting deletion")
                 return False
 
         except ClientError as e:
             self._handle_boto3_client_error(e, key=key)
 
     def clean_multiparts(self) -> bool:
-        """
-        Clean up failed multipart uploads in a bucket.
+        """Clean up failed multipart uploads in a bucket.
 
         Returns:
             dict: key:value pair of s3_multipart_key:clean_status.
                 clean_status True if removed, False if failed.
         """
         status_dict = {}
         success_counter = 0
@@ -848,16 +842,15 @@
 
             return status_dict
 
         except ClientError as e:
             self._handle_boto3_client_error(e)
 
     def size(self, items_per_page: int = 1000) -> int:
-        """
-        Return the total size of a bucket, in bytes.
+        """Return the total size of a bucket, in bytes.
 
         Uses a paginator to get around 1000 file limit for listing.
 
         Args:
             items_per_page (int): Number of items to return per page.
                 Default=1000. Increase to decrease the number of transactions.
 
@@ -916,30 +909,20 @@
 
         Returns:
             bool: True if success, False is failure.
         """
         client = Bucket.get_boto3_client()
 
         try:
-            log.debug("Setting public read access policy for static website.")
-            public_policy = {
-                "Version": "2012-10-17",
-                "Statement": [
-                    {
-                        "Sid": "PublicRead",
-                        "Effect": "Allow",
-                        "Principal": "*",
-                        "Action": "s3:GetObject",
-                        "Resource": f"arn:aws:s3:::{self.bucket_name}/*",
-                    }
-                ],
-            }
-            bucket_policy = json.dumps(public_policy)
-            client.put_bucket_policy(Bucket=self.bucket_name, Policy=bucket_policy)
-            log.info("Public read access policy set for static website.")
+            # Required for static website
+            self.set_public_read()
+            log.warning(
+                "Configuring a static website requires a public-read policy "
+                "on all objects. This has been configured for you"
+            )
 
             log.debug("Setting S3 static website configuration...")
             client.put_bucket_website(
                 Bucket=self.bucket_name,
                 WebsiteConfiguration={
                     "ErrorDocument": {
                         "Key": error_file,
@@ -960,14 +943,152 @@
             return True
 
         except ClientError as e:
             self._handle_boto3_client_error(e)
 
         return False
 
+    def set_public_read(self) -> bool:
+        """Set public-read policy on all objects.
+
+        Returns:
+            bool: True if success, False is failure.
+        """
+        client = Bucket.get_boto3_client()
+
+        try:
+            log.debug("Setting public-read access policy for bucket.")
+            public_policy = {
+                "Version": "2012-10-17",
+                "Statement": [
+                    {
+                        "Sid": "PublicRead",
+                        "Effect": "Allow",
+                        "Principal": "*",
+                        "Action": "s3:GetObject",
+                        "Resource": f"arn:aws:s3:::{self.bucket_name}/*",
+                    }
+                ],
+            }
+            bucket_policy = json.dumps(public_policy)
+            client.put_bucket_policy(Bucket=self.bucket_name, Policy=bucket_policy)
+            log.info(f"Public read access policy set for bucket {self.bucket_name}.")
+
+            return True
+
+        except ClientError as e:
+            self._handle_boto3_client_error(e)
+
+        return False
+
+    def grant_user_full_access(self, canonical_user_id: str) -> dict:
+        """Set FULL_ACCESS ACL on bucket for user.
+
+        Args:
+            canonical_user_id (str): Canonical ID of user.
+                From AWS or Cloudian dashboard.
+
+        Returns:
+            dict: New ACL configuration.
+
+        Note:
+            Must have FULL_ACCESS rights to grant this permission.
+            I.e. must be bucket owner.
+        """
+        client = Bucket.get_boto3_client()
+
+        try:
+            log.debug(f"Getting current ACL policy for bucket {self.bucket_name}.")
+            existing_acl = client.get_bucket_acl(Bucket=self.bucket_name)
+            log.debug(f"Existing ACL: {existing_acl}")
+
+            owner = existing_acl["Owner"]
+            grants = existing_acl["Grants"]
+
+            grants.append(
+                {
+                    "Grantee": {
+                        "Type": "CanonicalUser",
+                        "ID": canonical_user_id,
+                    },
+                    "Permission": "FULL_CONTROL",
+                }
+            )
+            acl_policy = {
+                "Owner": owner,
+                "Grants": grants,
+            }
+            log.debug(f"New ACL: {acl_policy}")
+
+            log.debug(f"Setting FULL_ACCESS permission to user {canonical_user_id}.")
+            client.put_bucket_acl(
+                Bucket=self.bucket_name, AccessControlPolicy=acl_policy
+            )
+            log.info(
+                f"FULL_ACCESS permission granted to user {canonical_user_id} "
+                f"on bucket {self.bucket_name}."
+            )
+
+            return acl_policy
+
+        except ClientError as e:
+            self._handle_boto3_client_error(e)
+
+        return {}
+
+    def remove_user_full_access(self, canonical_user_id: str) -> dict:
+        """Remove FULL_ACCESS ACL on bucket for user.
+
+        Args:
+            canonical_user_id (str): Canonical ID of user.
+                From AWS or Cloudian dashboard.
+
+        Returns:
+            dict: New ACL configuration.
+
+        Note:
+            Must have FULL_ACCESS rights to grant this permission.
+            I.e. must be bucket owner.
+        """
+        client = Bucket.get_boto3_client()
+
+        try:
+            log.debug(f"Getting current ACL policy for bucket {self.bucket_name}.")
+            existing_acl = client.get_bucket_acl(Bucket=self.bucket_name)
+            log.debug(f"Existing ACL: {existing_acl}")
+
+            owner = existing_acl["Owner"]
+            grants = existing_acl["Grants"]
+
+            for index, grant in enumerate(grants):
+                if grant["Grantee"]["ID"] == canonical_user_id:
+                    grants.pop(index)
+
+            acl_policy = {
+                "Owner": owner,
+                "Grants": grants,
+            }
+            log.debug(f"New ACL: {acl_policy}")
+
+            log.debug(f"Setting FULL_ACCESS permission to user {canonical_user_id}.")
+            client.put_bucket_acl(
+                Bucket=self.bucket_name, AccessControlPolicy=acl_policy
+            )
+            log.info(
+                f"FULL_ACCESS permission granted to user {canonical_user_id} "
+                f"on bucket {self.bucket_name}."
+            )
+
+            return acl_policy
+
+        except ClientError as e:
+            self._handle_boto3_client_error(e)
+
+        return {}
+
     def generate_index_html(
         self, title: str, file_list: Union[list, str], index_file: str = "index.html"
     ) -> BytesIO:
         """Write index file to root of S3 bucket, with embedded S3 download links.
 
         Args:
             title (str): HTML title tag for page.
@@ -1041,14 +1162,17 @@
             response = client.get_bucket_cors(Bucket=self.bucket_name)
             cors_rules = (
                 response["CORSRules"][0] if len(response["CORSRules"]) > 0 else None
             )
             return cors_rules
 
         except ClientError as e:
+            if e.response.get("Error").get("Code") == "AccessDenied":
+                # Update error code to CORS related
+                e.response["Error"]["Code"] = "CORSAccessDenied"
             self._handle_boto3_client_error(e)
 
         return None
 
     def set_cors_config(self, origins: list = None, allow_all: bool = False) -> dict:
         """Set the CORS config for a bucket.
 
@@ -1089,10 +1213,13 @@
             )
             client.put_bucket_cors(
                 Bucket=self.bucket_name, CORSConfiguration=cors_configuration
             )
             return True
 
         except ClientError as e:
+            if e.response.Error.Code == "AccessDenied":
+                # Update error code to CORS related
+                e.response.Error.Code = "CORSAccessDenied"
             self._handle_boto3_client_error(e)
 
         return False
```

### Comparing `envidat-utils-1.2.4/envidat/s3/exceptions.py` & `envidat-utils-1.4.0/envidat/s3/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,68 +7,91 @@
 log = logging.getLogger(__name__)
 
 
 class BucketException(Exception):
     """Parent class to be inherited for consistency."""
 
     def __init__(self, message, bucket):
+        """Log error and set error message."""
         log.error(message)
         self.bucket = bucket
         self.message = f"{message}"
         super().__init__(self.message)
 
 
 class NoSuchKey(BucketException):
     """Exception for if bucket key does not exist."""
 
     def __init__(self, key, bucket):
+        """Set params and init."""
         self.key = key
         self.bucket = bucket
         self.message = f"Object not found in bucket {bucket} matching {key}"
         super().__init__(self.message, self.bucket)
 
 
 class NoSuchBucket(BucketException):
     """Exception for if bucket does not exist."""
 
     def __init__(self, bucket_name):
+        """Set params and init."""
         self.bucket = bucket_name
         self.message = f"Bucket named '{bucket_name}' does not exist!"
         super().__init__(self.message, self.bucket)
 
 
 class BucketAlreadyExists(BucketException):
     """Exception for if bucket already exists."""
 
     def __init__(self, bucket_name):
+        """Set params and init."""
         self.bucket = bucket_name
         self.message = f"Bucket named '{bucket_name}' already exists. Creation failed."
         super().__init__(self.message, self.bucket)
 
 
 class BucketAccessDenied(BucketException):
     """Exception for if bucket access is denied."""
 
     def __init__(self, bucket_name):
+        """Set params and init."""
         self.bucket = bucket_name
-        self.message = f"Unable to access bucket {self.bucket}. Does it exist?"
+        self.message = (
+            f"Unable to access bucket {self.bucket}. "
+            "Do you have permission & does it exist?"
+        )
+        super().__init__(self.message, self.bucket)
+
+
+class CORSAccessDenied(BucketException):
+    """Exception for if CORS access is denied."""
+
+    def __init__(self, bucket_name):
+        """Set params and init."""
+        self.bucket = bucket_name
+        self.message = (
+            f"Unable to access CORS config for {self.bucket}. "
+            "Are you the owner of the bucket?"
+        )
         super().__init__(self.message, self.bucket)
 
 
 class NoSuchCORSConfiguration(BucketException):
     """Exception for if the bucket does not have a CORS configuration."""
 
     def __init__(self, bucket_name):
+        """Set params and init."""
         self.bucket = bucket_name
         self.message = f"Bucket {self.bucket} does not have CORS configured."
         super().__init__(self.message, self.bucket)
 
 
 class UnknownBucketException(BucketException):
     """Exception to catch all other unknown errors."""
 
     def __init__(self, bucket_name, e: ClientError):
+        """Set params and init."""
         self.bucket = bucket_name
         error_code: str = e.response.get("Error").get("Code")
         error_message: str = e.response.get("Error").get("Message")
         self.message = f"Unknown bucket exception {error_code}: {error_message}"
         super().__init__(self.message, self.bucket)
```

### Comparing `envidat-utils-1.2.4/pyproject.toml` & `envidat-utils-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,44 @@
     { name = "Sam Woodcock", email = "samuel.woodcock@wsl.ch" },
     { name = "Rebecca Kurup Buchholz", email = "rebecca.kurup@wsl.ch" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "boto3>=1.22.12",
     "xmltodict>=0.13.0",
-    "lxml>=4.9.1",
+    "validators>=0.20.0",
+    "jsonschema>=4.17.3",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.9,<3.11"
 readme = "README.md"
 keywords = [
     "envidat",
     "s3",
     "ckan",
     "wsl",
 ]
 classifiers = [
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.10",
 ]
-version = "1.2.4"
+version = "1.4.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://www.envidat.ch"
 documentation = "https://envidat.gitlab-pages.wsl.ch/envidat-python-utils"
 repository = "https://gitlabext.wsl.ch/EnviDat/envidat-python-utils.git"
 
 [project.optional-dependencies]
 dotenv = [
-    "python-dotenv>=0.20.0",
+    "python-dotenv>=1.0.0",
 ]
 
 [tool.pdm]
 includes = [
     "envidat",
 ]
 source-includes = [
@@ -56,45 +57,69 @@
 ]
 
 [tool.pdm.version]
 from = "envidat/__version__.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "python-dotenv>=0.20.0",
+    "python-dotenv>=1.0.0",
 ]
 test = [
-    "pytest",
+    "pytest>=7.3.1",
     "moto>=3.1.9",
 ]
 doc = [
     "mkdocs>=1.1",
     "mkdocs-material>=7.3",
     "mkgendocs>=0.9.0",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.4"
+version = "1.4.0"
 version_files = [
     "pyproject.toml:version",
     "envidat/__version__.py",
 ]
 
-[tool.isort]
-profile = "black"
-atomic = true
-known_first_party = [
-    "envidat",
-]
-
 [tool.pytest.ini_options]
 addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
 
+[tool.ruff]
+target-version = "py310"
+line-length = 88
+select = [
+    "I",
+    "E",
+    "W",
+    "D",
+    "B",
+    "F",
+    "N",
+    "Q",
+]
+ignore = [
+    "N805",
+    "B008",
+]
+exclude = [
+    ".git",
+    ".ruff_cache",
+    ".vscode",
+    "__pypackages__",
+    "build",
+    "dist",
+    "secret",
+    "envidat/__version__.py",
+]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [build-system]
 requires = [
     "pdm-pep517",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `envidat-utils-1.2.4/tests/test_bucket_io.py` & `envidat-utils-1.4.0/tests/test_bucket_io.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.2.4/tests/test_bucket_utils.py` & `envidat-utils-1.4.0/tests/test_bucket_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import pytest
 from moto import mock_s3
 
 from envidat.s3.bucket import Bucket
 from envidat.s3.exceptions import NoSuchCORSConfiguration
 
 
@@ -25,14 +27,53 @@
     bucket.is_public = False
 
     response = new_bucket.meta.client.head_bucket(Bucket="testing")
     assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
 
 
 @mock_s3
+def test_set_public_read(bucket):
+    bucket.create()
+
+    success = bucket.set_public_read()
+    assert success is True
+
+    client = bucket.get_boto3_client()
+    response = client.get_bucket_policy(
+        Bucket=bucket.bucket_name,
+    )
+    assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
+
+    policy = json.loads(response["Policy"])
+    assert policy["Statement"][0]["Sid"] == "PublicRead"
+
+
+@mock_s3
+def test_grant_full_access(bucket):
+    bucket.create()
+
+    acl = bucket.grant_user_full_access("ffffffff")
+    assert acl["Grants"][1]["Grantee"]["ID"] == "ffffffff"
+
+
+@mock_s3
+def test_remove_full_access(bucket):
+    bucket.create()
+
+    acl = bucket.grant_user_full_access("ffffffff")
+    assert acl["Grants"][1]["Grantee"]["ID"] == "ffffffff"
+
+    acl = bucket.remove_user_full_access("user_that_does_not_exist")
+    assert acl["Grants"][1]["Grantee"]["ID"] == "ffffffff"
+
+    acl = bucket.remove_user_full_access("ffffffff")
+    assert len(acl["Grants"]) == 1
+
+
+@mock_s3
 def test_configure_static_website(bucket):
     bucket.create()
 
     success = bucket.configure_static_website()
     assert success is True
 
 
@@ -121,15 +162,15 @@
 
 @mock_s3
 def test_get_bucket_size(bucket, create_tempfile):
     bucket.create()
 
     with create_tempfile("txt") as temp1:
         with open(temp1.name, "w") as w:
-            for n in range(0, 57):
+            for _n in range(0, 57):
                 w.write(str(1))
                 w.write(",")
 
         status = bucket.upload_file(temp1.name, temp1.name)
         assert status is True
 
     bucket_size = bucket.size()
@@ -146,15 +187,15 @@
 
 @mock_s3
 def test_get_bucket_many_page(bucket, create_tempfile):
     bucket.create()
 
     with create_tempfile("txt") as temp1:
         with open(temp1.name, "w") as w:
-            for n in range(0, 20):
+            for _n in range(0, 20):
                 w.write(str(1))
                 w.write(",")
 
         status = bucket.upload_file(temp1.name, temp1.name)
         assert status is True
 
     bucket_size = bucket.size(items_per_page=5)
```

### Comparing `envidat-utils-1.2.4/tests/test_converters.py` & `envidat-utils-1.4.0/tests/test_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     extension: str,
     host: str = "https://www.envidat.ch",
 ) -> str:
     """Get CKAN endpoint used to export datasets in various formats.
 
     Args:
         package (dict): EnviDat package in dictionary form.
-        file_format (str): Format of file used in CKAN endpoint (example: "datacite")
+        file_format (str): Format of file used in CKAN endpoint (example: "")
         extension (str): Extension used in CKAN endpoint (example: "xml")
         host (str): Host used in CKAN endpoint (default: "https://www.envidat.ch")
 
     Returns:
         str: String of CKAN endpoint used to export datasets in format compatible with
         arguments passed.
     """
@@ -48,15 +48,15 @@
     convert_dataset, package_name, file_format, extension
 ) -> tuple[str, str]:
     """Get CKAN output and corresponding converter output for one package.
 
     Args:
         convert_dataset (function): Function used to convert dataset.
         package_name (str): Name of package.
-        file_format (str): Format of file used in CKAN endpoint (example: "datacite")
+        file_format (str): Format of file used in CKAN endpoint (example: "")
         extension (str): Extension used in CKAN endpoint (example: "xml")
 
     Returns:
         tuple (<str: ckan_output>, <str: converter_output>): CKAN output and
         corresponding converter output for one package.
     """
     package = get_package(package_name)
@@ -73,108 +73,103 @@
 def get_converters_all_packages(
     convert_dataset, file_format, extension
 ) -> tuple[list, list]:
     """Get CKAN output and corresponding converter output for all packages.
 
     Args:
         convert_dataset (function): Function used to convert dataset.
-        file_format (str): Format of file used in CKAN endpoint (example: "datacite")
+        file_format (str): Format of file used in CKAN endpoint (example: "")
         extension (str): Extension used in CKAN endpoint (example: "xml")
 
     Returns:
         tuple (<list: ckan_packages>, <list: converter_packages>):
         List of all packages converted from CKAN and list of all packages converted
         using convert_dataset function.
     """
     packages = get_metadata_list_with_resources()
     ckan_packages = []
     converter_packages = []
 
-    for package in packages:
+    for package in packages[:10]:
 
         ckan_endpoint = get_ckan_exporter_endpoint(package, file_format, extension)
         request = get_url(ckan_endpoint)
         ckan_output = request.content.decode()
+        if ckan_output.startswith("No converter"):
+            # Skip if package conversion fails in ckan
+            continue
         ckan_packages.append(ckan_output)
 
         converter_output = convert_dataset(package)
         converter_packages.append(converter_output)
 
     return ckan_packages, converter_packages
 
 
 def get_datacite_converters_one_package(
-    convert_dataset, get_name_doi, package_name, file_format, extension
+    convert_dataset, package_name, file_format, extension
 ) -> tuple[str, str]:
     """Get DacaCite formatted CKAN output and DataCite converter output for one package.
 
     Args:
         convert_dataset (function): Function used to convert dataset.
-        get_name_doi (function): Function used to get dictionary with names as keys
-            and associated DOIs as values for all packages.
         package_name (str): Name of package.
         file_format (str): Format of file used in CKAN endpoint (example: "datacite")
         extension (str): Extension used in CKAN endpoint (example: "xml")
 
     Returns:
         tuple (<str: ckan_output>, <str: converter_output>): DataCite formatted
             CKAN output and corresponding converter output for one package.
     """
     package = get_package(package_name)
 
     ckan_endpoint = get_ckan_exporter_endpoint(package, file_format, extension)
     request = get_url(ckan_endpoint)
     ckan_output = request.content.decode()
 
-    name_doi = get_name_doi()
-    converter_output = convert_dataset(package, name_doi)
+    converter_output = convert_dataset(package)
 
     return ckan_output, converter_output
 
 
 def get_datacite_converters_all_packages(
-    convert_dataset, get_name_doi, file_format, extension
+    convert_dataset, file_format, extension
 ) -> tuple[list, list]:
-    """
-    Get DacaCite formatted CKAN output and DataCite converter output for all packages.
+    """Get DacaCite CKAN output and DataCite converter output for all packages.
 
     Args:
         convert_dataset (function): Function used to convert dataset.
-        get_name_doi (function): Function used to get dictionary with names as keys
-             and associated DOIs as values for all packages.
         file_format (str): Format of file used in CKAN endpoint (example: "datacite")
         extension (str): Extension used in CKAN endpoint (example: "xml")
 
     Returns:
         tuple (<list: ckan_packages>, <list: converter_packages>):
             DataCite formatted CKAN output and corresponding converter
             output for all packages.
     """
     packages = get_metadata_list_with_resources()
     ckan_packages = []
 
-    name_doi = get_name_doi()
     converter_packages = []
 
     for package in packages:
 
         ckan_endpoint = get_ckan_exporter_endpoint(package, file_format, extension)
         request = get_url(ckan_endpoint)
         ckan_output = request.content.decode()
         ckan_packages.append(ckan_output)
 
-        converter_output = convert_dataset(package, name_doi)
+        converter_output = convert_dataset(package)
         converter_packages.append(converter_output)
 
     return ckan_packages, converter_packages
 
 
 def convert_datacite_related_identifier(ckan_output) -> str:
-    """
-    Correct typo in EnviDat API Datacite output.
+    """Correct typo in EnviDat API Datacite output.
 
     To make the DataCite converters tests pass it was necessary to simulate
     correcting the typo in the CKAN DataCite converter variable
     'related_datasets_base_url': 'https://www.envidat.ch/#/metadata//'
     (the correct url omits the last slash: 'https://www.envidat.ch/#/metadata/').
 
     Args:
@@ -238,16 +233,15 @@
             "@relatedIdentifierType": "URL",
             "@relationType": "Cites",
         }
     ]
 
 
 def convert_dif_values(ckan_output):
-    """
-    Correct typo in EnviDat API DIF output.
+    """Correct typo in EnviDat API DIF output.
 
     To make the DIF converter tests pass it was necessary to simulate correcting the
     typo in the CKAN DIF converter 'Use_Constraints' value:
     "Usage constraintes defined by the license" (the correct spelling is "constraints")
     Also simulates removing extra whitespace produced by the CKAN output for
     the 'Dataset_Creator' value.
     """
@@ -275,16 +269,15 @@
 
 
 def get_dcat_ap_converters_all_packages(
     convert_dataset,
     file_format,
     extension,
 ) -> tuple[str, str]:
-    """
-    DCAT-AP CKAN and corresponding converter XML formatted strings for all packages.
+    """DCAT-AP CKAN and corresponding converter XML formatted strings for all packages.
 
     Note: As of October 14, 2022, the expected CKAN string should be
             'https://www.envidat.ch/opendata/export/dcat-ap-ch.xml'
 
     Args:
         convert_dataset (function): Function used to convert dataset.
         file_format (str): Format of file used in CKAN endpoint (example: "dcat-ap")
@@ -326,48 +319,39 @@
     ckan_packages, converter_packages = get_converters_all_packages(
         *bibtex_converter_all_packages
     )
 
     assert ckan_packages == converter_packages
 
 
-def test_datacite_converter_one_package(datacite_converter_one_package):
-    """Test DataCite converter for one package."""
-    ckan_output, converter_output = get_datacite_converters_one_package(
-        *datacite_converter_one_package
-    )
-
-    # Simulate correct CKAN DataCite converter variable 'related_datasets_base_url'
-    ckan_output = convert_datacite_related_identifier(ckan_output)
-
-    # Convert OrderedDict to xml format
-    converted_output_xml = unparse(converter_output, pretty=True)
-
-    assert ckan_output == converted_output_xml
-
-
-def test_datacite_converters_all_packages(datacite_converter_all_packages):
-    """Test DataCite converter for all packages."""
-    ckan_packages, converter_packages = get_datacite_converters_all_packages(
-        *datacite_converter_all_packages
-    )
-
-    # Simulate correcting CKAN DataCite converter variable 'related_datasets_base_url'
-    corr_ckan_packages = []
-    for package in ckan_packages:
-        corr_package = convert_datacite_related_identifier(package)
-        corr_ckan_packages.append(corr_package)
-
-    # Convert OrderedDict packages to xml format
-    converter_packages_xml = []
-    for package in converter_packages:
-        package_xml = unparse(package, pretty=True)
-        converter_packages_xml.append(package_xml)
+# def test_datacite_converter_one_package(datacite_converter_one_package):
+#     """Test DataCite converter for one package."""
+#     ckan_output, converter_output = get_datacite_converters_one_package(
+#         *datacite_converter_one_package
+#     )
+
+#     # Simulate correct CKAN DataCite converter variable 'related_datasets_base_url'
+#     ckan_output = convert_datacite_related_identifier(ckan_output)
+
+#     assert ckan_output == converter_output
+
+
+# def test_datacite_converters_all_packages(datacite_converter_all_packages):
+#     """Test DataCite converter for all packages."""
+#     ckan_packages, converter_packages = get_datacite_converters_all_packages(
+#         *datacite_converter_all_packages
+#     )
+
+#     # Simulate correcting CKAN DataCite converter variable 'related_datasets_base_url'
+#     corr_ckan_packages = []
+#     for package in ckan_packages:
+#         corr_package = convert_datacite_related_identifier(package)
+#         corr_ckan_packages.append(corr_package)
 
-    assert corr_ckan_packages == converter_packages_xml
+#     assert corr_ckan_packages == converter_packages
 
 
 def test_dif_converters_one_package(dif_converter_one_package):
     """Test DIF converter for one package."""
     ckan_output, converter_output = get_converters_one_package(
         *dif_converter_one_package
     )
```

### Comparing `envidat-utils-1.2.4/tests/test_metadata.py` & `envidat-utils-1.4.0/tests/test_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     record = Record(example_ckan_dict)
 
     assert Counter(list(record.content.keys())) == Counter(metadata_keys)
 
 
 def test_record_init_from_api(example_ckan_json, metadata_keys):
     """Test init using call to API."""
-    record_from_api = Record(
-        "ecological-properties-of-urban-ecosystems-biodiversity-dataset-of-zurich"
-    )
+    record_from_api = Record("10-16904-3")
 
     assert Counter(list(record_from_api.content.keys())) == Counter(metadata_keys)
 
     record_from_json = Record(example_ckan_json)
     assert record_from_api.content == record_from_json.content
```

### Comparing `envidat-utils-1.2.4/PKG-INFO` & `envidat-utils-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: envidat-utils
-Version: 1.2.4
+Version: 1.4.0
 Summary: Utilities in Python for the WSL EnviDat project.
 License: MIT
 Keywords: envidat,s3,ckan,wsl
 Author-email: Sam Woodcock <samuel.woodcock@wsl.ch>,Rebecca Kurup Buchholz <rebecca.kurup@wsl.ch>
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Provides-Extra: dotenv
 Project-URL: documentation, https://envidat.gitlab-pages.wsl.ch/envidat-python-utils
 Project-URL: homepage, https://www.envidat.ch
 Project-URL: repository, https://gitlabext.wsl.ch/EnviDat/envidat-python-utils.git
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: envidat-utils Version: 1.2.4 Summary: Utilities in
+Metadata-Version: 2.1 Name: envidat-utils Version: 1.4.0 Summary: Utilities in
 Python for the WSL EnviDat project. License: MIT Keywords: envidat,s3,ckan,wsl
 Author-email: Sam Woodcock
 woodcock@wsl.ch>,Rebecca Kurup Buchholz
-kurup@wsl.ch> Requires-Python: >=3.9 Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Utilities Provides-Extra: dotenv
-Project-URL: documentation, https://envidat.gitlab-pages.wsl.ch/envidat-python-
-utils Project-URL: homepage, https://www.envidat.ch Project-URL: repository,
-https://gitlabext.wsl.ch/EnviDat/envidat-python-utils.git Description-Content-
-Type: text/markdown # EnviDat Python Utils
+kurup@wsl.ch> Requires-Python: >=3.9,<3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Utilities Provides-Extra: dotenv Project-URL: documentation, https://
+envidat.gitlab-pages.wsl.ch/envidat-python-utils Project-URL: homepage, https:/
+/www.envidat.ch Project-URL: repository, https://gitlabext.wsl.ch/EnviDat/
+envidat-python-utils.git Description-Content-Type: text/markdown # EnviDat
+Python Utils
                                      [WSL]
                    Utilities for EnviDat projects in Python.
                     [Package_version] [Downloads] [Licence]
 --- **Documentation**: https://envidat.gitlab-pages.wsl.ch/envidat-python-
 utils/ **Source Code**: https://gitlabext.wsl.ch/EnviDat/envidat-python-utils -
 -- ## PyPi Package - This package aims to speed up EnviDat python workflows -
 Contains: - Backend API function wrappers. - S3 bucket class, with configurable
```

