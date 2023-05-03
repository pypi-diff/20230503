# Comparing `tmp/docker_compose_parser-0.0.13-py3-none-any.whl.zip` & `tmp/docker_compose_parser-0.0.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3858 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 14:54 docker_compose_parser/__init__.py
--rw-r--r--  2.0 unx     6574 b- defN 23-May-02 14:54 docker_compose_parser/file_models.py
--rw-r--r--  2.0 unx      452 b- defN 23-May-02 14:54 docker_compose_parser-0.0.13.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 14:54 docker_compose_parser-0.0.13.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-02 14:54 docker_compose_parser-0.0.13.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       22 b- defN 23-May-02 14:54 docker_compose_parser-0.0.13.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      652 b- defN 23-May-02 14:54 docker_compose_parser-0.0.13.dist-info/RECORD
-7 files, 7793 bytes uncompressed, 2668 bytes compressed:  65.8%
+Zip file size: 3894 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 07:58 docker_compose_parser/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 23-May-03 07:58 docker_compose_parser/file_models.py
+-rw-r--r--  2.0 unx      452 b- defN 23-May-03 07:58 docker_compose_parser-0.0.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 07:58 docker_compose_parser-0.0.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 07:58 docker_compose_parser-0.0.14.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-May-03 07:58 docker_compose_parser-0.0.14.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      652 b- defN 23-May-03 07:58 docker_compose_parser-0.0.14.dist-info/RECORD
+7 files, 7965 bytes uncompressed, 2704 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: docker_compose_parser/__init__.py
 Comment: 
 
 Filename: docker_compose_parser/file_models.py
 Comment: 
 
-Filename: docker_compose_parser-0.0.13.dist-info/METADATA
+Filename: docker_compose_parser-0.0.14.dist-info/METADATA
 Comment: 
 
-Filename: docker_compose_parser-0.0.13.dist-info/WHEEL
+Filename: docker_compose_parser-0.0.14.dist-info/WHEEL
 Comment: 
 
-Filename: docker_compose_parser-0.0.13.dist-info/namespace_packages.txt
+Filename: docker_compose_parser-0.0.14.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: docker_compose_parser-0.0.13.dist-info/top_level.txt
+Filename: docker_compose_parser-0.0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: docker_compose_parser-0.0.13.dist-info/RECORD
+Filename: docker_compose_parser-0.0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docker_compose_parser/file_models.py

```diff
@@ -11,14 +11,15 @@
 from zero_3rdparty.iter_utils import ignore_falsy as ignore_falsy_method
 from zero_3rdparty.iter_utils import key_equal_value_to_dict
 
 from model_lib import Entity, FileFormat, parse_payload
 
 NETWORK_NAME_DEFAULT = "compose-default"
 
+
 class ComposeServiceInfo(Entity):
     class Config:
         allow_mutation = True
         allow_population_by_field_name = True
         extra = Extra.allow
 
     image: Optional[str] = None
@@ -50,20 +51,24 @@
         self,
         image: str | None = None,
         include_ports: bool = False,
         port_overrides: list[str] | None = None,
         ignore_falsy: bool = False,
         new_environment: dict | None = None,
         network_name: str = "",
+        ensure_labels: dict[str, str] | None = None,
     ) -> dict:
         image = image or self.image
         assert image, "image unspecified"
+        existing_labels = sort_keys(self.labels)
+        if ensure_labels:
+            existing_labels.update(ensure_labels)
         service_dict = {
             "image": image,
-            "labels": sort_keys(self.labels),
+            "labels": existing_labels,
             "environment": sort_keys(new_environment or self.default_env),
             "ports": port_overrides or self.default_ports if include_ports else [],
             "command": self.command,
             "volumes": self.default_volumes,
             "networks": [network_name] if network_name else [],
         }
         if ignore_falsy:
```

## Comparing `docker_compose_parser-0.0.13.dist-info/RECORD` & `docker_compose_parser-0.0.14.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 docker_compose_parser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docker_compose_parser/file_models.py,sha256=59CWnRX7HfPM3c8BpWeuDGZza_0ieZX5JWZzOCJb72w,6574
-docker_compose_parser-0.0.13.dist-info/METADATA,sha256=L1OG5RH72JXM1ufdqrr9SPL1WoQIYfOt4LEaP8Kijow,452
-docker_compose_parser-0.0.13.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-docker_compose_parser-0.0.13.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-docker_compose_parser-0.0.13.dist-info/top_level.txt,sha256=8YtdxGp1aC6902pbkHJs1V4KXzxgXjsg2A4aXP2lb8c,22
-docker_compose_parser-0.0.13.dist-info/RECORD,,
+docker_compose_parser/file_models.py,sha256=VMiaHt2vn9vxNiQvxP85Vjcyzf-30I7nlP4GjCks-Sg,6746
+docker_compose_parser-0.0.14.dist-info/METADATA,sha256=q42eF-B-8I3mXpk6D2y6RxiAMCBK0gvClLXmMe40Www,452
+docker_compose_parser-0.0.14.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+docker_compose_parser-0.0.14.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+docker_compose_parser-0.0.14.dist-info/top_level.txt,sha256=8YtdxGp1aC6902pbkHJs1V4KXzxgXjsg2A4aXP2lb8c,22
+docker_compose_parser-0.0.14.dist-info/RECORD,,
```

