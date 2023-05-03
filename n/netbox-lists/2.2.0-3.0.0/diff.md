# Comparing `tmp/netbox-lists-2.2.0.tar.gz` & `tmp/netbox_lists-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-lists-2.2.0.tar", max compression
+gzip compressed data, was "netbox_lists-3.0.0.tar", max compression
```

## Comparing `netbox-lists-2.2.0.tar` & `netbox_lists-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11358 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/LICENSE
--rw-r--r--   0        0        0     2174 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/__init__.py
--rw-r--r--   0        0        0       95 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/constants.py
--rw-r--r--   0        0        0     1942 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/filtersets.py
--rw-r--r--   0        0        0      547 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/api/renderers.py
--rw-r--r--   0        0        0     2009 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/serializers.py
--rw-r--r--   0        0        0     1258 2023-04-30 05:28:18.803210 netbox-lists-2.2.0/netbox_lists/api/urls.py
--rw-r--r--   0        0        0     6649 2023-05-02 22:13:53.326068 netbox-lists-2.2.0/netbox_lists/api/utils.py
--rw-r--r--   0        0        0    21353 2023-05-02 22:13:55.566068 netbox-lists-2.2.0/netbox_lists/api/views.py
--rw-r--r--   0        0        0        0 2023-04-28 07:46:42.287331 netbox-lists-2.2.0/netbox_lists/py.typed
--rw-r--r--   0        0        0      997 2023-05-03 00:01:36.986215 netbox-lists-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 netbox-lists-2.2.0/setup.py
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 netbox-lists-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2174 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/constants.py
+-rw-r--r--   0        0        0     1942 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/filtersets.py
+-rw-r--r--   0        0        0      547 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/renderers.py
+-rw-r--r--   0        0        0     1606 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/serializers.py
+-rw-r--r--   0        0        0     1212 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/urls.py
+-rw-r--r--   0        0        0     6639 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/utils.py
+-rw-r--r--   0        0        0    25564 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/api/views.py
+-rw-r--r--   0        0        0        0 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/netbox_lists/py.typed
+-rw-r--r--   0        0        0      979 2023-05-03 03:30:58.021344 netbox_lists-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 netbox_lists-3.0.0/PKG-INFO
```

### Comparing `netbox-lists-2.2.0/LICENSE` & `netbox_lists-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.2.0/netbox_lists/__init__.py` & `netbox_lists-3.0.0/netbox_lists/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.2.0/netbox_lists/api/filtersets.py` & `netbox_lists-3.0.0/netbox_lists/api/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.2.0/netbox_lists/api/renderers.py` & `netbox_lists-3.0.0/netbox_lists/api/renderers.py`

 * *Files identical despite different names*

### Comparing `netbox-lists-2.2.0/netbox_lists/api/urls.py` & `netbox_lists-3.0.0/netbox_lists/api/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from django.urls import path
 from rest_framework.routers import DefaultRouter
 
 from .views import (
     AggregateListViewSet,
     DevicesListViewSet,
-    DevicesVMsAttrsListView,
-    DevicesVMsListView,
+    DevicesVMsAttrsListViewSet,
+    DevicesVMsListViewSet,
     IPAddressListViewSet,
     IPRangeListViewSet,
     ListsRootView,
     PrefixListViewSet,
     PrometheusDeviceSD,
     PrometheusVirtualMachineSD,
     ServiceListviewSet,
@@ -31,12 +30,10 @@
 router.register("devices", DevicesListViewSet, basename="devices")
 router.register(
     "virtual-machines", VirtualMachinesListViewSet, basename="virtual-machines"
 )
 router.register("prometheus-devices", PrometheusDeviceSD)
 router.register("prometheus-vms", PrometheusVirtualMachineSD)
 
-urlpatterns = [
-    path("devices-vms/", DevicesVMsListView.as_view()),
-    path("devices-vms-attrs/", DevicesVMsAttrsListView.as_view()),
-]
-urlpatterns += router.urls
+router.register("devices-vms", DevicesVMsListViewSet)
+router.register("devices-vms-attrs", DevicesVMsAttrsListViewSet)
+urlpatterns = router.urls
```

### Comparing `netbox-lists-2.2.0/netbox_lists/api/utils.py` & `netbox_lists-3.0.0/netbox_lists/api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     return (set_prefixlen_max(i) for i in itertools.chain.from_iterable(iterables))
 
 
 def get_svc_primary_ips_param(param: str, req: Request) -> bool:
     val = req.query_params.get(param, None)
     if val is None:
-        return settings.PLUGINS_CONFIG["netbox_lists"].get("service_primary_ips", True)
+        return settings.PLUGINS_CONFIG["netbox_lists"]["service_primary_ips"]
     elif val.lower() == "true":
         return True
     elif val.lower() == "false":
         return False
     else:
         raise ValidationError(f"{param} must be true or false.")
```

### Comparing `netbox-lists-2.2.0/netbox_lists/api/views.py` & `netbox_lists-3.0.0/netbox_lists/api/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import itertools
 import operator
 from functools import reduce
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
 
-import netaddr
 from dcim.filtersets import DeviceFilterSet
 from dcim.models import Device
 from django.conf import settings
 from django.db.models import Q
-from drf_yasg import openapi
-from drf_yasg.utils import swagger_auto_schema
+from django_filters.rest_framework import DjangoFilterBackend
+from drf_spectacular.utils import (
+    extend_schema,
+    extend_schema_view,
+    OpenApiExample,
+    OpenApiParameter,
+    OpenApiResponse,
+)
 from extras.models import Tag
 from ipam.filtersets import (
     AggregateFilterSet,
     IPAddressFilterSet,
     IPRangeFilterSet,
     ServiceFilterSet,
 )
@@ -22,15 +27,14 @@
 from rest_framework import mixins, status
 from rest_framework.exceptions import ValidationError
 from rest_framework.generics import get_object_or_404
 from rest_framework.renderers import BrowsableAPIRenderer, JSONRenderer
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.routers import APIRootView
-from rest_framework.views import APIView
 from rest_framework.viewsets import GenericViewSet
 from virtualization.filtersets import VirtualMachineFilterSet
 from virtualization.models import VirtualMachine
 
 from .constants import AS_CIDR_PARAM_NAME, FAMILY_PARAM_NAME, SUMMARIZE_PARAM_NAME
 from .filtersets import CustomPrefixFilterSet
 from .renderers import PlainTextRenderer
@@ -45,45 +49,109 @@
     get_summarize_param,
     get_svc_primary_ips_param,
     iprange_to_cidrs,
     make_ip_list_response,
     set_prefixlen_max,
 )
 
-FAMILY_PARAM = openapi.Parameter(
-    FAMILY_PARAM_NAME,
-    in_=openapi.IN_QUERY,
-    description="Filter IPs and or prefixes by address family (4|6).",
-    type=openapi.TYPE_INTEGER,
-    enum=[4, 6],
+FAMILY_PARAM = OpenApiParameter(
+    name=FAMILY_PARAM_NAME,
+    location="query",
+    description="Filter IPs and or prefixes by address family.",
+    type=int,
+    enum=(4, 6),
 )
-AS_CIDR_PARAM = openapi.Parameter(
-    AS_CIDR_PARAM_NAME,
-    in_=openapi.IN_QUERY,
+AS_CIDR_PARAM = OpenApiParameter(
+    name=AS_CIDR_PARAM_NAME,
+    location="query",
     description="Return IPs as /32 or /128",
-    type=openapi.TYPE_BOOLEAN,
+    default=settings.PLUGINS_CONFIG["netbox_lists"]["as_cidr"],
+    type=bool,
 )
-SUMMARIZE_PARAM = openapi.Parameter(
-    SUMMARIZE_PARAM_NAME,
-    in_=openapi.IN_QUERY,
-    description="Summarize the IPs/Prefixes before returning them.",
-    type=openapi.TYPE_BOOLEAN,
+SUMMARIZE_PARAM = OpenApiParameter(
+    name=SUMMARIZE_PARAM_NAME,
+    location="query",
+    description="Summarize the IPs/prefixes before returning them.",
+    type=bool,
+    default=settings.PLUGINS_CONFIG["netbox_lists"]["summarize"],
+)
+
+PROMETHEUS_RESPONSE_SCHEMA = OpenApiResponse(
+    response={
+        "type": "object",
+        "properties": {
+            "targets": {
+                "type": "array",
+                "items": {"type": "string", "description": "Primary IP or name"},
+            },
+            "labels": {"type": "object", "additionalProperties": {"type": "string"}},
+        },
+    },
+    examples=[
+        OpenApiExample(
+            "Device",
+            value={
+                "targets": ["2001:db8::1"],
+                "labels": {
+                    "__meta_netbox_id": "1",
+                    "__meta_netbox_name": "dmi01-akron-rtr01",
+                    "__meta_netbox_status": "active",
+                    "__meta_netbox_site_name": "DM-Akron",
+                    "__meta_netbox_platform_name": "Cisco IOS",
+                    "__meta_netbox_primary_ip": "2001:db8::1",
+                    "__meta_netbox_primary_ip4": "",
+                    "__meta_netbox_primary_ip6": "2001:db8::1",
+                    "__meta_netbox_serial": "",
+                },
+            },
+        ),
+        OpenApiExample(
+            "VM",
+            value={
+                "targets": ["192.0.2.100"],
+                "labels": {
+                    "__meta_netbox_id": "361",
+                    "__meta_netbox_name": "vm1",
+                    "__meta_netbox_status": "active",
+                    "__meta_netbox_cluster_name": "DO-AMS3",
+                    "__meta_netbox_site_name": "",
+                    "__meta_netbox_role_name": "Application Server",
+                    "__meta_netbox_platform_name": "Ubuntu Linux 20.04",
+                    "__meta_netbox_primary_ip": "192.0.2.100",
+                    "__meta_netbox_primary_ip4": "192.0.2.100",
+                    "__meta_netbox_primary_ip6": "",
+                },
+            },
+        ),
+    ],
 )
-IP_PREFIX_RESPONSES = {
-    200: openapi.Schema(type="array", items=openapi.Schema(type="string"))
-}
 
 OTHER_PARAMS = {
     FAMILY_PARAM_NAME,
     AS_CIDR_PARAM_NAME,
     SUMMARIZE_PARAM_NAME,
     # for BrowsableAPIRenderer
     "format",
 }
 
+LISTS_RESPONSES = {
+    (200, "application/json"): OpenApiResponse(
+        description="JSON or plain text list of IP addresses/prefixes.",
+        response=str,
+        examples=[
+            OpenApiExample("JSON example", value=["192.0.2.0/24", "2001:db8::/64"]),
+        ],
+    ),
+    (200, "text/plain"): OpenApiResponse(
+        response=str,
+        # This description is not used in swagger.
+        examples=[OpenApiExample("Text example", value="192.0.2.0/24\n2001:db8::/64")],
+    ),
+}
+
 
 class ListsRootView(APIRootView):
     def get_view_name(self):
         return "Lists"
 
 
 class InvalidFilterCheckMixin:
@@ -98,17 +166,19 @@
 
         if len(invalid_filters) > 0:
             raise ValidationError({k: "Invalid filter." for k in invalid_filters})
 
         return qs
 
 
+# View set instead of APIView sknce it makes OpenApi filtersets work.
 class ListsBaseViewSet(GenericViewSet):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer, PlainTextRenderer]
     pagination_class = None
+    filter_backends = (DjangoFilterBackend,)  # disable ordering
 
     # Adapted from
     # https://github.com/netbox-community/netbox/blob/a33e47780b42f49f4ea536bace1617fa7dda31ab/
     # netbox/netbox/api/views.py#L179
     def initial(self, request: Request, *args, **kwargs):
         super().initial(request, *args, **kwargs)
 
@@ -116,68 +186,72 @@
             return
 
         # Restrict the view's QuerySet to allow only the permitted objects
         self.queryset = self.queryset.restrict(request.user, "view")
 
 
 class ValuesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
-    @swagger_auto_schema(
-        manual_parameters=[SUMMARIZE_PARAM], responses=IP_PREFIX_RESPONSES
-    )
+    @extend_schema(parameters=[SUMMARIZE_PARAM], responses=LISTS_RESPONSES)
     def list(self, request: Request, use_net_ip: bool = False) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             queryset, get_summarize_param(request), use_net_ip=use_net_ip
         )
 
 
+@extend_schema_view(list=extend_schema(description="Get a list of prefixes."))
 class PrefixListViewSet(ValuesListViewSet):
     queryset = Prefix.objects.values_list("prefix", flat=True).distinct()
     filterset_class = CustomPrefixFilterSet
 
 
+@extend_schema_view(list=extend_schema(description="Get a list of aggregate prefixes."))
 class AggregateListViewSet(ValuesListViewSet):
     queryset = Aggregate.objects.values_list("prefix", flat=True).distinct()
     filterset_class = AggregateFilterSet
 
 
 class IPAddressListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = IPAddress.objects.values_list("address", flat=True).distinct()
     filterset_class = IPAddressFilterSet
 
-    @swagger_auto_schema(
-        manual_parameters=[AS_CIDR_PARAM], responses=IP_PREFIX_RESPONSES
+    @extend_schema(
+        description="Get a list of IP addresses.",
+        parameters=[AS_CIDR_PARAM, SUMMARIZE_PARAM],
+        responses=LISTS_RESPONSES,
     )
-    def list(self, request) -> Response:
+    def list(self, request: Request) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             (set_prefixlen_max(i) for i in queryset),
             get_summarize_param(request),
             use_net_ip=not get_as_cidr_param(request),
         )
 
 
 class ServiceListviewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = Service.objects.all()
     filterset_class = ServiceFilterSet
     other_query_params = OTHER_PARAMS.union({"primary_ips"})
 
-    @swagger_auto_schema(
-        manual_parameters=[
+    @extend_schema(
+        description="Get a list of IPs associated with services.",
+        parameters=[
             FAMILY_PARAM,
             AS_CIDR_PARAM,
             SUMMARIZE_PARAM,
-            openapi.Parameter(
-                "primary_ips",
-                in_=openapi.IN_QUERY,
+            OpenApiParameter(
+                name="primary_ips",
+                location="query",
                 description="Return Primary IPs if the service doesn't have any assigned IPs.",
-                type=openapi.TYPE_BOOLEAN,
+                type=bool,
+                default=settings.PLUGINS_CONFIG["netbox_lists"]["service_primary_ips"],
             ),
         ],
-        responses=IP_PREFIX_RESPONSES,
+        responses=LISTS_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         as_cidr = get_as_cidr_param(request)
         family = get_family_param(request)
         summarize = get_summarize_param(request)
         primary_ips = get_svc_primary_ips_param("primary_ips", request)
 
@@ -189,18 +263,18 @@
         )
 
 
 class DevicesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = Device.objects.all()
     filterset_class = DeviceFilterSet
 
-    @swagger_auto_schema(
-        operation_description="Returns the primary IPs of devices.",
-        manual_parameters=[AS_CIDR_PARAM, FAMILY_PARAM, SUMMARIZE_PARAM],
-        responses=IP_PREFIX_RESPONSES,
+    @extend_schema(
+        description="Get the primary IPs of devices.",
+        parameters=[AS_CIDR_PARAM, FAMILY_PARAM, SUMMARIZE_PARAM],
+        responses=LISTS_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         return make_ip_list_response(
@@ -213,18 +287,18 @@
         )
 
 
 class VirtualMachinesListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = VirtualMachine.objects.all()
     filterset_class = VirtualMachineFilterSet
 
-    @swagger_auto_schema(
-        operation_description="Returns the primary IPs of virtual machines.",
-        manual_parameters=[AS_CIDR_PARAM, FAMILY_PARAM],
-        responses=IP_PREFIX_RESPONSES,
+    @extend_schema(
+        description="Get the primary IPs of virtual machines.",
+        parameters=[AS_CIDR_PARAM, FAMILY_PARAM, SUMMARIZE_PARAM],
+        responses=LISTS_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         return make_ip_list_response(
@@ -233,42 +307,43 @@
                 family,
             ),
             summarize,
             use_net_ip=not as_cidr,
         )
 
 
-class DevicesVMsListView(APIView):
+class DevicesVMsListViewSet(ListsBaseViewSet):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer, PlainTextRenderer]
     # We need to have `queryset defined`. Otherwise, the following occurs:
     # Cannot apply TokenPermissions on a view that does not set `.queryset` or have a `.get_queryset()` method.
     # See https://github.com/encode/django-rest-framework/blob/
     # 71e6c30034a1dd35a39ca74f86c371713e762c79/rest_framework/permissions.py#L207
     #
     # Therefore, we use Device as the model.
     queryset = Device.objects.all()
+    filterset_class = DeviceFilterSet
 
     def validate_filters(self):
         valid_filters = OTHER_PARAMS.union(
             set(DeviceFilterSet.get_filters()).intersection(
                 VirtualMachineFilterSet.get_filters()
             )
         )
 
         invalid_filters = set(self.request.query_params).difference(valid_filters)
         if len(invalid_filters) > 0:
             raise ValidationError({k: "Invalid filter." for k in invalid_filters})
 
-    @swagger_auto_schema(
-        operation_description="Combined devices and virtual machines primary IPs list. "
-        "Use only parameters common to both devices and VMs.",
-        manual_parameters=[SUMMARIZE_PARAM],
-        responses=IP_PREFIX_RESPONSES,
+    @extend_schema(
+        description="Combined devices and virtual machines primary IPs list. "
+        "Use only filters common to both devices and VMs.",
+        parameters=[AS_CIDR_PARAM, FAMILY_PARAM, SUMMARIZE_PARAM],
+        responses=LISTS_RESPONSES,
     )
-    def get(self, request: Request) -> Response:
+    def list(self, request: Request) -> Response:
         self.validate_filters()
 
         family = get_family_param(request)
         as_cidr = get_as_cidr_param(request)
         summarize = get_summarize_param(request)
 
         devices_qs = filter_queryset(
@@ -290,18 +365,18 @@
         )
 
 
 class IPRangeListViewSet(InvalidFilterCheckMixin, ListsBaseViewSet):
     queryset = IPRange.objects.all()
     filterset_class = IPRangeFilterSet
 
-    @swagger_auto_schema(
-        operation_description="Returns a list of CIDRs for each range.",
-        manual_parameters=[SUMMARIZE_PARAM],
-        responses=IP_PREFIX_RESPONSES,
+    @extend_schema(
+        description="Get a list of CIDRs for each range.",
+        parameters=[SUMMARIZE_PARAM],
+        responses=LISTS_RESPONSES,
     )
     def list(self, request: Request) -> Response:
         queryset = self.filter_queryset(self.get_queryset())
         return make_ip_list_response(
             itertools.chain.from_iterable(
                 iprange_to_cidrs(r.start_address.ip, r.end_address.ip) for r in queryset
             ),
@@ -365,15 +440,15 @@
             .filter(Q(tags=tag) & family_filter)
             .values_list("prefix", flat=True)
             .distinct()
         )
 
     def get_ips(
         self, tag: Tag, family: Union[int, None], request: Request
-    ) -> Iterable[netaddr.IPNetwork]:
+    ) -> Iterable[IPNetwork]:
         if family == 4:
             family_filter = Q(address__family=4)
         elif family == 6:
             family_filter = Q(address__family=6)
         else:
             family_filter = Q()
 
@@ -449,88 +524,101 @@
             "format",
         }
 
         invalid_params = set(self.request.query_params).difference(valid_params)
         if len(invalid_params) > 0:
             raise ValidationError({k: "Invalid filter." for k in invalid_params})
 
-    @swagger_auto_schema(
-        manual_parameters=[
+    @extend_schema(
+        description="Get a list of IPs/prefixes associated with the tag.",
+        parameters=[
             SUMMARIZE_PARAM,
             FAMILY_PARAM,
-            openapi.Parameter(
-                "prefixes",
-                in_=openapi.IN_QUERY,
-                description="Include prefixes",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "aggregates",
-                in_=openapi.IN_QUERY,
-                description="Include aggregates",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "services",
-                in_=openapi.IN_QUERY,
-                description="Include services",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "devices",
-                in_=openapi.IN_QUERY,
-                description="Include devices",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "vms",
-                in_=openapi.IN_QUERY,
-                description="Include vms",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "devices_primary",
-                in_=openapi.IN_QUERY,
-                description="Include devices (primary IPs only)",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "vms_primary",
-                in_=openapi.IN_QUERY,
-                description="Include vms (primary IPs only)",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "ips",
-                in_=openapi.IN_QUERY,
-                description="Include IP Addresses",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "service_primary_ips",
-                in_=openapi.IN_QUERY,
-                description="Return Primary IPs if the service doesn't have any assigned IPs.",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "all",
-                in_=openapi.IN_QUERY,
-                description="Include ALL of the above options except *_primary.",
-                type=openapi.TYPE_BOOLEAN,
-            ),
-            openapi.Parameter(
-                "all_primary",
-                in_=openapi.IN_QUERY,
-                description="Include ALL of the above options, using Device/VM primary IPs.",
-                type=openapi.TYPE_BOOLEAN,
+            OpenApiParameter(
+                name="prefixes",
+                location="query",
+                description="Include prefixes.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="aggregates",
+                location="query",
+                description="Include aggregates.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="services",
+                location="query",
+                description="Include services.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="devices",
+                location="query",
+                description="Include devices. Mutually exclusive with `devices_primary`.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="vms",
+                location="query",
+                description="Include VMs. Mutually exclusive with `vms_primary`.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="devices_primary",
+                location="query",
+                description="Include devices (primary IPs only). Mutually exclusive with `devices`.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="vms_primary",
+                location="query",
+                description="Include VMs (primary IPs only). Mutually exclusive with `vms`.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="ips",
+                location="query",
+                description="Include IP Addresses.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="service_primary_ips",
+                location="query",
+                description="Return primary IPs if the service doesn't have any assigned IPs. "
+                "Only used if `services=True`.",
+                type=bool,
+                default=settings.PLUGINS_CONFIG["netbox_lists"]["service_primary_ips"],
+            ),
+            OpenApiParameter(
+                name="all",
+                location="query",
+                description="Include **all** options except *_primary.",
+                type=bool,
+                default=False,
+            ),
+            OpenApiParameter(
+                name="all_primary",
+                location="query",
+                description="Include **all** options, using device/VM primary IPs.",
+                type=bool,
+                default=False,
             ),
         ],
-        responses=IP_PREFIX_RESPONSES,
+        responses=LISTS_RESPONSES,
     )
-    def retrieve(self, request, slug=None) -> Response:
+    def retrieve(self, request: Request, slug: Optional[str] = None) -> Response:
         if not slug:
             return Response("No slug", status.HTTP_400_BAD_REQUEST)
 
         self.check_query()
 
         tag = get_object_or_404(Tag, slug=slug)
         family = get_family_param(request)
@@ -562,17 +650,19 @@
     InvalidFilterCheckMixin, mixins.ListModelMixin, ListsBaseViewSet
 ):
     queryset = VirtualMachine.objects.filter()
     filterset_class = VirtualMachineFilterSet
     serializer_class = PrometheusVMSerializer
 
 
-class DevicesVMsAttrsListView(APIView):
+class DevicesVMsAttrsListViewSet(ListsBaseViewSet):
     renderer_classes = [JSONRenderer, BrowsableAPIRenderer]
-    queryset = Device.objects.all()
+    filterset_class = DeviceFilterSet
+    filter_backends = (DjangoFilterBackend,)
+    queryset = Device.objects.filter()
 
     def _to_dict(
         self,
         attrs: Iterable[Iterable[str]],
         display_attrs: Iterable[Iterable[str]],
         device: Union[Device, VirtualMachine],
     ) -> Dict[str, Any]:
@@ -587,22 +677,44 @@
             VirtualMachineFilterSet.get_filters()
         )
 
         invalid_filters = set(self.request.query_params).difference(valid_filters)
         if len(invalid_filters) > 0:
             raise ValidationError({k: "Invalid filter." for k in invalid_filters})
 
-    def get(self, request: Request) -> Response:
+    @extend_schema(
+        description="Get a list of device and VM objects. "
+        "Use only filters common to both devices and VMs.",
+        responses={
+            200: OpenApiResponse(
+                response={
+                    "type": "array",
+                    "items": {"type": "object", "additionalProperties": True},
+                },
+                examples=[
+                    OpenApiExample(
+                        "Example 1",
+                        value={
+                            "id": 1,
+                            "name": "dmi01-akron-rtr01",
+                            "role__slug": "router",
+                            "platform__slug": "cisco-ios",
+                            "primary_ip__address": "2001:db8::1/64",
+                            "tags": [],
+                        },
+                    )
+                ],
+            )
+        },
+    )
+    def list(self, request: Request) -> Response:
         self.validate_filters()
 
         attrs = settings.PLUGINS_CONFIG["netbox_lists"]["devices_vms_attrs"]
 
-        # TODO remove in next major release
-        attrs = [a.split("__") if isinstance(a, str) else a for a in attrs]
-
         device_attrs: List[Iterable[str]] = []
         for a in attrs:
             if len(a) > 0 and a[0] == "role":
                 device_attrs.append(("device_role", *a[1:]))
             else:
                 device_attrs.append(a)
```

### Comparing `netbox-lists-2.2.0/pyproject.toml` & `netbox_lists-3.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "netbox-lists"
-version = "2.2.0"
+version = "3.0.0"
 description = ""
 authors = ["Devon Mar <devonm@mdmm.ca>"]
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 netaddr = "^0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 flake8 = "^5.0"
-pynetbox = "^6.6.2"
+pynetbox = "^7.0.1"
 requests = "^2.27.1"
 isort = "^5.10.1"
 black = "^22.8.0"
 mypy = "^0.971"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
@@ -38,15 +38,14 @@
 
 [[tool.mypy.overrides]]
 module = [
     "rest_framework.*",
     "taggit.*",
     "django_filters",
     "netaddr.*",
-    "drf_yasg.*",
     # NetBox
     "dcim.*",
     "ipam.*",
     "extras.*",
     "virtualization.*",
 ]
 ignore_missing_imports = true
```

