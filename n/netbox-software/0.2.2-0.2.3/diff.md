# Comparing `tmp/netbox_software-0.2.2.tar.gz` & `tmp/netbox_software-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.2.2.tar", max compression
+gzip compressed data, was "netbox_software-0.2.3.tar", max compression
```

## Comparing `netbox_software-0.2.2.tar` & `netbox_software-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.2/LICENSE
--rw-r--r--   0        0        0     3420 2023-07-13 08:07:13.677335 netbox_software-0.2.2/README.md
--rw-r--r--   0        0        0      640 2023-07-13 08:07:13.665335 netbox_software-0.2.2/netbox_software/__init__.py
--rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.2/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.2/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.2/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.2/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1357 2023-07-13 08:04:55.515077 netbox_software-0.2.2/netbox_software/api/views.py
--rw-r--r--   0        0        0     4349 2023-07-13 08:04:55.507077 netbox_software-0.2.2/netbox_software/filtersets.py
--rw-r--r--   0        0        0     5698 2023-07-13 08:06:01.104149 netbox_software-0.2.2/netbox_software/forms.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.2/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     5415 2023-07-13 07:37:44.876577 netbox_software-0.2.2/netbox_software/models.py
--rw-r--r--   0        0        0     3102 2023-07-13 07:37:44.872576 netbox_software-0.2.2/netbox_software/navigation.py
--rw-r--r--   0        0        0     1162 2023-07-13 07:37:44.888577 netbox_software-0.2.2/netbox_software/search.py
--rw-r--r--   0        0        0     4494 2023-07-13 07:37:44.904577 netbox_software-0.2.2/netbox_software/tables.py
--rw-r--r--   0        0        0     5647 2023-07-12 12:45:38.932973 netbox_software-0.2.2/netbox_software/template_content.py
--rw-r--r--   0        0        0      954 2023-07-13 07:41:42.248256 netbox_software-0.2.2/netbox_software/templates/netbox_software/application.html
--rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.2/netbox_software/templates/netbox_software/application_edit.html
--rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.2/netbox_software/templates/netbox_software/applicationversion.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/applicationversion_edit.html
--rw-r--r--   0        0        0     1613 2023-07-13 07:37:44.912577 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0     2201 2023-07-13 07:37:44.872576 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2395 2023-07-13 07:50:20.332738 netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.2/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.2.2/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1685 2023-07-12 09:48:10.295965 netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     3416 2023-07-13 07:37:44.900577 netbox_software-0.2.2/netbox_software/urls.py
--rw-r--r--   0        0        0     5243 2023-07-13 07:37:44.864576 netbox_software-0.2.2/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-07-13 08:07:13.669335 netbox_software-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-13 12:43:26.715969 netbox_software-0.2.3/README.md
+-rw-r--r--   0        0        0      534 2023-07-13 12:43:26.707969 netbox_software-0.2.3/netbox_software/__init__.py
+-rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.3/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.3/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.3/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.3/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1357 2023-07-13 10:00:09.172753 netbox_software-0.2.3/netbox_software/api/views.py
+-rw-r--r--   0        0        0     4830 2023-07-13 12:13:31.207506 netbox_software-0.2.3/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     6062 2023-07-13 11:54:22.813357 netbox_software-0.2.3/netbox_software/forms.py
+-rw-r--r--   0        0        0     6229 2023-07-13 09:59:12.131848 netbox_software-0.2.3/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.3/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     6692 2023-07-13 11:44:23.611927 netbox_software-0.2.3/netbox_software/models.py
+-rw-r--r--   0        0        0     3117 2023-07-13 10:15:17.055009 netbox_software-0.2.3/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1216 2023-07-13 12:12:09.530212 netbox_software-0.2.3/netbox_software/search.py
+-rw-r--r--   0        0        0     4452 2023-07-13 11:47:12.302581 netbox_software-0.2.3/netbox_software/tables.py
+-rw-r--r--   0        0        0     5647 2023-07-13 08:14:35.344556 netbox_software-0.2.3/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1435 2023-07-13 11:02:11.516704 netbox_software-0.2.3/netbox_software/templates/netbox_software/application.html
+-rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.3/netbox_software/templates/netbox_software/application_edit.html
+-rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion_edit.html
+-rw-r--r--   0        0        0     1704 2023-07-13 10:48:52.323169 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2108 2023-07-13 10:27:29.270544 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2477 2023-07-13 10:50:18.520568 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.3/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0     1116 2023-07-13 11:11:57.226346 netbox_software-0.2.3/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1691 2023-07-13 11:40:24.952229 netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     3525 2023-07-13 10:14:12.001988 netbox_software-0.2.3/netbox_software/urls.py
+-rw-r--r--   0        0        0     5243 2023-07-13 10:00:09.160753 netbox_software-0.2.3/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-07-13 12:43:26.723969 netbox_software-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.3/PKG-INFO
```

### Comparing `netbox_software-0.2.2/LICENSE` & `netbox_software-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/README.md` & `netbox_software-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.2          |
+|     3.2+       | 0.2.3          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

### Comparing `netbox_software-0.2.2/netbox_software/__init__.py` & `netbox_software-0.2.3/netbox_software/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.2.2'
+    version = '0.2.3'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
-        # "enable_virtual-machine_software": True,
         "device_software_location": "left",
-        # "virtual-machine_software_location": "left",
     }
 
 
 config = NetboxSoftware
```

### Comparing `netbox_software-0.2.2/netbox_software/admin.py` & `netbox_software-0.2.3/netbox_software/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/api/serializers.py` & `netbox_software-0.2.3/netbox_software/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/api/views.py` & `netbox_software-0.2.3/netbox_software/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/filtersets.py` & `netbox_software-0.2.3/netbox_software/filtersets.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,31 +63,31 @@
             Q(name__icontains=value) |
             Q(comments__icontains=value)
         )
 
 
 class DeviceSoftwareFilterSet(NetBoxModelFilterSet):
     app = MultiValueCharFilter(
-        queryset=Application.objects.all(),
+        method='filter_app',
         field_name='name',
-        lookup_expr='in',
         label=_('App (name)'),
     )
     app_id = MultiValueNumberFilter(
-        queryset=Application.objects.all(),
+        method='filter_app',
+        field_name='pk',
         label=_('App (ID)'),
     )
     version = MultiValueCharFilter(
-        queryset=ApplicationVersion.objects.all(),
+        method='filter_version',
         field_name='name',
-        lookup_expr='in',
         label=_('Version (name)'),
     )
     version_id = MultiValueNumberFilter(
-        queryset=ApplicationVersion.objects.all(),
+        method='filter_version',
+        field_name='pk',
         label=_('Version (ID)'),
     )
 
     device = MultiValueCharFilter(
         method='filter_device',
         field_name='name',
         label=_('Device (name)'),
@@ -106,22 +106,38 @@
         method='filter_virtual_machine',
         field_name='pk',
         label=_('Virtual machine (ID)'),
     )
 
     class Meta:
         model = DeviceSoftware
-        fields = ('id', 'app')
+        fields = ('id',)
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
-            Q(app__icontains=value) |
-            Q(version__icontains=value)
+            Q(app__name__icontains=value) |
+            Q(version__name__icontains=value)
+        )
+
+    def filter_app(self, queryset, name, value):
+        apps = Application.objects.filter(**{'{}__in'.format(name): value})
+        if not apps.exists():
+            return queryset.none()
+        return queryset.filter(
+            app__in=apps
+        )
+
+    def filter_version(self, queryset, name, value):
+        versions = ApplicationVersion.objects.filter(**{'{}__in'.format(name): value})
+        if not versions.exists():
+            return queryset.none()
+        return queryset.filter(
+            version__in=versions
         )
 
     def filter_device(self, queryset, name, value):
         devices = Device.objects.filter(**{'{}__in'.format(name): value})
         if not devices.exists():
             return queryset.none()
         devices_ids = []
```

### Comparing `netbox_software-0.2.2/netbox_software/forms.py` & `netbox_software-0.2.3/netbox_software/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,29 +166,39 @@
             self.instance.assigned_object = None
 
 
 class DeviceSoftwareFilterForm(NetBoxModelFilterSetForm):
     model = DeviceSoftware
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
-        ('Атрибуты', ('app',)),
+        ('Атрибуты', ('app_id', 'version_id', 'software_type_id', 'vendor_id')),
         ('Устройство/ВМ', ('device_id', 'virtual_machine_id')),
     )
 
     device_id = DynamicModelMultipleChoiceField(
         label='Устройство',
         queryset=Device.objects.all(),
         required=False
     )
 
     virtual_machine_id = DynamicModelMultipleChoiceField(
         label='ВМ',
         queryset=VirtualMachine.objects.all(),
         required=False
     )
+    app_id = forms.ModelMultipleChoiceField(
+        label='Приложение',
+        queryset=Application.objects.all(),
+        required=False
+    )
+    version_id = forms.ModelMultipleChoiceField(
+        label='Версия',
+        queryset=ApplicationVersion.objects.all(),
+        required=False
+    )
 
     software_type_id = forms.ModelMultipleChoiceField(
         label='Тип',
         queryset=SoftwareType.objects.all(),
         required=False
     )
     vendor_id = forms.ModelMultipleChoiceField(
```

### Comparing `netbox_software-0.2.2/netbox_software/models.py` & `netbox_software-0.2.3/netbox_software/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,36 +37,59 @@
         devices = []
         dev_softs = DeviceSoftware.objects.filter(vendor=self)
         for soft in dev_softs:
             devices.append(soft.device.name)
         return DeviceSoftware.objects.filter(vendor=self)
 
     def get_software_count(self):
-        return DeviceSoftware.objects.filter(vendor=self).count()
+        return DeviceSoftware.objects.filter(app__vendor=self).values('app__name', 'version__name').distinct().count()
+        # result = []
+        # # data = DeviceSoftware.objects.filter(app__vendor=self).values('app__name', 'version__name').distinct()
+        #
+        # keys = []
+        # for item in data:
+        #     # if item['app__name'] in keys:
+        #     #     continue
+        #     keys.append(item['app__name'])
+        #     result.append([item['app__name'],item['version__name']])
+        # return len(result)
 
     def get_software(self):
-        soft_list = []
-        dev_softs = DeviceSoftware.objects.filter(vendor=self)
-        for soft in dev_softs:
-            soft_list.append(soft)
-        return soft_list
+        # return DeviceSoftware.objects.filter(app__vendor=self).distinct()
+        result = []
+        data = DeviceSoftware.objects.filter(app__vendor=self).distinct()
+        keys = {}
+        for item in data:
+            if item.app.name in keys.keys() and item.version.name in keys[item.app.name]['versions']:
+                continue
+            if item.app.name in keys.keys():
+                keys[item.app.name]['versions'].append(item.version.name)
+                result.append(item)
+                continue
+            keys[item.app.name] = {'versions': [item.version.name]}
+
+            result.append(item)
+        return result
 
 
 class SoftwareType(NetBoxModel):
     name = models.CharField(verbose_name="название", max_length=100, help_text='Укажите тип ПО')
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
     class Meta:
         ordering = ('name',)
         verbose_name_plural = "Типы ПО"
         verbose_name = "Тип ПО"
 
     def __str__(self):
         return self.name
 
+    def get_apps(self):
+        return Application.objects.filter(software_type=self)
+
     def get_absolute_url(self):
         return reverse('plugins:netbox_software:softwaretype', args=[self.pk])
 
     def get_devices_count(self):
         return DeviceSoftware.objects.filter(software_type=self).count()
 
     def get_devices(self):
@@ -80,33 +103,37 @@
         help_text='Укажите имя, которое будет отображаться для этого ПО.'
     )
 
     software_type = models.ForeignKey(
         to=SoftwareType,
         verbose_name="тип ПО",
         on_delete=models.CASCADE,
-        related_name='device_software'
+        related_name='app_soft_types'
     )
 
     vendor = models.ForeignKey(
         to=Vendor,
         verbose_name="Разработчик",
         on_delete=models.CASCADE,
-        related_name='device_software'
+        related_name='app_vendor'
     )
 
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
     class Meta:
         ordering = ('name',)
-        verbose_name = "ПО"
+        verbose_name_plural = "Приложения"
+        verbose_name = "Приложение"
 
     def __str__(self):
         return self.name
 
+    def get_all_versions(self):
+        return list(set(DeviceSoftware.objects.filter(app=self).values_list('version__name', flat=True)))
+
 
 class ApplicationVersion(NetBoxModel):
     name = models.CharField(verbose_name="название", max_length=50, help_text='Укажите тип ПО')
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
     class Meta:
         ordering = ('name',)
@@ -143,29 +170,29 @@
         fk_field='assigned_object_id'
     )
 
     version = models.ForeignKey(
         verbose_name="версия",
         to=ApplicationVersion,
         on_delete=models.CASCADE,
-        related_name='device_app_version'
+        related_name='devices_with_version'
     )
 
     comments = models.TextField(
         verbose_name="комментарий",
         blank=True
     )
 
     class Meta:
-        ordering = ('name',)
+        ordering = ('app',)
         verbose_name_plural = "ПО устройств"
         verbose_name = "ПО устройства"
 
     def __str__(self):
-        return self.name
+        return f'{self.app.name} v{self.version.name}'
 
     def to_objectchange(self, action):
         objectchange = super().to_objectchange(action)
         objectchange.related_object = self.assigned_object
         return objectchange
 
     def get_absolute_url(self):
@@ -174,8 +201,8 @@
     def get_devices(self):
         return DeviceSoftware.objects.filter(vendor=self.vendor).count()
 
     def get_software(self):
         return list(DeviceSoftware.objects.filter(vendor=self.vendor))
 
     def get_software_count(self):
-        return DeviceSoftware.objects.filter(app=self.app).count()
+        return DeviceSoftware.objects.filter(app=self.app, version=self.version).count()
```

### Comparing `netbox_software-0.2.2/netbox_software/navigation.py` & `netbox_software-0.2.3/netbox_software/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
         menuitem.append(
             PluginMenuItem(
-                link='plugins:netbox_software:app_list',
+                link='plugins:netbox_software:application_list',
                 link_text='ПО',
                 buttons=[PluginMenuButton(
-                    link='plugins:netbox_software:app_add',
+                    link='plugins:netbox_software:application_add',
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
                     color=ButtonColorChoices.GREEN
                 )],
                 permissions=['dcim.view_device']
             )
         )
@@ -81,10 +81,9 @@
             groups=(
                 ('', menuitem),
             ),
             icon_class='mdi mdi-microsoft-xbox-controller-off'
         )
 
     else:
-
         # Fall back to pre 3.4 navigation option
         menu_items = menuitem
```

### Comparing `netbox_software-0.2.2/netbox_software/search.py` & `netbox_software-0.2.3/netbox_software/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,14 @@
             ("name", 100),
             ("comments", 5000),
         )
 
     class DeviceSoftwareIndex(SearchIndex):
         model = DeviceSoftware
         fields = (
-            ("name", 100),
-            ("version", 500),
+            ("app__name", 100),
+            ("version__name", 500),
             ("comments", 5000),
         )
 
     # Register indexes
-    indexes = [VendorIndex, SoftwareTypeIndex, DeviceSoftwareIndex]
+    indexes = [VendorIndex, SoftwareTypeIndex, ApplicationIndex, ApplicationVersionIndex, DeviceSoftwareIndex]
```

### Comparing `netbox_software-0.2.2/netbox_software/tables.py` & `netbox_software-0.2.3/netbox_software/tables.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 VENDOR_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:vendor' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
-APPLICATION_TYPE_SOFTWARE_LINK = """
+APPLICATION_VERSION_SOFTWARE_LINK = """
 {% if record %}
-    <a href="{% url 'plugins:netbox_software:apptype' pk=record.pk %}">{% firstof record.name record.name %}</a>
+    <a href="{% url 'plugins:netbox_software:applicationversion' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
 APPLICATION_SOFTWARE_LINK = """
 {% if record %}
-    <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.name record.app %}</a>
+    <a href="{% url 'plugins:netbox_software:application' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
 DEVICE_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.app record.app %}</a>
 {% endif %}
@@ -54,15 +54,15 @@
     class Meta(NetBoxTable.Meta):
         model = SoftwareType
         fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
         default_columns = ('name',)
 
 
 class ApplicationVersionTable(NetBoxTable):
-    name = tables.TemplateColumn(template_code=APPLICATION_TYPE_SOFTWARE_LINK)
+    name = tables.TemplateColumn(template_code=APPLICATION_VERSION_SOFTWARE_LINK)
 
     class Meta(NetBoxTable.Meta):
         model = ApplicationVersion
         fields = ('pk', 'id', 'name', 'comments', 'actions', 'created', 'last_updated',)
         default_columns = ('name',)
 
 
@@ -89,17 +89,14 @@
     # name = tables.TemplateColumn(template_code=DEVICE_SOFTWARE_LINK)
     app = tables.Column(
         linkify=True
     )
     version = tables.Column(
         linkify=True
     )
-    device = tables.Column(
-        linkify=True
-    )
     assigned_object = tables.Column(
         linkify=True,
         orderable=False,
         verbose_name='Устройство'
     )
 
     tags = columns.TagColumn(
@@ -131,17 +128,17 @@
         orderable = False
 
 
 class AssignedDeviceSoftwareTable(NetBoxTable):
     """
     List DeviceSoftware assigned to an object.
     """
-    name = tables.Column(
+    app = tables.Column(
         linkify=True,
         verbose_name='ПО'
     )
 
     class Meta(NetBoxTable.Meta):
         model = DeviceSoftware
-        fields = ('name', 'software_type', 'vendor', 'version', 'assigned_object', 'description')
+        fields = ('app', 'software_type', 'vendor', 'version', 'assigned_object', 'description')
         exclude = ('id', )
```

### Comparing `netbox_software-0.2.2/netbox_software/template_content.py` & `netbox_software-0.2.3/netbox_software/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/application_edit.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/application_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/applicationversion.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,37 @@
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">ПО устройства</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Название ПО</th>
-              <td>{{ object.app|placeholder }}</td>
+              <td><a href="{% url 'plugins:netbox_software:application' pk=object.app.pk %}">{{ object.app|linkify }}</a></td>
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
-              <td>{{ object.app.software_type }}</td>
+              <td>{{ object.app.software_type|linkify }}</td>
             </tr>
             <tr>
               <th scope="row">Установлено</th>
               <td> на {{ object.get_software_count }} хостах</td>
             </tr>
             <tr>
               <th scope="row">Разработчик</th>
-              <td>{{ object.app.vendor }}</tr>
+              <td>{{ object.app.vendor|linkify }}</tr>
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
-ÐÐ°Ð·Ð²Ð°Ð�{{ object.app|placeholder }}
+ÐÐ°Ð·Ð²Ð°Ð�{{_object.app|linkify_}}
                        {% if object.assigned_object %} {
 Ð£ÑÑÑÐ¾Ð�{ object.assigned_object|linkify }} {% else %} {
                        { ''|placeholder }} {% endif %}
-Ð¢Ð¸Ð¿ ÐÐ  {{ object.app.software_type }}
+Ð¢Ð¸Ð¿ ÐÐ  {{ object.app.software_type|linkify }}
 Ð£ÑÑÐ°Ð½Ð�Ð½Ð° {{ object.get_software_count }} ÑÐ¾ÑÑÐ°Ñ
-Ð Ð°Ð·ÑÐ°Ð�{{ object.app.vendor }}
+Ð Ð°Ð·ÑÐ°Ð�{{ object.app.vendor|linkify }}
 ÐÐµÑÑÐ¸Ñ�{{ object.version|placeholder }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 {% load helpers %}
 
 {% block form %}
     <div class="field-group my-5">
       {% render_field form.app %}
 
       <div class="field-group my-1">
-        {% render_field form.app.software_type %}
-        {% render_field form.app.vendor %}
         {% render_field form.version %}
         <div class="field-group my-5">
         <div class="row mb-2">
           <h5 class="offset-sm-3">Назначение ПО</h5>
         </div>
         <div class="row mb-2">
           <div class="offset-sm-3">
```

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
             <th>Название</th>
             <th>версия</th>
             <th></th>
         </tr>
         {% for software in device_software %}
         <tr>
             <td>
-                {{ software.app.name }}
+                <a href="{% url 'plugins:netbox_software:application' pk=software.app.pk %}">{{ software.app.name }}</a>
             </td>
-            <td>{{ software.app.version }}</td>
+            <td>{{ software.version.name }}</td>
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
 ÐÐ°Ð·Ð²Ð°Ð½Ð²ÐµÑÑÐ¸Ñ
-{{ software.app.name }} {{ software.app.version }}
+{{_software.app.name_}} {{ software.version.name }}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
  ÐÑÐµ_ÐÐ_ÑÐ¾ÑÑÐ°
```

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor.html`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             </tr>
             <tr>
               <th scope="row">Приложений всего</th>
               <td> {{ object.get_software_count }}</td>
               <td></td>
             </tr>
             <tr>
-              <th scope="row">Приложений:</th>
+              <th scope="row">Приложения:</th>
               <table>
                 {% if object.get_software %}
                   {% for soft in object.get_software %}
                     <tr>
-                      <th scope="row"><a href="{% url 'plugins:netbox_software:devicesoftware' pk=soft.pk %}">| {{ soft.name }}</a></th>
+                      <th scope="row"><a href="{% url 'plugins:netbox_software:devicesoftware' pk=soft.pk %}">{{ soft.app.name }}</a></th>
                       <td></td>
-                      <td> | Версия: {{ soft.version }} |</td>
+                      <td> | Версия: {{ soft.version.name }} </td>
                     </tr>
                   {% endfor %}
                 {% else %}
                 <tr>
                   <th scope="row"></th>
                   <td>нет установленных приложений </td>
                   <td></td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
 ** Ð Ð°Ð·ÑÐ°Ð±Ð¾ÑÑÐ¸Ðº **
 ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ð�{{ object.name|placeholder }}
 ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ�{{ object.get_software_count }}
 Ð²ÑÐµÐ³Ð¾
-ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ð¹:
-|_{{_soft.name_}}                                                            | ÐÐµÑÑÐ¸Ñ: {{ soft.version }} |
+ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ñ:
+{{_soft.app.name_}}                                                          | ÐÐµÑÑÐ¸Ñ: {{ soft.version.name }}
                                Ð½ÐµÑ ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð½ÑÑ
                                Ð¿ÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ð¹
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.2.2/netbox_software/urls.py` & `netbox_software-0.2.3/netbox_software/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,27 +24,28 @@
         'model': models.SoftwareType
     }),
 
     # ApplicationVersion
     path('applicationversion/', views.ApplicationVersionListView.as_view(), name='applicationversion_list'),
     path('applicationversion/add/', views.ApplicationVersionEditView.as_view(), name='applicationversion_add'),
     path('applicationversion/<int:pk>/', views.ApplicationVersionView.as_view(), name='applicationversion'),
-    path('applicationversion/<int:pk>/edit/', views.ApplicationVersionEditView.as_view(), name='applicationversion_edit'),
-    path('applicationversion/<int:pk>/delete/', views.ApplicationVersionDeleteView.as_view(), name='applicationversion_delete'),
-    path('applicationversion/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='applicationversion_changelog', kwargs={
-        'model': models.ApplicationVersion
-    }),
+    path('applicationversion/<int:pk>/edit/', views.ApplicationVersionEditView.as_view(),
+         name='applicationversion_edit'),
+    path('applicationversion/<int:pk>/delete/', views.ApplicationVersionDeleteView.as_view(),
+         name='applicationversion_delete'),
+    path('applicationversion/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='applicationversion_changelog',
+         kwargs={'model': models.ApplicationVersion}),
 
     # App
-    path('app/', views.ApplicationListView.as_view(), name='app_list'),
-    path('app/add/', views.ApplicationEditView.as_view(), name='app_add'),
-    path('app/<int:pk>/', views.ApplicationView.as_view(), name='app'),
-    path('app/<int:pk>/edit/', views.ApplicationEditView.as_view(), name='app_edit'),
-    path('app/<int:pk>/delete/', views.ApplicationDeleteView.as_view(), name='app_delete'),
-    path('app/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='app_changelog', kwargs={
+    path('application/', views.ApplicationListView.as_view(), name='application_list'),
+    path('application/add/', views.ApplicationEditView.as_view(), name='application_add'),
+    path('application/<int:pk>/', views.ApplicationView.as_view(), name='application'),
+    path('application/<int:pk>/edit/', views.ApplicationEditView.as_view(), name='application_edit'),
+    path('application/<int:pk>/delete/', views.ApplicationDeleteView.as_view(), name='application_delete'),
+    path('application/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='application_changelog', kwargs={
         'model': models.Application
     }),
 
     # DeviceSoftware
     path('device-software/', views.DeviceSoftwareListView.as_view(), name='devicesoftware_list'),
     path('device-software/add/', views.DeviceSoftwareEditView.as_view(), name='devicesoftware_add'),
     path('device-software/<int:pk>/', views.DeviceSoftwareView.as_view(), name='devicesoftware'),
```

### Comparing `netbox_software-0.2.2/netbox_software/views.py` & `netbox_software-0.2.3/netbox_software/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.2/PKG-INFO` & `netbox_software-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.2.2
+Version: 0.2.3
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
-|     3.2+       | 0.2.2          |
+|     3.2+       | 0.2.3          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

