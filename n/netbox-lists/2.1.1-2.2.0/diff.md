# Comparing `tmp/netbox-lists-2.1.1.tar.gz` & `tmp/netbox-lists-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-lists-2.1.1.tar", max compression
+gzip compressed data, was "netbox-lists-2.2.0.tar", max compression
```

## Comparing `netbox-lists-2.1.1.tar` & `netbox-lists-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11358 2022-04-25 19:25:46.911225 netbox-lists-2.1.1/LICENSE
--rw-r--r--   0        0        0      641 2022-04-25 19:25:46.911225 netbox-lists-2.1.1/netbox_lists/__init__.py
--rw-r--r--   0        0        0        0 2022-04-25 19:25:46.911225 netbox-lists-2.1.1/netbox_lists/api/__init__.py
--rw-r--r--   0        0        0      113 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/constants.py
--rw-r--r--   0        0        0     1942 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/filtersets.py
--rw-r--r--   0        0        0      547 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/renderers.py
--rw-r--r--   0        0        0     1258 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/urls.py
--rw-r--r--   0        0        0     6454 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/utils.py
--rw-r--r--   0        0        0    20294 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/api/views.py
--rw-r--r--   0        0        0        0 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/netbox_lists/py.typed
--rw-r--r--   0        0        0      997 2022-04-25 19:25:46.915225 netbox-lists-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      610 2022-04-25 19:26:12.827747 netbox-lists-2.1.1/setup.py
--rw-r--r--   0        0        0      434 2022-04-25 19:26:12.828101 netbox-lists-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2174 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/constants.py
+-rw-r--r--   0        0        0     1942 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/filtersets.py
+-rw-r--r--   0        0        0      547 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/renderers.py
+-rw-r--r--   0        0        0     2009 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/serializers.py
+-rw-r--r--   0        0        0     1258 2023-04-30 05:28:18.803210 netbox-lists-2.2.0/netbox_lists/api/urls.py
+-rw-r--r--   0        0        0     6649 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/utils.py
+-rw-r--r--   0        0        0    21353 2023-05-02 22:13:55.566068 netbox-lists-2.2.0/netbox_lists/api/views.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/py.typed
+-rw-r--r--   0        0        0      997 2023-05-03 00:01:36.986215 netbox-lists-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 netbox-lists-2.2.0/setup.py
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 netbox-lists-2.2.0/PKG-INFO
```

### Comparing `netbox-lists-2.1.1/LICENSE` & `netbox-lists-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.1.1/netbox_lists/api/filtersets.py` & `netbox-lists-2.2.0/netbox_lists/api/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.1.1/netbox_lists/api/renderers.py` & `netbox-lists-2.2.0/netbox_lists/api/renderers.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.1.1/netbox_lists/api/urls.py` & `netbox-lists-2.2.0/netbox_lists/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.1.1/netbox_lists/api/utils.py` & `netbox-lists-2.2.0/netbox_lists/api/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 from django_filters.utils import translate_validation
 from netaddr import cidr_merge, IPNetwork, iprange_to_cidrs
 from rest_framework.exceptions import ValidationError
 from rest_framework.request import Request
 from rest_framework.response import Response
 from taggit.managers import _TaggableManager
 
-from .constants import (
-    AS_CIDR_PARAM_NAME,
-    FAMILY_PARAM_NAME,
-    LOOKUP_SEP,
-    SUMMARIZE_PARAM_NAME,
-)
+from .constants import AS_CIDR_PARAM_NAME, FAMILY_PARAM_NAME, SUMMARIZE_PARAM_NAME
 
 
 def make_ip_list_response(
     networks: Iterable[IPNetwork],
     summarize: bool,
     use_net_ip: bool = False,
 ) -> Response:
@@ -191,22 +186,33 @@
         return {str(k): _json_rep(v) for k, v in obj.items()}
     elif isinstance(obj, _TaggableManager):
         return list(obj.slugs())
     else:
         return str(obj)
 
 
-def _get_attr_r(attrs: List[str], obj: Any) -> Any:
-    if len(attrs) == 0 or obj is None:
-        return _json_rep(obj)
+def get_attr(attrs: Iterable[str], obj: Any) -> Any:
+    for a in attrs:
+        if obj is None:
+            return None
+        elif isinstance(obj, dict):
+            obj = obj.get(a)
+        else:
+            obj = getattr(obj, a, None)
+    return obj
+
 
-    return _get_attr_r(attrs[1:], getattr(obj, attrs[0]))
+def get_attr_str(attrs: Iterable[str], obj: Any) -> str:
+    val = get_attr(attrs, obj)
+    if val is None:
+        return ""
+    return str(val)
 
 
-def get_attr_r(attr: str, obj: Any) -> Any:
-    return _get_attr_r(attr.split(LOOKUP_SEP), obj)
+def get_attr_json(attrs: Iterable[str], obj: Any) -> Any:
+    return _json_rep(get_attr(attrs, obj))
 
 
 def filter_queryset(filterset: FilterSet) -> QuerySet:
     if not filterset.is_valid():
         raise translate_validation(filterset.errors)
     return filterset.qs
```

### Comparing `netbox-lists-2.1.1/netbox_lists/api/views.py` & `netbox-lists-2.2.0/netbox_lists/api/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,40 +15,42 @@
     AggregateFilterSet,
     IPAddressFilterSet,
     IPRangeFilterSet,
     ServiceFilterSet,
 )
 from ipam.models import Aggregate, IPAddress, IPRange, Prefix, Service
 from netaddr import IPNetwork
-from rest_framework import status
+from rest_framework import mixins, status
+from rest_framework.exceptions import ValidationError
 from rest_framework.generics import get_object_or_404
 from rest_framework.renderers import BrowsableAPIRenderer, JSONRenderer
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.routers import APIRootView
 from rest_framework.views import APIView
 from rest_framework.viewsets import GenericViewSet
 from virtualization.filtersets import VirtualMachineFilterSet
 from virtualization.models import VirtualMachine
 
 from .constants import AS_CIDR_PARAM_NAME, FAMILY_PARAM_NAME, SUMMARIZE_PARAM_NAME
 from .filtersets import CustomPrefixFilterSet
 from .renderers import PlainTextRenderer
+from .serializers import PrometheusDeviceSerializer, PrometheusVMSerializer
 from .utils import (
     device_vm_primary_list,
+    filter_queryset,
     get_as_cidr_param,
-    get_attr_r,
+    get_attr_json,
     get_family_param,
     get_service_ips,
     get_summarize_param,
     get_svc_primary_ips_param,
     iprange_to_cidrs,
     make_ip_list_response,
     set_prefixlen_max,
-    filter_queryset,
 )
 
 FAMILY_PARAM = openapi.Parameter(
     FAMILY_PARAM_NAME,
     in_=openapi.IN_QUERY,
     description="Filter IPs and or prefixes by address family (4|6).",
     type=openapi.TYPE_INTEGER,
@@ -62,39 +64,69 @@
 )
 SUMMARIZE_PARAM = openapi.Parameter(
     SUMMARIZE_PARAM_NAME,
     in_=openapi.IN_QUERY,
     description="Summarize the IPs/Prefixes before returning them.",
     type=openapi.TYPE_BOOLEAN,
 )
+IP_PREFIX_RESPONSES = {
+    200: openapi.Schema(type="array", items=openapi.Schema(type="string"))
+}
+
+OTHER_PARAMS = {
+    FAMILY_PARAM_NAME,
+    AS_CIDR_PARAM_NAME,
+    SUMMARIZE_PARAM_NAME,
+    # for BrowsableAPIRenderer
+    "format",
+}
 
 
 class ListsRootView(APIRootView):
     def get_view_name(self):
         return "Lists"
 
 
+class InvalidFilterCheckMixin:
+    # Adapted from
+    # https://stackoverflow.com/questions/27182527/how-can-i-stop-django-rest-framework-to-show-all-records-if-query-parameter-is-w
+    def get_queryset(self):
+        other_params = getattr(self, "other_query_params", OTHER_PARAMS)
+        qs = super().get_queryset()
+        invalid_filters = set(self.request.query_params).difference(
+            other_params, self.filterset_class.get_filters()
+        )
+
+        if len(invalid_filters) > 0:
+            raise ValidationError({k: "Invalid filter." for k in invalid_filters})
+
+        return qs
+
+
 class ListsBaseViewSet(GenericViewSet):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer, PlainTextRenderer]
+    pagination_class = None
 
     # Adapted from
     # https://github.com/netbox-community/netbox/blob/a33e47780b42f49f4ea536bace1617fa7dda31ab/
     # netbox/netbox/api/views.py#L179
     def initial(self, request: Request, *args, **kwargs):
         super().initial(request, *args, **kwargs)
 
         if not request.user.is_authenticated:
             return
 
         # Restrict the view's QuerySet to allow only the permitted objects
         self.queryset = self.queryset.restrict(request.user, "view")
 
 
-class ValuesListViewSet(ListsBaseViewSet):
-    @swagger_auto_schema(manual_parameters=[SUMMARIZE_PARAM])
+class ValuesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
+    @swagger_auto_schema(
+        manual_parameters=[SUMMARIZE_PARAM], responses=IP_PREFIX_RESPONSES
+    )
     def list(self, request: Request, use_net_ip: bool = False) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             queryset, get_summarize_param(request), use_net_ip=use_net_ip
         )
 
 
@@ -104,43 +136,48 @@
 
 
 class AggregateListViewSet(ValuesListViewSet):
     queryset = Aggregate.objects.values_list("prefix", flat=True).distinct()
     filterset_class = AggregateFilterSet
 
 
-class IPAddressListViewSet(ListsBaseViewSet):
+class IPAddressListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = IPAddress.objects.values_list("address", flat=True).distinct()
     filterset_class = IPAddressFilterSet
 
-    @swagger_auto_schema(manual_parameters=[AS_CIDR_PARAM])
+    @swagger_auto_schema(
+        manual_parameters=[AS_CIDR_PARAM], responses=IP_PREFIX_RESPONSES
+    )
     def list(self, request) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             (set_prefixlen_max(i) for i in queryset),
             get_summarize_param(request),
             use_net_ip=not get_as_cidr_param(request),
         )
 
 
-class ServiceListviewSet(ListsBaseViewSet):
+class ServiceListviewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = Service.objects.all()
     filterset_class = ServiceFilterSet
+    other_query_params = OTHER_PARAMS.union({"primary_ips"})
 
     @swagger_auto_schema(
         manual_parameters=[
+            FAMILY_PARAM,
             AS_CIDR_PARAM,
             SUMMARIZE_PARAM,
             openapi.Parameter(
                 "primary_ips",
                 in_=openapi.IN_QUERY,
                 description="Return Primary IPs if the service doesn't have any assigned IPs.",
                 type=openapi.TYPE_BOOLEAN,
             ),
-        ]
+        ],
+        responses=IP_PREFIX_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         as_cidr = get_as_cidr_param(request)
         family = get_family_param(request)
         summarize = get_summarize_param(request)
         primary_ips = get_svc_primary_ips_param("primary_ips", request)
 
@@ -148,21 +185,22 @@
         return make_ip_list_response(
             get_service_ips(qs, family, primary_ips),
             summarize,
             use_net_ip=not as_cidr,
         )
 
 
-class DevicesListViewSet(ListsBaseViewSet):
+class DevicesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = Device.objects.all()
     filterset_class = DeviceFilterSet
 
     @swagger_auto_schema(
         operation_description="Returns the primary IPs of devices.",
         manual_parameters=[AS_CIDR_PARAM, FAMILY_PARAM, SUMMARIZE_PARAM],
+        responses=IP_PREFIX_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         return make_ip_list_response(
@@ -171,21 +209,22 @@
                 family,
             ),
             summarize,
             use_net_ip=not as_cidr,
         )
 
 
-class VirtualMachinesListViewSet(ListsBaseViewSet):
+class VirtualMachinesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = VirtualMachine.objects.all()
     filterset_class = VirtualMachineFilterSet
 
     @swagger_auto_schema(
         operation_description="Returns the primary IPs of virtual machines.",
         manual_parameters=[AS_CIDR_PARAM, FAMILY_PARAM],
+        responses=IP_PREFIX_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         return make_ip_list_response(
@@ -204,20 +243,34 @@
     # Cannot apply TokenPermissions on a view that does not set `.queryset` or have a `.get_queryset()` method.
     # See https://github.com/encode/django-rest-framework/blob/
     # 71e6c30034a1dd35a39ca74f86c371713e762c79/rest_framework/permissions.py#L207
     #
     # Therefore, we use Device as the model.
     queryset = Device.objects.all()
 
+    def validate_filters(self):
+        valid_filters = OTHER_PARAMS.union(
+            set(DeviceFilterSet.get_filters()).intersection(
+                VirtualMachineFilterSet.get_filters()
+            )
+        )
+
+        invalid_filters = set(self.request.query_params).difference(valid_filters)
+        if len(invalid_filters) > 0:
+            raise ValidationError({k: "Invalid filter." for k in invalid_filters})
+
     @swagger_auto_schema(
         operation_description="Combined devices and virtual machines primary IPs list. "
-        "Use only parameters common to both devices and VMs ('role' can be used for both devices and VMs).",
+        "Use only parameters common to both devices and VMs.",
         manual_parameters=[SUMMARIZE_PARAM],
+        responses=IP_PREFIX_RESPONSES,
     )
     def get(self, request: Request) -> Response:
+        self.validate_filters()
+
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         devices_qs = filter_queryset(
             DeviceFilterSet(
                 request.query_params,
@@ -233,21 +286,22 @@
         devices = device_vm_primary_list(devices_qs, family)
         vms = device_vm_primary_list(vms_qs, family)
         return make_ip_list_response(
             itertools.chain(devices, vms), summarize, use_net_ip=not as_cidr
         )
 
 
-class IPRangeListViewSet(ListsBaseViewSet):
+class IPRangeListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = IPRange.objects.all()
     filterset_class = IPRangeFilterSet
 
     @swagger_auto_schema(
         operation_description="Returns a list of CIDRs for each range.",
         manual_parameters=[SUMMARIZE_PARAM],
+        responses=IP_PREFIX_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             itertools.chain.from_iterable(
                 iprange_to_cidrs(r.start_address.ip, r.end_address.ip) for r in queryset
             ),
@@ -371,17 +425,42 @@
             return []
 
         return device_vm_primary_list(
             VirtualMachine.objects.restrict(request.user, "view").filter(tags=tag),
             family,
         )
 
+    def check_query(self) -> None:
+        """Raises an exception if an invalid query param is used."""
+        valid_params = {
+            SUMMARIZE_PARAM_NAME,
+            FAMILY_PARAM_NAME,
+            "prefixes",
+            "aggregates",
+            "services",
+            "devices",
+            "vms",
+            "devices_primary",
+            "vms_primary",
+            "ips",
+            "service_primary_ips",
+            "all",
+            "all_primary",
+            # for BrowsableAPIRenderer
+            "format",
+        }
+
+        invalid_params = set(self.request.query_params).difference(valid_params)
+        if len(invalid_params) > 0:
+            raise ValidationError({k: "Invalid filter." for k in invalid_params})
+
     @swagger_auto_schema(
         manual_parameters=[
             SUMMARIZE_PARAM,
+            FAMILY_PARAM,
             openapi.Parameter(
                 "prefixes",
                 in_=openapi.IN_QUERY,
                 description="Include prefixes",
                 type=openapi.TYPE_BOOLEAN,
             ),
             openapi.Parameter(
@@ -440,20 +519,23 @@
             ),
             openapi.Parameter(
                 "all_primary",
                 in_=openapi.IN_QUERY,
                 description="Include ALL of the above options, using Device/VM primary IPs.",
                 type=openapi.TYPE_BOOLEAN,
             ),
-        ]
+        ],
+        responses=IP_PREFIX_RESPONSES,
     )
     def retrieve(self, request, slug=None) -> Response:
         if not slug:
             return Response("No slug", status.HTTP_400_BAD_REQUEST)
 
+        self.check_query()
+
         tag = get_object_or_404(Tag, slug=slug)
         family = get_family_param(request)
 
         prefixes = self.get_prefixes(tag, family, request)
         aggregates = self.get_aggregates(tag, family, request)
         ips = self.get_ips(tag, family, request)
         services = self.get_services(tag, family, request)
@@ -464,107 +546,67 @@
             itertools.chain(
                 prefixes, aggregates, ips, services, devices_primary, vms_primary
             ),
             get_summarize_param(request),
         )
 
 
-class PrometheusDeviceSD(GenericViewSet):
+class PrometheusDeviceSD(
+    InvalidFilterCheckMixin, mixins.ListModelMixin, ListsBaseViewSet
+):
     queryset = Device.objects.all()
     filterset_class = DeviceFilterSet
-
-    def _sd_device(self, d: Device) -> Dict[str, Any]:
-        labels = {
-            "__meta_netbox_id": d.id,
-            "__meta_netbox_name": d.name,
-            "__meta_netbox_status": d.status,
-            "__meta_netbox_site_name": d.site.name,
-            "__meta_netbox_platform_name": d.platform.name if d.platform else "",
-            "__meta_netbox_primary_ip": str(d.primary_ip.address.ip)
-            if d.primary_ip
-            else "",
-            "__meta_netbox_primary_ip4": str(d.primary_ip4.address.ip)
-            if d.primary_ip4
-            else "",
-            "__meta_netbox_primary_ip6": str(d.primary_ip6.address.ip)
-            if d.primary_ip6
-            else "",
-            "__meta_netbox_serial": d.serial,
-        }
-        for k, v in d.custom_field_data.items():
-            labels[f"__meta_netbox_cf_{k}"] = v
-
-        return {
-            "targets": [str(d.primary_ip.address.ip) if d.primary_ip else d.name],
-            "labels": labels,
-        }
-
-    def list(self, request: Request) -> Response:
-        queryset = self.filter_queryset(self.get_queryset())
-        return Response([self._sd_device(d) for d in queryset])
+    serializer_class = PrometheusDeviceSerializer
 
 
-class PrometheusVirtualMachineSD(GenericViewSet):
+class PrometheusVirtualMachineSD(
+    InvalidFilterCheckMixin, mixins.ListModelMixin, ListsBaseViewSet
+):
     queryset = VirtualMachine.objects.filter()
     filterset_class = VirtualMachineFilterSet
-
-    def _sd_vm(self, vm: VirtualMachine) -> Dict[str, Any]:
-        labels = {
-            "__meta_netbox_id": str(vm.id),
-            "__meta_netbox_name": vm.name,
-            "__meta_netbox_status": vm.status,
-            "__meta_netbox_cluster_name": vm.cluster.name,
-            "__meta_netbox_site_name": vm.site.name if vm.site else "",
-            "__meta_netbox_role_name": vm.role.name if vm.role else "",
-            "__meta_netbox_platform_name": vm.platform.name if vm.platform else "",
-            "__meta_netbox_primary_ip": str(vm.primary_ip.address.ip)
-            if vm.primary_ip
-            else "",
-            "__meta_netbox_primary_ip4": str(vm.primary_ip4.address.ip)
-            if vm.primary_ip4
-            else "",
-            "__meta_netbox_primary_ip6": str(vm.primary_ip6.address.ip)
-            if vm.primary_ip6
-            else "",
-        }
-        for k, v in vm.custom_field_data.items():
-            labels[f"__meta_netbox_cf_{k}"] = str(v)
-
-        return {
-            "targets": [str(vm.primary_ip.address.ip) if vm.primary_ip else vm.name],
-            "labels": labels,
-        }
-
-    def list(self, request: Request) -> Response:
-        queryset = self.filter_queryset(self.get_queryset())
-        return Response([self._sd_vm(vm) for vm in queryset])
+    serializer_class = PrometheusVMSerializer
 
 
 class DevicesVMsAttrsListView(APIView):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer]
     queryset = Device.objects.all()
 
     def _to_dict(
         self,
-        attrs: List[str],
-        display_attrs: List[str],
+        attrs: Iterable[Iterable[str]],
+        display_attrs: Iterable[Iterable[str]],
         device: Union[Device, VirtualMachine],
     ) -> Dict[str, Any]:
         """Convert a device or VM to a dictionary"""
-        return {d_a: get_attr_r(a, device) for a, d_a in zip(attrs, display_attrs)}
+        return {
+            "__".join(d_a): get_attr_json(a, device)
+            for a, d_a in zip(attrs, display_attrs)
+        }
+
+    def validate_filters(self):
+        valid_filters = set(DeviceFilterSet.get_filters()).intersection(
+            VirtualMachineFilterSet.get_filters()
+        )
+
+        invalid_filters = set(self.request.query_params).difference(valid_filters)
+        if len(invalid_filters) > 0:
+            raise ValidationError({k: "Invalid filter." for k in invalid_filters})
 
     def get(self, request: Request) -> Response:
+        self.validate_filters()
+
         attrs = settings.PLUGINS_CONFIG["netbox_lists"]["devices_vms_attrs"]
 
-        device_attrs = []
+        # TODO remove in next major release
+        attrs = [a.split("__") if isinstance(a, str) else a for a in attrs]
+
+        device_attrs: List[Iterable[str]] = []
         for a in attrs:
-            if a == "role":
-                device_attrs.append("role")
-            elif a.startswith("role__"):
-                device_attrs.append(a.replace("role__", "device_role__"))
+            if len(a) > 0 and a[0] == "role":
+                device_attrs.append(("device_role", *a[1:]))
             else:
                 device_attrs.append(a)
 
         devices = filter_queryset(
             DeviceFilterSet(
                 request.query_params,
                 queryset=Device.objects.restrict(request.user, "view").all(),
```

### Comparing `netbox-lists-2.1.1/pyproject.toml` & `netbox-lists-2.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "netbox-lists"
-version = "2.1.1"
+version = "2.2.0"
 description = ""
 authors = ["Devon Mar <devonm@mdmm.ca>"]
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 netaddr = "^0.8.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^3.8"
-pynetbox = "^6.1.3"
-requests = "^2.26.0"
+pytest = "^7.0"
+flake8 = "^5.0"
+pynetbox = "^6.6.2"
+requests = "^2.27.1"
 isort = "^5.10.1"
-black = "^22.1.0"
-mypy = "^0.941"
+black = "^22.8.0"
+mypy = "^0.971"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `netbox-lists-2.1.1/setup.py` & `netbox-lists-2.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['netaddr>=0.8.0,<0.9.0']
 
 setup_kwargs = {
     'name': 'netbox-lists',
-    'version': '2.1.1',
+    'version': '2.2.0',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Devon Mar',
     'author_email': 'devonm@mdmm.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6.2,<4.0.0',
 }
```

