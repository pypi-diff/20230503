# Comparing `tmp/pants_py_deploy-0.0.13-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,14 @@
-Zip file size: 12803 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 13:35 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4308 b- defN 23-May-02 13:35 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7744 b- defN 23-May-02 13:35 pants_py_deploy/compose_file_models.py
--rw-r--r--  2.0 unx     7078 b- defN 23-May-02 13:35 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx      261 b- defN 23-May-02 13:35 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     2222 b- defN 23-May-02 13:35 pants_py_deploy/models.py
--rw-r--r--  2.0 unx     5293 b- defN 23-May-02 13:35 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx     2367 b- defN 23-May-02 13:35 pants_py_deploy/ports.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-02 13:35 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2150 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1202 b- defN 23-May-02 13:35 pants_py_deploy-0.0.13.dist-info/RECORD
-14 files, 33017 bytes uncompressed, 10777 bytes compressed:  67.4%
+Zip file size: 10523 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 07:58 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4603 b- defN 23-May-03 07:58 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-03 07:58 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx      444 b- defN 23-May-03 07:58 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     3415 b- defN 23-May-03 07:58 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx     8961 b- defN 23-May-03 07:58 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      370 b- defN 23-May-03 07:58 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2163 b- defN 23-May-03 07:58 pants_py_deploy-0.0.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 07:58 pants_py_deploy-0.0.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 07:58 pants_py_deploy-0.0.14.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-03 07:58 pants_py_deploy-0.0.14.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1026 b- defN 23-May-03 07:58 pants_py_deploy-0.0.14.dist-info/RECORD
+12 files, 28174 bytes uncompressed, 8773 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,43 +1,37 @@
 Filename: pants_py_deploy/__init__.py
 Comment: 
 
 Filename: pants_py_deploy/compose_file.py
 Comment: 
 
-Filename: pants_py_deploy/compose_file_models.py
-Comment: 
-
 Filename: pants_py_deploy/export_env.py
 Comment: 
 
 Filename: pants_py_deploy/fields.py
 Comment: 
 
 Filename: pants_py_deploy/models.py
 Comment: 
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
-Filename: pants_py_deploy/ports.py
-Comment: 
-
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.13.dist-info/METADATA
+Filename: pants_py_deploy-0.0.14.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.13.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.14.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.13.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.14.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.13.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.13.dist-info/RECORD
+Filename: pants_py_deploy-0.0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/compose_file.py

```diff
@@ -1,117 +1,127 @@
 from collections import ChainMap
 from itertools import chain
 from typing import Iterable
 
-from pants.engine.fs import FileContent
-from pants_py_deploy.compose_file_models import (
+from compose_chart_export.ports import PrefixPort
+from docker_compose_parser.file_models import (
     ComposeServiceInfo,
     export_compose_dict_from_services,
     iter_compose_info,
 )
+from pants.engine.fs import FileContent
 from pants_py_deploy.fields import COMPOSE_NETWORK_NAME
 from pants_py_deploy.models import ComposeFiles, ComposeService, FileEnvVars
-from pants_py_deploy.ports import PrefixPort
 from zero_3rdparty.str_utils import ensure_suffix
 
 from model_lib import FileFormat, dump, parse_payload
 
 
 def create_compose_files(
-    new_paths: set[str], env_vars: FileEnvVars, compose_files: ComposeFiles
+    new_paths: set[str], compose_files: ComposeFiles
 ) -> list[FileContent]:
     new_files = []
     path_to_service = compose_files.paths_managed
     for path in new_paths:
-        service_dicts = _as_service_dicts(path_to_service[path], env_vars)
-        compose_full_dict = export_compose_dict_from_services(
-            service_dicts, network_name=COMPOSE_NETWORK_NAME
-        )
-        compose_yaml = dump(compose_full_dict, FileFormat.yaml)
+        compose_services = path_to_service[path]
+        compose_yaml = as_new_compose_yaml(compose_services)
         new_files.append(create_compose_file(path, compose_yaml))
     return new_files
 
 
-def _as_service_dicts(
-    compose_services: Iterable[ComposeService], env_vars: FileEnvVars
-) -> dict[str, dict]:
-    return {
-        service.name: _as_service_dict(service, env_vars)
-        for service in compose_services
-    }
+def as_new_compose_yaml(compose_services: Iterable[ComposeService]) -> str:
+    service_dicts = _as_service_dicts(compose_services)
+    compose_full_dict = export_compose_dict_from_services(
+        service_dicts, network_name=COMPOSE_NETWORK_NAME
+    )
+    compose_yaml = dump(compose_full_dict, FileFormat.yaml)
+    return compose_yaml
+
+
+def _as_service_dicts(compose_services: Iterable[ComposeService]) -> dict[str, dict]:
+    return {service.name: _as_service_dict(service) for service in compose_services}
 
 
-def _as_service_dict(compose_service: ComposeService, env_vars: FileEnvVars) -> dict:
-    dependencies = compose_service.dependency_paths
-    path_env_vars = _file_env_vars(env_vars, dependencies)
-    ports = _compose_ports(env_vars, dependencies)
+def _as_service_dict(compose_service: ComposeService) -> dict:
     service_info = ComposeServiceInfo(
         image=compose_service.image_url,
-        default_env=path_env_vars,
-        default_ports=ports,
+        default_env={**compose_service.env_vars},
+        default_ports=file_compose_ports(compose_service.ports),
         default_volumes=[],
         command=[],
+        labels={"chart_name": compose_service.name}
+        if compose_service.chart_path
+        else {},
     )
     return service_info.as_service_dict(
         ignore_falsy=True, include_ports=True, network_name=COMPOSE_NETWORK_NAME
     )
 
 
 def modify_existing_compose(
     compose_files: ComposeFiles,
     digest_contents: Iterable[FileContent],
-    env_vars: FileEnvVars,
 ) -> list[FileContent]:
     new_contents = []
     for file_content in digest_contents:
         path = file_content.path
         if not compose_files.is_managed(path):
             new_contents.append(file_content)
             continue
-        existing_full = parse_payload(file_content.content, FileFormat.yaml)
-        existing_infos = dict(iter_compose_info(file_content.content))
-        managed_service_dicts = _as_service_dicts(
-            compose_files.paths_managed[path], env_vars
-        )
-        for service_name, service_dict in managed_service_dicts.items():
-            if existing_info := existing_infos.get(service_name):
-                new_dictionary = existing_info.as_service_dict(
-                    image=service_dict["image"],
-                    include_ports=True,
-                    port_overrides=service_dict.get("ports", []),
-                    ignore_falsy=True,
-                    new_environment=service_dict.get("environment", {}),
-                    network_name=COMPOSE_NETWORK_NAME,
-                )
-                existing_full["services"][service_name] = new_dictionary
-            else:
-                existing_full["services"][service_name] = service_dict
-        compose_yaml = dump(existing_full, FileFormat.yaml)
+        compose_services = compose_files.paths_managed[path]
+        compose_yaml = as_compose_yaml(compose_services, file_content)
         new_contents.append(create_compose_file(path, compose_yaml))
     return new_contents
 
 
+def as_compose_yaml(
+    compose_services: Iterable[ComposeService], file_content: FileContent
+) -> str:
+    existing_full = parse_payload(file_content.content, FileFormat.yaml)
+    existing_infos = dict(iter_compose_info(file_content.content))
+    managed_service_dicts = _as_service_dicts(compose_services)
+    for service_name, service_dict in managed_service_dicts.items():
+        if existing_info := existing_infos.get(service_name):
+            new_dictionary = existing_info.as_service_dict(
+                image=service_dict["image"],
+                include_ports=True,
+                port_overrides=service_dict.get("ports", []),
+                ignore_falsy=True,
+                new_environment=service_dict.get("environment", {}),
+                network_name=COMPOSE_NETWORK_NAME,
+                ensure_labels=service_dict.get("labels", {}),
+            )
+            existing_full["services"][service_name] = new_dictionary
+        else:
+            existing_full["services"][service_name] = service_dict
+    compose_yaml = dump(existing_full, FileFormat.yaml)
+    return compose_yaml
+
+
 def create_compose_file(path: str, content: str) -> FileContent:
     return FileContent(
         path=ensure_suffix(path, "/docker-compose.yaml"),
         content=content.encode("utf-8"),
     )
 
 
-def _file_env_vars(
-    env_vars: FileEnvVars, dependencies: Iterable[str]
-) -> dict[str, str]:
+def file_env_vars(env_vars: FileEnvVars, dependencies: Iterable[str]) -> dict[str, str]:
     env_vars_paths = set(dependencies) & env_vars.file_env_vars.keys()
     file_env_vars = ChainMap(
         *[
             {env.name: env.default for env in env_vars.file_env_vars[env_file]}
             for env_file in env_vars_paths
         ]
     )
     return {**file_env_vars}
 
 
-def _compose_ports(env_vars: FileEnvVars, dependencies: Iterable[str]) -> list[str]:
-    file_ports: Iterable[PrefixPort] = chain.from_iterable(
+def file_compose_ports(ports: Iterable[PrefixPort]) -> list[str]:
+    return [f"{port.port}:{port.port}" for port in ports]
+
+
+def combined_ports(
+    env_vars: FileEnvVars, dependencies: Iterable[str]
+) -> Iterable[PrefixPort]:
+    return chain.from_iterable(
         env_vars.file_port_info.get(port_file, []) for port_file in dependencies
     )
-    return [f"{port.port}:{port.port}" for port in file_ports]
```

## pants_py_deploy/export_env.py

```diff
@@ -2,15 +2,15 @@
 
 import ast
 import dataclasses
 import logging
 import typing
 from pydoc import locate
 
-from pants_py_deploy.ports import PrefixPort
+from compose_chart_export.ports import PrefixPort
 
 logger = logging.getLogger(__name__)
 NodeType = typing.TypeVar("NodeType", bound=ast.AST)
 REQUIRED = "__REQUIRED__"
 
 
 @dataclasses.dataclass
```

## pants_py_deploy/fields.py

```diff
@@ -1,10 +1,16 @@
-from pants.engine.target import BoolField
+from pants.engine.target import BoolField, StringField
 
 
 class ComposeEnabledField(BoolField):
     alias = "compose_enabled"
     default = False
     help = "If set to true, it will create a docker-compose file in the same directory"
 
 
+class ComposeChartField(StringField):
+    alias = "compose_chart"
+    default = ""
+    help = "If set to a path, it will use the docker-compose file to export a chart"
+
+
 COMPOSE_NETWORK_NAME = "pants-default"
```

## pants_py_deploy/models.py

```diff
@@ -1,16 +1,18 @@
 from collections import defaultdict
 from dataclasses import dataclass
+from itertools import chain
 from typing import Iterable
 
+from compose_chart_export.ports import PrefixPort
 from pants.backend.docker.target_types import DockerImageTarget
 from pants.engine.collection import Collection
+from pants.engine.fs import DigestContents
 from pants.util.frozendict import FrozenDict
 from pants.util.ordered_set import FrozenOrderedSet
-from pants_py_deploy.ports import PrefixPort
 
 
 @dataclass(frozen=True)
 class EnvVar:
     name: str
     default: str
 
@@ -48,15 +50,18 @@
 
 
 @dataclass(frozen=True)
 class ComposeService:
     path: str
     name: str
     dependency_paths: FrozenOrderedSet[str]
+    env_vars: FrozenDict[str, str]
+    ports: Collection[PrefixPort]
     image_tag: str
+    chart_path: str = ""
 
     @property
     def image_url(self) -> str:
         return f"{self.name}:{self.image_tag}"
 
 
 @dataclass(frozen=True)
@@ -72,11 +77,49 @@
             for path, services in path_to_service.items()
         }
         object.__setattr__(self, "paths_managed", FrozenDict(paths_managed))
 
     def is_managed(self, path: str) -> bool:
         return path in self.paths_managed
 
+    @property
+    def helm_charts(self) -> dict[str, ComposeService]:
+        return {
+            path: service
+            for service in chain.from_iterable(self.paths_managed.values())
+            if (path := service.chart_path)
+        }
+
 
 @dataclass(frozen=True)
 class ComposeServiceRequest:
     image: DockerImageTarget
+
+
+@dataclass(frozen=True)
+class HelmChartsExported:
+    # chart paths always is to the Chart.yaml file
+    charts: FrozenDict[str, DigestContents]
+
+    def __init__(self, charts: dict[str, DigestContents]):
+        """Expecting FileContent to have the full relative path.
+
+        Keys are path to the chart itself
+        """
+        object.__setattr__(self, "charts", FrozenDict(charts))
+
+    @property
+    def full_digest(self) -> DigestContents:
+        return DigestContents(chain.from_iterable(self.charts.values()))
+
+
+@dataclass(frozen=True)
+class ComposeExportChartRequest:
+    # chart paths always is to the Chart.yaml file
+    service: ComposeService
+    chart_path: str
+
+
+@dataclass(frozen=True)
+class ComposeExportChart:
+    chart_path: str
+    files: DigestContents
```

## pants_py_deploy/plugin.py

```diff
@@ -1,80 +1,155 @@
-from dataclasses import dataclass
-from pathlib import PurePath
+from itertools import chain
+from pathlib import Path, PurePath
+from tempfile import TemporaryDirectory
+from typing import Optional
 
+from compose_chart_export.compose_export import export_from_compose
+from compose_chart_export.ports import PrefixPort
 from pants.backend.docker.target_types import DockerImageTagsField, DockerImageTarget
 from pants.backend.python.target_types import PythonSourceField
 from pants.core.goals.fix import FixFilesRequest, FixResult, Partitions
 from pants.core.util_rules.source_files import SourceFiles, SourceFilesRequest
+from pants.engine.collection import Collection
 from pants.engine.fs import (
     CreateDigest,
     Digest,
     DigestContents,
     DigestSubset,
+    FileContent,
     PathGlobs,
 )
 from pants.engine.internals.native_engine import Snapshot
 from pants.engine.internals.selectors import Get, MultiGet
 from pants.engine.rules import collect_rules, rule
-from pants.engine.target import (
-    AllTargets,
-    FieldSet,
-    TransitiveTargets,
-    TransitiveTargetsRequest,
-)
+from pants.engine.target import AllTargets, TransitiveTargets, TransitiveTargetsRequest
+from pants.util.frozendict import FrozenDict
 from pants.util.meta import classproperty
 from pants.util.ordered_set import FrozenOrderedSet
-from pants_py_deploy.compose_file import create_compose_files, modify_existing_compose
+from pants_py_deploy.compose_file import (
+    as_compose_yaml,
+    as_new_compose_yaml,
+    combined_ports,
+    create_compose_files,
+    file_env_vars,
+    modify_existing_compose,
+)
 from pants_py_deploy.export_env import read_env_and_ports
-from pants_py_deploy.fields import ComposeEnabledField
+from pants_py_deploy.fields import ComposeChartField, ComposeEnabledField
 from pants_py_deploy.models import (
+    ComposeExportChart,
+    ComposeExportChartRequest,
     ComposeFiles,
     ComposeService,
     ComposeServiceRequest,
     EnvVar,
     FileEnvVars,
+    HelmChartsExported,
 )
+from zero_3rdparty.file_utils import iter_paths_and_relative
 from zero_3rdparty.str_utils import ensure_suffix
 
 
-@dataclass(frozen=True)
-class DockerComposeFieldSet(FieldSet):
-    required_fields = (PythonSourceField,)
-
-    source: PythonSourceField
-
-
-#
-#
 class DockerComposeFileFixer(FixFilesRequest):
-    """Ensures all non-comment lines only consist of the word 'brick'."""
-
-    field_set_type = DockerComposeFieldSet
-
     @classproperty
     def tool_name(cls) -> str:
         return "docker-compose"
 
     @classproperty
     def tool_id(cls) -> str:
         return "dockercompose"
 
 
+class HelmChartFileFixer(FixFilesRequest):
+    @classproperty
+    def tool_name(cls) -> str:
+        return "helm-chart"
+
+    @classproperty
+    def tool_id(cls) -> str:
+        return "helmchart"
+
+
+@rule
+async def export_helm_charts(compose_files: ComposeFiles) -> HelmChartsExported:
+    requests = []
+    for chart_path, service in compose_files.helm_charts.items():
+        requests.append(
+            Get(ComposeExportChart, ComposeExportChartRequest(service, chart_path))
+        )
+    exports = await MultiGet(requests)
+    charts = {export.chart_path: export.files for export in exports}
+    return HelmChartsExported(charts)
+
+
+@rule
+async def export_helm_chart(request: ComposeExportChartRequest) -> ComposeExportChart:
+    chart_yaml_path = request.chart_path
+    chart_path = PurePath(chart_yaml_path).parent
+    chart_digest: Optional[DigestContents] = None
+
+    def store_digest(exported_chart_path: Path):
+        nonlocal chart_digest
+        file_contents = []
+        for path, relative_path in iter_paths_and_relative(
+            exported_chart_path, "*", rglob=True
+        ):
+            if path.is_dir():
+                continue
+            file_contents.append(
+                FileContent(
+                    path=f"{chart_path}/{relative_path}", content=path.read_bytes()
+                )
+            )
+        chart_digest = DigestContents(file_contents)
+
+    service = request.service
+    with TemporaryDirectory() as tmpdir:
+        digest = await Get(DigestContents, PathGlobs([service.path]))
+        if digest:
+            compose_yaml = as_compose_yaml([service], digest[0])
+        else:
+            compose_yaml = as_new_compose_yaml([service])
+        docker_compose_path = Path(tmpdir) / "docker-compose.yaml"
+        docker_compose_path.write_text(compose_yaml)
+        export_from_compose(
+            compose_path=docker_compose_path,
+            chart_version=service.image_tag,
+            chart_name=service.name,
+            image_url=service.image_url,
+            on_exported=store_digest,
+        )
+    assert chart_digest
+    return ComposeExportChart(chart_path=chart_yaml_path, files=chart_digest)
+
+
 @rule
 async def docker_compose_partition(
     request: DockerComposeFileFixer.PartitionRequest, compose_files: ComposeFiles
 ) -> Partitions:
-    managed_files = [path for path in compose_files.paths_managed.keys()]
+    managed_files = list(compose_files.paths_managed.keys())
     input_digest = [
         file for file in request.files if PurePath(file).stem == "docker-compose"
     ]
     return Partitions.single_partition(set(input_digest + managed_files))
 
 
 @rule
+async def helm_chart_partition(
+    request: HelmChartFileFixer.PartitionRequest,
+    new_exported_charts: HelmChartsExported,
+) -> Partitions:
+    managed_chart_files = list(
+        file.path for file in chain.from_iterable(new_exported_charts.charts.values())
+    )
+
+    return Partitions.single_partition(managed_chart_files)
+
+
+@rule
 async def find_env_vars(targets: AllTargets) -> FileEnvVars:
     # don't understand why targets: Targets doesn't work
     sources = await Get(
         SourceFiles,
         SourceFilesRequest(
             [
                 target[PythonSourceField]
@@ -100,28 +175,40 @@
     }
     file_ports = {file: ports for file, (_, ports) in file_env_vars_ports.items()}
     return FileEnvVars(file_env_vars, file_ports)
 
 
 @rule
 async def resolve_compose_service(
-    service_request: ComposeServiceRequest,
+    service_request: ComposeServiceRequest, all_env_vars: FileEnvVars
 ) -> ComposeService:
     image = service_request.image
     transitive_targets = await Get(
         TransitiveTargets, TransitiveTargetsRequest([image.address])
     )
-    path = image.address.spec_path
+    spec_path = image.address.spec_path
     dependencies = [str(dep.address) for dep in transitive_targets.dependencies]
     image_tag = image[DockerImageTagsField].value[0]
+    compose_chart_relative_path = service_request.image.get(
+        ComposeChartField, default_raw_value=""
+    ).value
+    if compose_chart_relative_path:
+        chart_path = ensure_suffix(
+            f"{spec_path}/{compose_chart_relative_path}", "/Chart.yaml"
+        )
+    else:
+        chart_path = ""
     return ComposeService(
-        path=ensure_suffix(path, "/docker-compose.yaml"),
+        path=ensure_suffix(spec_path, "/docker-compose.yaml"),
         name=image.address.target_name,
         dependency_paths=FrozenOrderedSet(dependencies),
+        env_vars=FrozenDict(file_env_vars(all_env_vars, dependencies)),
+        ports=Collection[PrefixPort](combined_ports(all_env_vars, dependencies)),
         image_tag=image_tag,
+        chart_path=chart_path,
     )
 
 
 @rule
 async def find_managed_compose_files_with_sources(targets: AllTargets) -> ComposeFiles:
     compose_targets: list[DockerImageTarget] = [
         target
@@ -130,35 +217,55 @@
     ]
     compose_services = await MultiGet(
         [
             Get(ComposeService, ComposeServiceRequest(image=target))
             for target in compose_targets
         ]
     )
-    return ComposeFiles(compose_services)
+    return ComposeFiles(
+        compose_services,
+    )
 
 
 @rule
 async def fix_docker_compose(
     request: DockerComposeFileFixer.Batch,
-    env_vars: FileEnvVars,
     compose_files: ComposeFiles,
 ) -> FixResult:
     input_snapshot = request.snapshot
     digest_contents = await Get(DigestContents, Digest, input_snapshot.digest)
-    updated_contents = modify_existing_compose(compose_files, digest_contents, env_vars)
+    updated_contents = modify_existing_compose(compose_files, digest_contents)
     updates_paths = {file_content.path for file_content in updated_contents}
     new_files = compose_files.paths_managed.keys() - updates_paths
-    new_contents = create_compose_files(new_files, env_vars, compose_files)
+    new_contents = create_compose_files(new_files, compose_files)
     all_contents = updated_contents + new_contents
     output_snapshot = await Get(Snapshot, CreateDigest(all_contents))
     return FixResult(
         input=input_snapshot,
         output=output_snapshot,
         stdout="",
         stderr="",
         tool_name=DockerComposeFileFixer.tool_name,
     )
 
 
+@rule
+async def fix_helm_charts(
+    request: HelmChartFileFixer.Batch, charts: HelmChartsExported
+) -> FixResult:
+    new_contents = await Get(Snapshot, CreateDigest(charts.full_digest))
+    return FixResult(
+        input=request.snapshot,
+        output=new_contents,
+        stderr="",
+        stdout="",
+        tool_name=HelmChartFileFixer.tool_name,
+    )
+
+
 def rules():
-    return [*collect_rules(), *DockerComposeFileFixer.rules(), find_env_vars]
+    return [
+        *collect_rules(),
+        *DockerComposeFileFixer.rules(),
+        *HelmChartFileFixer.rules(),
+        find_env_vars,
+    ]
```

## pants_py_deploy/register.py

```diff
@@ -1,10 +1,11 @@
 from pants.backend.docker.target_types import DockerImageTarget
 from pants_py_deploy import plugin
-from pants_py_deploy.fields import ComposeEnabledField
+from pants_py_deploy.fields import ComposeChartField, ComposeEnabledField
 
 
 def rules():
     return [
         *plugin.rules(),
         DockerImageTarget.register_plugin_field(ComposeEnabledField),
+        DockerImageTarget.register_plugin_field(ComposeChartField),
     ]
```

## Comparing `pants_py_deploy-0.0.13.dist-info/METADATA` & `pants_py_deploy-0.0.14.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.13
+Version: 0.0.14
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: model-lib (==0.0.12)
+Requires-Dist: docker-compose-parser (==0.0.13)
+Requires-Dist: model-lib (==0.0.13)
 Requires-Dist: pantsbuild.pants (<2.17,>=2.16.0a0)
-Requires-Dist: pydantic (==1.10.2)
 
 # Pants py_deploy plugin
 - Purpose: Make it easy to maintain docker-compose files and helm-charts across projects
 - Goals
   - Support updating services.{service_name}.
     - `environment` by scanning source code
     - `ports` by scanning source code
```

## Comparing `pants_py_deploy-0.0.13.dist-info/RECORD` & `pants_py_deploy-0.0.14.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pants_py_deploy/compose_file.py,sha256=j3m1t5FSOHLs0dYIVzzsQJEt0ManT4vt9Eg7aIGMsVs,4308
-pants_py_deploy/compose_file_models.py,sha256=KpkmWQcThF7XsRE1pC69ljDrkIi4Jk3P6r4wRvnEQT8,7744
-pants_py_deploy/export_env.py,sha256=yCurh7x07tiMi-MoEcq3WUobrTJkGaiW5b6d55jLv3Q,7078
-pants_py_deploy/fields.py,sha256=gKrdqf6kHaosNHG93syWFDEtVH8cWpO4PaeOWKp1QyA,261
-pants_py_deploy/models.py,sha256=e_2s6RFg5oZrYzKVgfKgsXb6ien6y_nYK4AuJ0QlqWo,2222
-pants_py_deploy/plugin.py,sha256=Y8J_FWxewG_4hFrvPjD4K0mBEG3ndQ8M0uC3B-bQdQw,5293
-pants_py_deploy/ports.py,sha256=b4Kxxnjk9uedTrlJ1cpZmWMuMOTaHhsOuIbcJGbX3YU,2367
-pants_py_deploy/register.py,sha256=aVXxmofChwsPDqQU_lEUp608IUlwkjwbrp7Y1hO71nk,283
-pants_py_deploy-0.0.13.dist-info/METADATA,sha256=6eNUKlj4RDT0W7OA5T6UZTsJ7XRXP2DBI6L839EDB7A,2150
-pants_py_deploy-0.0.13.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.13.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.13.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.13.dist-info/RECORD,,
+pants_py_deploy/compose_file.py,sha256=__uZE1ah8UzU3CUFnH7iYbclWSnzxQ6hAX3srt9rkWM,4603
+pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
+pants_py_deploy/fields.py,sha256=r-u3vf62YNCSVKuqEWxaBY8RBslvkW28wzY59tyW1mU,444
+pants_py_deploy/models.py,sha256=01FBjZNjLqyOA4SYb87CrIpl3AYGPqY7J5LXZc7bhXs,3415
+pants_py_deploy/plugin.py,sha256=h7hpZuh3klYE2NxLsohpTXQJUDO0S9AQ7fY1EksjLX0,8961
+pants_py_deploy/register.py,sha256=l86gNKZ2OqRaUjBjRRr46vYIvoZeTyBfZaghHYTXEcc,370
+pants_py_deploy-0.0.14.dist-info/METADATA,sha256=tTs8B_KsBIZYt_kzUdMyCSsnVULMROIanFmFIzgTFQo,2163
+pants_py_deploy-0.0.14.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.14.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.14.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.14.dist-info/RECORD,,
```

