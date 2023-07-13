# Comparing `tmp/netbox_software-0.2.1.tar.gz` & `tmp/netbox_software-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.2.1.tar", max compression
+gzip compressed data, was "netbox_software-0.2.2.tar", max compression
```

## Comparing `netbox_software-0.2.1.tar` & `netbox_software-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.1/LICENSE
--rw-r--r--   0        0        0     3420 2023-07-12 13:04:05.122871 netbox_software-0.2.1/README.md
--rw-r--r--   0        0        0      640 2023-07-12 13:04:05.106870 netbox_software-0.2.1/netbox_software/__init__.py
--rw-r--r--   0        0        0      432 2023-07-12 08:33:18.432206 netbox_software-0.2.1/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.1/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     3279 2023-07-12 09:55:40.939239 netbox_software-0.2.1/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      317 2023-07-12 08:47:07.805077 netbox_software-0.2.1/netbox_software/api/urls.py
--rw-r--r--   0        0        0      797 2023-07-12 09:21:02.309618 netbox_software-0.2.1/netbox_software/api/views.py
--rw-r--r--   0        0        0     3000 2023-07-12 12:42:24.681855 netbox_software-0.2.1/netbox_software/filtersets.py
--rw-r--r--   0        0        0     4341 2023-07-12 09:26:23.994787 netbox_software-0.2.1/netbox_software/forms.py
--rw-r--r--   0        0        0     4000 2023-07-12 09:30:42.438940 netbox_software-0.2.1/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.1/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     6449 2023-07-12 09:43:09.423061 netbox_software-0.2.1/netbox_software/models.py
--rw-r--r--   0        0        0     2616 2023-07-12 09:55:40.931239 netbox_software-0.2.1/netbox_software/navigation.py
--rw-r--r--   0        0        0      799 2023-07-12 08:33:18.436206 netbox_software-0.2.1/netbox_software/search.py
--rw-r--r--   0        0        0     3283 2023-07-12 09:28:27.960779 netbox_software-0.2.1/netbox_software/tables.py
--rw-r--r--   0        0        0     5647 2023-07-12 12:45:38.932973 netbox_software-0.2.1/netbox_software/template_content.py
--rw-r--r--   0        0        0     1606 2023-07-12 07:09:12.516168 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0     2194 2023-07-11 16:51:09.747148 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2387 2023-07-12 12:46:24.945718 netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.1/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1685 2023-07-12 09:48:10.295965 netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     2079 2023-07-12 08:47:07.813077 netbox_software-0.2.1/netbox_software/urls.py
--rw-r--r--   0        0        0     3139 2023-07-12 08:33:18.388206 netbox_software-0.2.1/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-07-12 13:04:05.114870 netbox_software-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-13 08:07:13.677335 netbox_software-0.2.2/README.md
+-rw-r--r--   0        0        0      640 2023-07-13 08:07:13.665335 netbox_software-0.2.2/netbox_software/__init__.py
+-rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.2/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.2/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.2/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.2/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1357 2023-07-13 08:04:55.515077 netbox_software-0.2.2/netbox_software/api/views.py
+-rw-r--r--   0        0        0     4349 2023-07-13 08:04:55.507077 netbox_software-0.2.2/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     5698 2023-07-13 08:06:01.104149 netbox_software-0.2.2/netbox_software/forms.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.2/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     5415 2023-07-13 07:37:44.876577 netbox_software-0.2.2/netbox_software/models.py
+-rw-r--r--   0        0        0     3102 2023-07-13 07:37:44.872576 netbox_software-0.2.2/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1162 2023-07-13 07:37:44.888577 netbox_software-0.2.2/netbox_software/search.py
+-rw-r--r--   0        0        0     4494 2023-07-13 07:37:44.904577 netbox_software-0.2.2/netbox_software/tables.py
+-rw-r--r--   0        0        0     5647 2023-07-12 12:45:38.932973 netbox_software-0.2.2/netbox_software/template_content.py
+-rw-r--r--   0        0        0      954 2023-07-13 07:41:42.248256 netbox_software-0.2.2/netbox_software/templates/netbox_software/application.html
+-rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.2/netbox_software/templates/netbox_software/application_edit.html
+-rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.2/netbox_software/templates/netbox_software/applicationversion.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/applicationversion_edit.html
+-rw-r--r--   0        0        0     1613 2023-07-13 07:37:44.912577 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2201 2023-07-13 07:37:44.872576 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2395 2023-07-13 07:50:20.332738 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.2/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.2/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1685 2023-07-12 09:48:10.295965 netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     3416 2023-07-13 07:37:44.900577 netbox_software-0.2.2/netbox_software/urls.py
+-rw-r--r--   0        0        0     5243 2023-07-13 07:37:44.864576 netbox_software-0.2.2/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-07-13 08:07:13.669335 netbox_software-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.2/PKG-INFO
```

### Comparing `netbox_software-0.2.1/LICENSE` & `netbox_software-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.1/README.md` & `netbox_software-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.1          |
+|     3.2+       | 0.2.2          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

### Comparing `netbox_software-0.2.1/netbox_software/__init__.py` & `netbox_software-0.2.2/netbox_software/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.2.1'
+    version = '0.2.2'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
```

### Comparing `netbox_software-0.2.1/netbox_software/api/serializers.py` & `netbox_software-0.2.2/netbox_software/api/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from drf_spectacular.utils import extend_schema_field
 from django.contrib.contenttypes.models import ContentType
 
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
 from netbox.api.fields import ChoiceField, ContentTypeField, SerializedPKRelatedField
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from utilities.api import get_serializer_for_model
-from ..models import DeviceSoftware, SoftwareType, Vendor, SOFTWARE_ASSIGNMENT_MODELS
+from ..models import DeviceSoftware, SoftwareType, Vendor, SOFTWARE_ASSIGNMENT_MODELS, ApplicationVersion, Application
 
 
 # Vendor Serializer
 class VendorSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_software-api:vendor-detail')
 
     class Meta:
@@ -22,15 +22,15 @@
     url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_software-api:vendor-detail')
 
     class Meta:
         model = Vendor
         fields = ('id', 'url', 'display', 'name',)
 
 
-# Vendor Serializer
+# SoftwareType Serializer
 class SoftwareTypeSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:softwaretype-detail'
     )
 
     class Meta:
         model = SoftwareType
@@ -43,35 +43,82 @@
     )
 
     class Meta:
         model = SoftwareType
         fields = ('id', 'url', 'display', 'name',)
 
 
+# Application Serializer
+class ApplicationVersionSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:applicationversion-detail'
+    )
+
+    class Meta:
+        model = ApplicationVersion
+        fields = ('id', 'url', 'display', 'name', 'comments', 'custom_fields', 'created', 'last_updated',)
+
+
+class NestedApplicationVersionSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:applicationversion-detail'
+    )
+
+    class Meta:
+        model = ApplicationVersion
+        fields = ('id', 'url', 'display', 'name',)
+
+
+# Device Software Serializer
+class ApplicationSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:application-detail'
+    )
+    software_type = NestedSoftwareTypeSerializer()
+    vendor = NestedVendorSerializer()
+
+    class Meta:
+        model = Application
+        fields = (
+            'id', 'url', 'display', 'name', 'software_type', 'vendor', 'comments', 'tags', 'custom_fields',
+            'created', 'last_updated',
+        )
+
+
+class NestedApplicationSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:application-detail'
+    )
+
+    class Meta:
+        model = Application
+        fields = ('id', 'url', 'display', 'name',)
+
+
 # Device Software Serializer
 class DeviceSoftwareSerializer(NetBoxModelSerializer):
 
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
     assigned_object_type = ContentTypeField(
         queryset=ContentType.objects.filter(SOFTWARE_ASSIGNMENT_MODELS),
         required=False,
         allow_null=True
     )
     assigned_object = serializers.SerializerMethodField(read_only=True)
 
-    software_type = NestedSoftwareTypeSerializer()
-    vendor = NestedVendorSerializer()
+    app = NestedApplicationSerializer()
+    version = NestedApplicationVersionSerializer()
 
     class Meta:
         model = DeviceSoftware
         fields = (
-            'id', 'url', 'display', 'name', 'software_type', 'vendor', 'version', 'assigned_object_type',
-            'assigned_object_id', 'assigned_object', 'comments', 'tags', 'custom_fields', 'created', 'last_updated',
+            'id', 'url', 'display', 'app', 'version', 'assigned_object_type', 'assigned_object_id', 'assigned_object',
+            'comments', 'tags', 'custom_fields', 'created', 'last_updated',
         )
 
     @extend_schema_field(serializers.JSONField(allow_null=True))
     def get_assigned_object(self, obj):
         if obj.assigned_object is None:
             return None
         serializer = get_serializer_for_model(obj.assigned_object, prefix=NESTED_SERIALIZER_PREFIX)
@@ -82,9 +129,9 @@
 class NestedDeviceSoftwareSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
 
     class Meta:
         model = DeviceSoftware
-        fields = ('id', 'url', 'display', 'name', 'version',)
+        fields = ('id', 'url', 'display',)
```

### Comparing `netbox_software-0.2.1/netbox_software/api/views.py` & `netbox_software-0.2.2/netbox_software/api/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import models, filtersets
-from .serializers import DeviceSoftwareSerializer, SoftwareTypeSerializer, VendorSerializer
+from .serializers import DeviceSoftwareSerializer, SoftwareTypeSerializer, VendorSerializer, \
+    ApplicationVersionSerializer, ApplicationSerializer
 
 
 class VendorViewSet(NetBoxModelViewSet):
     queryset = models.Vendor.objects.all()
     serializer_class = VendorSerializer
     filterset_class = filtersets.VendorFilterSet
 
 
 class SoftwareTypeViewSet(NetBoxModelViewSet):
     queryset = models.SoftwareType.objects.all()
     serializer_class = SoftwareTypeSerializer
     filterset_class = filtersets.SoftwareTypeFilterSet
 
 
+class ApplicationVersionViewSet(NetBoxModelViewSet):
+    queryset = models.ApplicationVersion.objects.prefetch_related('tags')
+    serializer_class = ApplicationVersionSerializer
+    filterset_class = filtersets.ApplicationVersionFilterSet
+
+
+class ApplicationViewSet(NetBoxModelViewSet):
+    queryset = models.Application.objects.prefetch_related('tags', 'software_type', 'vendor')
+    serializer_class = ApplicationSerializer
+    filterset_class = filtersets.ApplicationFilterSet
+
+
 class DeviceSoftwareViewSet(NetBoxModelViewSet):
-    queryset = models.DeviceSoftware.objects.prefetch_related('tags', 'assigned_object')
+    queryset = models.DeviceSoftware.objects.prefetch_related('tags', 'app', 'version', 'assigned_object')
     serializer_class = DeviceSoftwareSerializer
     filterset_class = filtersets.DeviceSoftwareFilterSet
```

### Comparing `netbox_software-0.2.1/netbox_software/filtersets.py` & `netbox_software-0.2.2/netbox_software/filtersets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import django_filters
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext as _
 from netbox.filtersets import NetBoxModelFilterSet
 from utilities.filters import MultiValueNumberFilter, MultiValueCharFilter
 from dcim.models import Device
 from virtualization.models import VirtualMachine
-from .models import DeviceSoftware, SoftwareType, Vendor
+from .models import DeviceSoftware, SoftwareType, Vendor, ApplicationVersion, Application
 from django.db.models import Q
 
 
 class VendorFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Vendor
         fields = ('id', 'name',)
@@ -33,15 +33,64 @@
             return queryset
         return queryset.filter(
             Q(name__icontains=value) |
             Q(comments__icontains=value)
         )
 
 
+class ApplicationVersionFilterSet(NetBoxModelFilterSet):
+    class Meta:
+        model = ApplicationVersion
+        fields = ('id', 'name',)
+
+    def search(self, queryset, name, value):
+        if not value.strip():
+            return queryset
+        return queryset.filter(
+            Q(name__icontains=value) |
+            Q(comments__icontains=value)
+        )
+
+
+class ApplicationFilterSet(NetBoxModelFilterSet):
+    class Meta:
+        model = Application
+        fields = ('id', 'name', 'software_type', 'vendor')
+
+    def search(self, queryset, name, value):
+        if not value.strip():
+            return queryset
+        return queryset.filter(
+            Q(name__icontains=value) |
+            Q(comments__icontains=value)
+        )
+
+
 class DeviceSoftwareFilterSet(NetBoxModelFilterSet):
+    app = MultiValueCharFilter(
+        queryset=Application.objects.all(),
+        field_name='name',
+        lookup_expr='in',
+        label=_('App (name)'),
+    )
+    app_id = MultiValueNumberFilter(
+        queryset=Application.objects.all(),
+        label=_('App (ID)'),
+    )
+    version = MultiValueCharFilter(
+        queryset=ApplicationVersion.objects.all(),
+        field_name='name',
+        lookup_expr='in',
+        label=_('Version (name)'),
+    )
+    version_id = MultiValueNumberFilter(
+        queryset=ApplicationVersion.objects.all(),
+        label=_('Version (ID)'),
+    )
+
     device = MultiValueCharFilter(
         method='filter_device',
         field_name='name',
         label=_('Device (name)'),
     )
     device_id = MultiValueNumberFilter(
         method='filter_device',
@@ -57,21 +106,21 @@
         method='filter_virtual_machine',
         field_name='pk',
         label=_('Virtual machine (ID)'),
     )
 
     class Meta:
         model = DeviceSoftware
-        fields = ('id', 'name', 'software_type', 'vendor')
+        fields = ('id', 'app')
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
-            Q(name__icontains=value) |
+            Q(app__icontains=value) |
             Q(version__icontains=value)
         )
 
     def filter_device(self, queryset, name, value):
         devices = Device.objects.filter(**{'{}__in'.format(name): value})
         if not devices.exists():
             return queryset.none()
```

### Comparing `netbox_software-0.2.1/netbox_software/forms.py` & `netbox_software-0.2.2/netbox_software/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
 from dcim.models import Device
 from virtualization.models import VirtualMachine
-from .models import DeviceSoftware, SoftwareType, Vendor
+from .models import DeviceSoftware, SoftwareType, Vendor, ApplicationVersion, Application
 
 from django.conf import settings
 from packaging import version
 
 NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
 if NETBOX_CURRENT_VERSION >= version.parse("3.5"):
     from utilities.forms.fields import TagFilterField, CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField
@@ -42,14 +42,73 @@
 class SoftwareTypeFilterForm(NetBoxModelFilterSetForm):
     model = SoftwareType
     name = forms.CharField(
         label='Название',
         required=False
     )
 
+class ApplicationVersionForm(NetBoxModelForm):
+    comments = CommentField()
+    class Meta:
+        model = ApplicationVersion
+        fields = ('name', 'comments',)
+
+
+class ApplicationVersionFilterForm(NetBoxModelFilterSetForm):
+    model = ApplicationVersion
+    name = forms.CharField(
+        label='Название',
+        required=False
+    )
+
+
+class ApplicationForm(NetBoxModelForm):
+    comments = CommentField()
+
+    software_type = DynamicModelChoiceField(
+        label='Тип',
+        queryset=SoftwareType.objects.all(),
+        required=True
+    )
+    vendor = DynamicModelChoiceField(
+        label='Разработчик',
+        queryset=Vendor.objects.all(),
+        required=True
+    )
+
+    class Meta:
+        model = Application
+        fields = ('name', 'vendor', 'software_type', 'comments', 'tags')
+
+
+class ApplicationFilterForm(NetBoxModelFilterSetForm):
+    model = Application
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag')),
+        ('Атрибуты', ('name', 'software_type_id', 'vendor_id')),
+    )
+
+    name = forms.CharField(
+        label='Название',
+        required=False
+    )
+
+    software_type_id = forms.ModelMultipleChoiceField(
+        label='Тип',
+        queryset=SoftwareType.objects.all(),
+        required=False
+    )
+    vendor_id = forms.ModelMultipleChoiceField(
+        label='Разработчик',
+        queryset=Vendor.objects.all(),
+        required=False
+    )
+
+    tag = TagFilterField(model)
+
 
 # Device Software Form & Filter Form
 class DeviceSoftwareForm(NetBoxModelForm):
     comments = CommentField()
 
     device = DynamicModelChoiceField(
         label='Устройство',
@@ -58,29 +117,28 @@
     )
 
     virtual_machine = DynamicModelChoiceField(
         label='Устройство',
         queryset=VirtualMachine.objects.all(),
         required=False
     )
-
-    software_type = DynamicModelChoiceField(
-        label='Тип',
-        queryset=SoftwareType.objects.all(),
+    app = DynamicModelChoiceField(
+        label='ПО',
+        queryset=Application.objects.all(),
         required=True
     )
-    vendor = DynamicModelChoiceField(
-        label='Разработчик',
-        queryset=Vendor.objects.all(),
+    version = DynamicModelChoiceField(
+        label='Версия',
+        queryset=ApplicationVersion.objects.all(),
         required=True
     )
 
     class Meta:
         model = DeviceSoftware
-        fields = ('name', 'vendor', 'software_type', 'version', 'comments', 'tags')
+        fields = ('app', 'version', 'comments', 'tags')
 
     def __init__(self, *args, **kwargs):
         # Initialize helper selectors
         instance = kwargs.get('instance')
         initial = kwargs.get('initial', {}).copy()
         if instance:
             if type(instance.assigned_object) is Device:
@@ -108,23 +166,18 @@
             self.instance.assigned_object = None
 
 
 class DeviceSoftwareFilterForm(NetBoxModelFilterSetForm):
     model = DeviceSoftware
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
-        ('Атрибуты', ('name', 'software_type_id', 'vendor_id')),
+        ('Атрибуты', ('app',)),
         ('Устройство/ВМ', ('device_id', 'virtual_machine_id')),
     )
 
-    name = forms.CharField(
-        label='Название',
-        required=False
-    )
-
     device_id = DynamicModelMultipleChoiceField(
         label='Устройство',
         queryset=Device.objects.all(),
         required=False
     )
 
     virtual_machine_id = DynamicModelMultipleChoiceField(
```

### Comparing `netbox_software-0.2.1/netbox_software/models.py` & `netbox_software-0.2.2/netbox_software/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 from django.db import models
 from django.urls import reverse
 
 from netbox.models import NetBoxModel
 from utilities.choices import ChoiceSet
 
 
+SOFTWARE_ASSIGNMENT_MODELS = Q(
+    Q(app_label='dcim', model='device') |
+    Q(app_label='virtualization', model='virtualmachine')
+)
+
+
 class Vendor(NetBoxModel):
-    name = models.CharField(verbose_name="название", max_length=100, help_text='Укажите производителя ПО')
+    name = models.CharField(verbose_name="название", max_length=150, help_text='Укажите производителя ПО')
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
     class Meta:
         ordering = ('name',)
         verbose_name_plural = "Разработчики"
         verbose_name = "Разработчик"
 
@@ -63,27 +69,66 @@
     def get_devices_count(self):
         return DeviceSoftware.objects.filter(software_type=self).count()
 
     def get_devices(self):
         return DeviceSoftware.objects.filter(software_type=self)
 
 
-SOFTWARE_ASSIGNMENT_MODELS = Q(
-    Q(app_label='dcim', model='device') |
-    Q(app_label='virtualization', model='virtualmachine')
-)
-
-
-class DeviceSoftware(NetBoxModel):
+class Application(NetBoxModel):
     name = models.CharField(
         verbose_name="название",
         max_length=100,
         help_text='Укажите имя, которое будет отображаться для этого ПО.'
     )
 
+    software_type = models.ForeignKey(
+        to=SoftwareType,
+        verbose_name="тип ПО",
+        on_delete=models.CASCADE,
+        related_name='device_software'
+    )
+
+    vendor = models.ForeignKey(
+        to=Vendor,
+        verbose_name="Разработчик",
+        on_delete=models.CASCADE,
+        related_name='device_software'
+    )
+
+    comments = models.TextField(verbose_name="комментарий", blank=True)
+
+    class Meta:
+        ordering = ('name',)
+        verbose_name = "ПО"
+
+    def __str__(self):
+        return self.name
+
+
+class ApplicationVersion(NetBoxModel):
+    name = models.CharField(verbose_name="название", max_length=50, help_text='Укажите тип ПО')
+    comments = models.TextField(verbose_name="комментарий", blank=True)
+
+    class Meta:
+        ordering = ('name',)
+        verbose_name_plural = "Версии ПО"
+        verbose_name = "Версия ПО"
+
+    def __str__(self):
+        return self.name
+
+
+class DeviceSoftware(NetBoxModel):
+    app = models.ForeignKey(
+        to=Application,
+        verbose_name="Приложение",
+        on_delete=models.CASCADE,
+        related_name='devices'
+    )
+
     assigned_object_type = models.ForeignKey(
         to=ContentType,
         limit_choices_to=SOFTWARE_ASSIGNMENT_MODELS,
         on_delete=models.PROTECT,
         related_name='+',
         blank=True,
         null=True
@@ -94,32 +139,19 @@
         null=True
     )
     assigned_object = GenericForeignKey(
         ct_field='assigned_object_type',
         fk_field='assigned_object_id'
     )
 
-    software_type = models.ForeignKey(
-        to=SoftwareType,
-        verbose_name="тип ПО",
-        on_delete=models.CASCADE,
-        related_name='device_software'
-    )
-
-    vendor = models.ForeignKey(
-        to=Vendor,
-        verbose_name="Разработчик",
-        on_delete=models.CASCADE,
-        related_name='device_software'
-    )
-
-    version = models.CharField(
+    version = models.ForeignKey(
         verbose_name="версия",
-        max_length=50,
-        blank=True
+        to=ApplicationVersion,
+        on_delete=models.CASCADE,
+        related_name='device_app_version'
     )
 
     comments = models.TextField(
         verbose_name="комментарий",
         blank=True
     )
 
@@ -142,67 +174,8 @@
     def get_devices(self):
         return DeviceSoftware.objects.filter(vendor=self.vendor).count()
 
     def get_software(self):
         return list(DeviceSoftware.objects.filter(vendor=self.vendor))
 
     def get_software_count(self):
-        return DeviceSoftware.objects.filter(name=self.name, version=self.version).count()
-
-
-# class VirtualMachineSoftware(NetBoxModel):
-#     name = models.CharField(
-#         verbose_name="название",
-#         max_length=100,
-#         help_text='Укажите имя, которое будет отображаться для этого ПО.'
-#     )
-#
-#     virtual_machine = models.ForeignKey(
-#         verbose_name="виртуальая машина",
-#         to='virtualization.VirtualMachine',
-#         on_delete=models.CASCADE,
-#         related_name='software'
-#     )
-#
-#     software_type = models.ForeignKey(
-#         to=SoftwareType,
-#         verbose_name="тип ПО",
-#         on_delete=models.CASCADE,
-#         related_name='vm_software'
-#     )
-#
-#     vendor = models.ForeignKey(
-#         to=Vendor,
-#         verbose_name="Разработчик",
-#         on_delete=models.CASCADE,
-#         related_name='vm_software'
-#     )
-#
-#     version = models.CharField(
-#         verbose_name="версия",
-#         max_length=50,
-#         blank=True
-#     )
-#
-#     comments = models.TextField(
-#         verbose_name="комментарий",
-#         blank=True
-#     )
-#
-#     class Meta:
-#         ordering = ('name',)
-#         verbose_name_plural = "ПО виртуальных машин"
-#         verbose_name = "ПО виртуальной машины"
-#
-#     def __str__(self):
-#         return self.name
-#
-#     def get_absolute_url(self):
-#         return reverse('plugins:netbox_software:virtualmachinesoftware', args=[self.pk])
-#
-#     def get_software_count(self):
-#         return DeviceSoftware.objects.filter(name=self.name, version=self.version).count() + \
-#             VirtualMachineSoftware.objects.filter(name=self.name, version=self.version).count()
-#
-#     def get_software(self):
-#         return list(DeviceSoftware.objects.filter(vendor=self.vendor)) + list(
-#             VirtualMachineSoftware.objects.filter(vendor=self.vendor))
+        return DeviceSoftware.objects.filter(app=self.app).count()
```

### Comparing `netbox_software-0.2.1/netbox_software/navigation.py` & `netbox_software-0.2.2/netbox_software/navigation.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     def name(self):
         return self._name
 
 
 if plugin_settings.get('enable_navigation_menu'):
 
     menuitem = []
-
     # Add a menu item for Device software if enabled
     if plugin_settings.get('enable_device_software'):
         menuitem.append(
             PluginMenuItem(
                 link='plugins:netbox_software:devicesoftware_list',
                 link_text='ПО устройств',
                 buttons=[PluginMenuButton(
@@ -30,15 +29,14 @@
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
-
         menuitem.append(
             PluginMenuItem(
                 link='plugins:netbox_software:softwaretype_list',
                 link_text='Типы ПО',
                 buttons=[PluginMenuButton(
                     link='plugins:netbox_software:softwaretype_add',
                     title='Создать',
@@ -57,14 +55,27 @@
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
+        menuitem.append(
+            PluginMenuItem(
+                link='plugins:netbox_software:app_list',
+                link_text='ПО',
+                buttons=[PluginMenuButton(
+                    link='plugins:netbox_software:app_add',
+                    title='Создать',
+                    icon_class='mdi mdi-plus-thick',
+                    color=ButtonColorChoices.GREEN
+                )],
+                permissions=['dcim.view_device']
+            )
+        )
 
     # If we are using NB 3.4.0+ display the new top level navigation option
     if settings.VERSION >= '3.4.0':
         menu = MyPluginMenu(
             name='SoftPl',
             label='Установленное ПО',
             groups=(
```

### Comparing `netbox_software-0.2.1/netbox_software/tables.py` & `netbox_software-0.2.2/netbox_software/tables.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 import django_tables2 as tables
 
 from netbox.tables import NetBoxTable, columns
 from tenancy.tables import TenantColumn
-from .models import DeviceSoftware, Vendor, SoftwareType
+from .models import DeviceSoftware, Vendor, SoftwareType, ApplicationVersion, Application
 
 SOFTWARE_TYPE_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:softwaretype' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
 VENDOR_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:vendor' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
+APPLICATION_TYPE_SOFTWARE_LINK = """
+{% if record %}
+    <a href="{% url 'plugins:netbox_software:apptype' pk=record.pk %}">{% firstof record.name record.name %}</a>
+{% endif %}
+"""
+
+APPLICATION_SOFTWARE_LINK = """
+{% if record %}
+    <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.name record.app %}</a>
+{% endif %}
+"""
+
 DEVICE_SOFTWARE_LINK = """
 {% if record %}
-    <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.name record.name %}</a>
+    <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.app record.app %}</a>
 {% endif %}
 """
 
 SOFTWARE_ASSIGN_LINK = """
 <a href="{% url ''plugins:netbox_software:devicesoftware' pk=record.pk %}?{% if request.GET.device_soft %}device={{ request.GET.device_soft }}{% elif request.GET.vm_soft %}vm_soft={{ request.GET.vm_soft }}{% endif %}&return_url={{ request.GET.return_url }}">{{ record }}</a>
 """
 
+
 class VendorTable(NetBoxTable):
     name = tables.TemplateColumn(template_code=VENDOR_SOFTWARE_LINK)
 
     class Meta(NetBoxTable.Meta):
         model = Vendor
         fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
         default_columns = ('name',)
@@ -40,22 +53,50 @@
 
     class Meta(NetBoxTable.Meta):
         model = SoftwareType
         fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
         default_columns = ('name',)
 
 
-class DeviceSoftwareTable(NetBoxTable):
-    name = tables.TemplateColumn(template_code=DEVICE_SOFTWARE_LINK)
+class ApplicationVersionTable(NetBoxTable):
+    name = tables.TemplateColumn(template_code=APPLICATION_TYPE_SOFTWARE_LINK)
+
+    class Meta(NetBoxTable.Meta):
+        model = ApplicationVersion
+        fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
+        default_columns = ('name',)
+
+
+class ApplicationTable(NetBoxTable):
+    name = tables.TemplateColumn(template_code=APPLICATION_SOFTWARE_LINK)
     software_type = tables.Column(
         linkify=True
     )
     vendor = tables.Column(
         linkify=True
     )
+    tags = columns.TagColumn(
+        url_name='dcim:sitegroup_list'
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = Application
+        fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'comments', 'actions', 'created', 'last_updated',
+                  'tags')
+        default_columns = ('name', 'software_type', 'vendor')
+
+
+class DeviceSoftwareTable(NetBoxTable):
+    # name = tables.TemplateColumn(template_code=DEVICE_SOFTWARE_LINK)
+    app = tables.Column(
+        linkify=True
+    )
+    version = tables.Column(
+        linkify=True
+    )
     device = tables.Column(
         linkify=True
     )
     assigned_object = tables.Column(
         linkify=True,
         orderable=False,
         verbose_name='Устройство'
@@ -63,32 +104,33 @@
 
     tags = columns.TagColumn(
         url_name='dcim:sitegroup_list'
     )
 
     class Meta(NetBoxTable.Meta):
         model = DeviceSoftware
-        fields = ('pk', 'id', 'name', 'software_type', 'vendor', 'version', 'comments', 'actions',
-                  'created', 'last_updated', 'tags')
-        default_columns = ('name', 'software_type', 'assigned_object', 'vendor', 'tags')
+        fields = ('pk', 'id', 'app', 'version', 'comments', 'actions', 'created', 'last_updated', 'tags')
+        default_columns = ('app', 'software_type', 'assigned_object', 'version', 'tags')
 
 
 class DeviceSoftwareAssignTable(NetBoxTable):
-    name = tables.TemplateColumn(
-        template_code=SOFTWARE_ASSIGN_LINK,
-        verbose_name='ПО'
+    app = tables.Column(
+        orderable=False
+    )
+    version = tables.Column(
+        orderable=False
     )
     status = columns.ChoiceFieldColumn()
     assigned_object = tables.Column(
         orderable=False
     )
 
     class Meta(NetBoxTable.Meta):
         model = DeviceSoftware
-        fields = ('name', 'software_type', 'vendor', 'version', 'assigned_object', 'description')
+        fields = ('app', 'version', 'assigned_object', 'description')
         exclude = ('id', )
         orderable = False
 
 
 class AssignedDeviceSoftwareTable(NetBoxTable):
     """
     List DeviceSoftware assigned to an object.
```

### Comparing `netbox_software-0.2.1/netbox_software/template_content.py` & `netbox_software-0.2.2/netbox_software/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,37 +5,37 @@
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">ПО устройства</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Название ПО</th>
-              <td>{{ object.name|placeholder }}</td>
+              <td>{{ object.app|placeholder }}</td>
             </tr>
             <tr>
                 <th scope="row">Устройство</th>
                 <td>
                   {% if object.assigned_object %}
                     {{ object.assigned_object|linkify }}
                   {% else %}
                     {{ ''|placeholder }}
                   {% endif %}
                 </td>
             </tr>
             <tr>
               <th scope="row">Тип ПО</th>
-              <td>{{ object.software_type }}</td>
+              <td>{{ object.app.software_type }}</td>
             </tr>
             <tr>
               <th scope="row">Установлено</th>
               <td> на {{ object.get_software_count }} хостах</td>
             </tr>
             <tr>
               <th scope="row">Разработчик</th>
-              <td>{{ object.vendor }}</tr>
+              <td>{{ object.app.vendor }}</tr>
             <tr>
               <th scope="row">Версия</th>
               <td>{{ object.version|placeholder }}</tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
 ** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
-ÐÐ°Ð·Ð²Ð°Ð�{{ object.name|placeholder }}
+ÐÐ°Ð·Ð²Ð°Ð�{{ object.app|placeholder }}
                        {% if object.assigned_object %} {
 Ð£ÑÑÑÐ¾Ð�{ object.assigned_object|linkify }} {% else %} {
                        { ''|placeholder }} {% endif %}
-Ð¢Ð¸Ð¿ ÐÐ  {{ object.software_type }}
+Ð¢Ð¸Ð¿ ÐÐ  {{ object.app.software_type }}
 Ð£ÑÑÐ°Ð½Ð�Ð½Ð° {{ object.get_software_count }} ÑÐ¾ÑÑÐ°Ñ
-Ð Ð°Ð·ÑÐ°Ð�{{ object.vendor }}º
+Ð Ð°Ð·ÑÐ°Ð�{{ object.app.vendor }}
 ÐÐµÑÑÐ¸Ñ�{{ object.version|placeholder }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /p  {% extends 'generic/object_edit.html' %}
 {% load static %}
 {% load form_helpers %}
 {% load helpers %}
 
 {% block form %}
     <div class="field-group my-5">
-      {% render_field form.name %}
+      {% render_field form.app %}
 
       <div class="field-group my-1">
-        {% render_field form.software_type %}
-        {% render_field form.vendor %}
+        {% render_field form.app.software_type %}
+        {% render_field form.app.vendor %}
         {% render_field form.version %}
         <div class="field-group my-5">
         <div class="row mb-2">
           <h5 class="offset-sm-3">Назначение ПО</h5>
         </div>
         <div class="row mb-2">
           <div class="offset-sm-3">
```

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
             <th>Название</th>
             <th>версия</th>
             <th></th>
         </tr>
         {% for software in device_software %}
         <tr>
             <td>
-                {{ software.name }}
+                {{ software.app.name }}
             </td>
-            <td>{{ software.version }}</td>
+            <td>{{ software.app.version }}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:devicesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
                   <a href="{% url 'plugins:netbox_software:devicesoftware_edit' pk=software.pk %}?return_url=
                   {% url 'dcim:device' pk=object.pk %}" class="btn btn-warning btn-sm lh-1" title="Редактировать">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load helpers %}
 ** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° {% if device_software %} (Ð²ÑÐµÐ³Ð¾:_{
 {_soft_count_}}) {% endif %} **
 {% if device_software %}
-ÐÐ°Ð·Ð²Ð°Ð²ÐµÑÑÐ¸Ñ
-{{ software.name }} {{ software.version }}
+ÐÐ°Ð·Ð²Ð°Ð½Ð²ÐµÑÑÐ¸Ñ
+{{ software.app.name }} {{ software.app.version }}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
  ÐÑÐµ_ÐÐ_ÑÐ¾ÑÑÐ°
```

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.1/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.1/PKG-INFO` & `netbox_software-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,15 +27,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.1          |
+|     3.2+       | 0.2.2          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

