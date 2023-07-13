# Comparing `tmp/pih-1.46001.tar.gz` & `tmp/pih-1.46231.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.46001.tar", last modified: Tue Jul 11 06:56:24 2023, max compression
+gzip compressed data, was "pih-1.46231.tar", last modified: Thu Jul 13 05:06:15 2023, max compression
```

## Comparing `pih-1.46001.tar` & `pih-1.46231.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 06:56:23.072092 pih-1.46001/
--rw-rw-rw-   0        0        0      261 2023-07-11 06:56:24.712780 pih-1.46001/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 06:56:24.275210 pih-1.46001/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.46001/pih/__init__.py
--rw-rw-rw-   0        0        0    19633 2023-07-11 03:15:46.000000 pih-1.46001/pih/collection.py
--rw-rw-rw-   0        0        0    55119 2023-07-11 04:21:24.000000 pih-1.46001/pih/console_api.py
--rw-rw-rw-   0        0        0   106061 2023-07-11 03:57:38.000000 pih-1.46001/pih/const.py
--rw-rw-rw-   0        0        0   299535 2023-07-11 06:56:13.000000 pih-1.46001/pih/pih.py
--rw-rw-rw-   0        0        0    24689 2023-07-09 01:49:27.000000 pih-1.46001/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.46001/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.46001/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.46001/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6368 2023-07-11 03:24:37.000000 pih-1.46001/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.46001/pih/service_example.py
--rw-rw-rw-   0        0        0    37450 2023-07-11 02:24:33.000000 pih-1.46001/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.46001/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-11 06:56:24.634563 pih-1.46001/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-11 06:56:21.000000 pih-1.46001/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 06:56:22.000000 pih-1.46001/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2014 2023-06-27 04:00:23.000000 pih-1.46001/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-11 06:56:24.744140 pih-1.46001/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.683650 pih-1.46231/
+-rw-rw-rw-   0        0        0      261 2023-07-13 05:06:15.667995 pih-1.46231/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.324249 pih-1.46231/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.46231/pih/__init__.py
+-rw-rw-rw-   0        0        0    19907 2023-07-13 01:30:06.000000 pih-1.46231/pih/collection.py
+-rw-rw-rw-   0        0        0    56312 2023-07-13 04:47:44.000000 pih-1.46231/pih/console_api.py
+-rw-rw-rw-   0        0        0   106507 2023-07-13 03:02:11.000000 pih-1.46231/pih/const.py
+-rw-rw-rw-   0        0        0   303620 2023-07-13 05:05:09.000000 pih-1.46231/pih/pih.py
+-rw-rw-rw-   0        0        0    24689 2023-07-09 01:49:27.000000 pih-1.46231/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.46231/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.46231/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.46231/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6368 2023-07-11 03:24:37.000000 pih-1.46231/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.46231/pih/service_example.py
+-rw-rw-rw-   0        0        0    37523 2023-07-12 23:19:16.000000 pih-1.46231/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.46231/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-13 05:06:15.621121 pih-1.46231/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-13 05:06:14.000000 pih-1.46231/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-13 05:06:13.000000 pih-1.46231/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-07-13 05:05:53.000000 pih-1.46231/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 05:06:15.683650 pih-1.46231/setup.cfg
```

### Comparing `pih-1.46001/pih/collection.py` & `pih-1.46231/pih/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -533,20 +533,31 @@
     ip: str | None = None
     description: str | None = None
     variant: str | None = None
     port: int | None = None
     community: str | None = None 
     accessable: bool | None = None
 
+@dataclass
+class DiskStatistics:
+    name: str | None = None
+    free_space: int | None = None
+    size: int | None = None
+
+@dataclass
+class TimeSeriesStatistics:
+    count: int = 0
+    values: list[datetime] | None = None
 
 @dataclass
 class PrinterReport(PrinterStatus):
     name: str | None = None
     model: str | None = None
     serial: int | None = None
+    adminDescription: str | None = None
     meta: str | None = None
     printsOverall: int | None = None
     printsColor: int | None = None
     printsMonochrome: int | None = None
     fuserType: int | None = None
     fuserCapacity: int | None = None
     fuserRemaining: int | None = None
```

### Comparing `pih-1.46001/pih/console_api.py` & `pih-1.46231/pih/console_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTIES, FIELD_COLLECTION, PasswordSettings, CheckableSections, HOSTS, AD, PATHS, FILE
 from pih import PIH, A, NotFound, ActionValue, ActionStack, Input, Output, Session, while_not_do
 from pih.collection import (Mark, User, FullName, 
                             MarkDivision, UserBase, LoginPasswordPair, 
                             MarkGroup, Result, FieldItemList,
                             WorkstationDescription, ResourceStatus, SiteResourceStatus,
                             CTIndicationsValue, Workstation, RobocopyJobStatus, 
-                            ChillerIndicationsValueContainer, PrinterReport)
+                            ChillerIndicationsValueContainer, PrinterReport, DiskStatistics)
 from pih import A
 
 class ConsoleAppsApi:
 
     LINE: str = "........................................................"
 
     def __init__(self, pih: PIH = None):
@@ -68,32 +68,42 @@
             qr_code_image_path: str = PIH.PATH.QR_CODE.polibase_person_card_registry_folder(card_registry_folder_name_item)
             if show_result and len(card_registry_folder_name_list) == 1:
                 if not result:
                     self.output.error("qr код не был создан")
             if result:
                 result_path_list.append(qr_code_image_path)
         return result_path_list
+    
+    def disks_information(self, host: str | None = None) -> None:
+        host = host or self.input.input("Введите название хоста (компьютера или сервера)")
+        if A.C_R.accessibility_by_ping(host):
+            disk_statistics_list: list[DiskStatistics] = list(filter(lambda item: item.size > 0, A.PS.get_disk_statistics_list(host)))
+            if A.D_C.empty(disk_statistics_list):
+                self.output.error("Хост не имеет дисков")
+            else:
+                self.output.write_line("Информация о дисках:\n")
+                for disk_statistics in disk_statistics_list:
+                    self.output.write_line(f" {A.CT_V.BULLET} {self.bold(disk_statistics.name)}: {A.D_F.size(disk_statistics.free_space)} из {A.D_F.size(disk_statistics.size)}")
+        else:
+            self.output.error("Хост не доступен или не найден")
 
     def resources_and_indications_check(self, checkable_section_list: list[CheckableSections], ask_for_update_before: bool = False, force_update: bool = False, all: bool = False) -> None:
         if CheckableSections.RESOURCES in checkable_section_list or CheckableSections.WS in checkable_section_list:
             def label_function(resource: ResourceStatus, index: int) -> str:
                 result: list[str] = [] 
                 accessable: bool = resource.accessable
-                status: str = self.output.good_str("доступен") if accessable else self.bold(
-                    self.output.red_str("не доступен!"))
-                result.append(self.bold(self.output.blue_str(
-                    resource.name)) + ("" if isinstance(resource, SiteResourceStatus) else f": {status}"))
+                status: str = A.D_F.yes_no(accessable, True)
+                result.append(" ".join((status, self.bold(self.output.blue_str(
+                    resource.name)))))
                 if isinstance(resource, SiteResourceStatus):
                     if resource.check_free_space_status:
                         free_space_result_list: str = resource.free_space_status.split(" ")
-                        result.append(f"Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
+                        result.append(f"      Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
                     if resource.check_certificate_status:
-                        result.append(f"Сертификат доступен до: {resource.certificate_status}")
-                    result.append(ConsoleAppsApi.LINE)
-                    result.append(status)
+                        result.append(f"      Сертификат доступен до: {resource.certificate_status}")
                 return A.CT.NEW_LINE.join(result)
             force_update = force_update or (ask_for_update_before and self.input.yes_no(
                 "Обновить перед получением"))
             if force_update:
                 self.output.write_line(
                     self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
             for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS]:
@@ -120,24 +130,29 @@
             with self.output.make_indent(2):
                 self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
                 self.output.write_image(f"Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(modification_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
         if CheckableSections.VALENTA in checkable_section_list:
             count: int = len(A.PTH.get_file_list_by_directory_info(A.PTH.WS_816_SCAN.VALUE))
             self.output.new_line()
             self.output.write_line(
-                self.bold(f"{A.CT_V.BULLET} Новые исследования в Валенте: " +("Нет" if count == 0 else f"Да ({count})")))
+                self.bold(f"{A.CT_V.BULLET} Новые исследования в Валенте: " + ("Нет" if count == 0 else f"Да ({count})")))
+        if CheckableSections.SERVERS in checkable_section_list:
+            self.output.new_line()
+            self.output.write_line(self.bold(f"{A.CT_V.BULLET} Доступность серверов"))
+            with self.output.make_indent(2):
+                A.R.every(A.R_SRVS.all_description(), lambda server: self.output.write_line(" " .join((A.D_F.yes_no(A.C_R.accessibility_by_ping(server.name, count=1), True), self.bold(server.name)))))
         if CheckableSections.PRINTERS in checkable_section_list:
             self.output.new_line()
             self.output.separated_line()
             self.output.write_line(
                 self.bold(f"{A.CT_V.BULLET} Отчет по принтерам"))
             printer_report_list: list[PrinterReport] = A.R_PR.report(send_to_log=False).data
             for printer_report in printer_report_list:
                 self.output.separated_line()
-                with self.output.make_indent(3):
+                with self.output.make_indent(2):
                     self.output.write_line(A.D_F.printer_report(printer_report, self.bold))     
         if not all:
             if CheckableSections.BACKUPS in checkable_section_list:
                 robocopy_job_status_list: Result[list[RobocopyJobStatus]] = A.R_B.robocopy_job_status_list()
                 sort_by_status: bool = self.input.yes_no("Сортировать по статусу", no_label=f"{self.bold(f'Сортировать по дате выполнения - {A.CT_V.NUMBER_SYMBOLS[0]}')}")
                 A.R.sort(robocopy_job_status_list, (lambda item: item.last_status or max(A.CT_RBK.STATUS_CODE.keys())) if sort_by_status else lambda item: datetime.fromtimestamp(0) if A.D_C.empty(item.last_created) else A.D.datetime_from_string(item.last_created), sort_by_status)
                 def job_status_item_label_function(job_status: RobocopyJobStatus, index: int) -> str:
```

### Comparing `pih-1.46001/pih/const.py` & `pih-1.46231/pih/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     DOMAIN_SUFFIX: str = "lan"
     DOMAIN: str = ".".join([DOMAIN_NAME, DOMAIN_SUFFIX])
     DOMAIN_MAIN: str = DOMAIN
     USER_HOME_FOLDER_DISK: str = "U:"
     OU: str = "OU="
     ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
     WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
+    SERVERS_CONTAINER_DN: str = f"{OU}Servers,{ROOT_CONTAINER_DN}"
     USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
     ACTIVE_USERS_CONTAINER_DN: str = f"{OU}{USERS_CONTAINER_DN_SUFFIX}"
     INACTIVE_USERS_CONTAINER_DN: str = f"{OU}dead{USERS_CONTAINER_DN_SUFFIX}"
     PATH_ROOT: str = f"\\\\{DOMAIN_MAIN}"
     SEARCH_ALL_PATTERN: str = "*"
     GROUP_CONTAINER_DN: str = f"{OU}Groups,{ROOT_CONTAINER_DN}"
     JOB_POSITION_CONTAINER_DN: str = f"{OU}Job positions,{GROUP_CONTAINER_DN}"
@@ -717,14 +718,15 @@
 
     RESOURCES: int = auto()
     WS: int = auto()
     PRINTERS: int = auto()
     INDICATIONS: int = auto()
     BACKUPS: int = auto()
     VALENTA: int = auto()
+    SERVERS: int = auto()
 
     @staticmethod
     def all() :
         return [item for item in CheckableSections]
     
 class DocumentTypes(Enum):
     
@@ -1875,14 +1877,17 @@
     #
     POLIBASE_CREATION_DB_DUMP_START_TIME: TimeStorageValue = TimeStorageValue(
         "POLIBASE_CREATION_DB_DUMP_START_TIME", "20:30")
     #
     RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES: IntStorageValue = IntStorageValue(
         "RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES", 15)
     #
+    PRINTER_REPORT_PERIOD_IN_MINUTES: IntStorageValue = IntStorageValue(
+        "PRINTER_REPORT_PERIOD_IN_MINUTES", 5)
+    #
     POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION: StorageValue = StorageValue(
         "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION", CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
 
     POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE: StorageValue = StorageValue(
         "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE", CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_TEXT)
 
     POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: StorageValue = StorageValue(
@@ -1961,14 +1966,20 @@
 
     EMAIL_VALIDATION_IS_ON: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_IS_ON", True)
     EMAIL_VALIDATION_TEST: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_TEST", False)
 
     CHILLER_ALERT_TEMPEARTURE: FloatStorageValue = FloatStorageValue(
         "CHILLER_ALERT_TEMPEARTURE", 17.0)
     
+    CHILLER_MAX_TEMPEARTURE: IntStorageValue = IntStorageValue(
+        "CHILLER_MAX_TEMPEARTURE", 16)
+    
+    CHILLER_MIN_TEMPEARTURE: IntStorageValue = IntStorageValue(
+        "CHILLER_MIN_TEMPEARTURE", 10)
+    
 class PARAM_ITEMS:
 
     NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.NAME, "")
     PID: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PID, "")
     STATUS: ParamItem = ParamItem(FIELD_NAME_COLLECTION.STATUS, "")
     PERSON_PIN: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PERSON_PIN, "")
     PERSON_NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PERSON_NAME, "")
```

### Comparing `pih-1.46001/pih/pih.py` & `pih-1.46231/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -1625,15 +1625,15 @@
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.46001"
+            return "1.46231"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1809,15 +1809,17 @@
             return PIH.ACTION.SETTINGS.set(settings_item, value)
 
         @staticmethod
         def set_default(settings_item: SETTINGS) -> bool:
             return PIH.ACTION.SETTINGS.set_default(settings_item)
 
         @staticmethod
-        def get(settings_item: SETTINGS) -> Any:
+        def get(settings_item: SETTINGS | str) -> Any:
+            if isinstance(settings_item, str):
+                return PIH.RESULT.SETTINGS.get_by_name(settings_item).data
             return PIH.RESULT.SETTINGS.get(settings_item).data
 
         @staticmethod
         def init() -> None:
             for setting_item in SETTINGS:
                 if setting_item.value.auto_init:
                     PIH.SETTINGS.set_default(setting_item)
@@ -1897,14 +1899,32 @@
                 @staticmethod
                 def offer_telegram_bot_url_text(person_full_name: str) -> str:
                     return str(PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT)).format(name=FullNameTool.to_given_name(person_full_name)) 
 
     class PSTOOLS:
 
         @staticmethod
+        def get_disk_statistics_list(host: str) -> list[DiskStatistics]:
+            output: str = PIH.PSTOOLS.execute_command_list(f"powershell Get-WmiObject -Class win32_logicalDisk -ComputerName {host}", True, True, as_shell=True).stdout
+            result: list[DiskStatistics] = []
+            delimiter: str = ": "
+            delimiter_length: int = len(delimiter)
+            disk_statistics: DiskStatistics | None = None
+            for line in ListTool.not_empty_items(output.splitlines()):
+                line: str = line
+                if line.startswith("DeviceID"):
+                    disk_statistics = DiskStatistics(line[line.find(delimiter) + delimiter_length: -1])
+                    result.append(disk_statistics)
+                if line.startswith("FreeSpace"):
+                    disk_statistics.free_space = DataTool.if_not_empty(line[line.find(delimiter) + delimiter_length:], lambda item: int(item), 0)
+                if line.startswith("Size"):
+                    disk_statistics.size = DataTool.if_not_empty(line[line.find(delimiter) + delimiter_length:], lambda item: int(item), 0)
+            return result
+
+        @staticmethod
         def get_users_logged_on(host: str, active: bool | None = True) -> list[str]:
             def get_login_list(complete_process: CompletedProcess) -> set[str]:
                 result: set[str] = set()
                 output: str = complete_process.stdout.decode(WINDOWS.CHARSETS.ALTERNATIVE)
                 for line in output.splitlines()[1:]:
                     line = line.lower()
                     if DataTool.is_none(active) or (active and (line.find("active") != -1 or line.find("активно") != -1)) or (not active and (line.find("disc") != -1 or line.find("диск") != -1)):
@@ -1916,31 +1936,31 @@
             result |= get_login_list(PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                 ["query", "user", "/server"], host, interactive=None, run_from_system_account=True), True, True, False))
             return list(result)
 
         @staticmethod
         def stop_windows_service(name: str, workstation_name: str) -> bool:
             output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
-            ["sc", "stop", "stisvc"], workstation_name,  interactive=True, run_from_system_account=True), True, True).stdout
+                ["sc", "stop", name], workstation_name,  interactive=True, run_from_system_account=True), True, True).stdout
             return output.find("3  STOP_PENDING") != -1
 
         @staticmethod
         def start_windows_service(name: str, workstation_name: str) -> bool:
             output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
-            ["sc", "start", "stisvc"], workstation_name, interactive=True, run_from_system_account=True), True, True).stdout
+            ["sc", "start", name], workstation_name, interactive=True, run_from_system_account=True), True, True).stdout
             return output.find("2  START_PENDING") != -1 
 
         @staticmethod
         def windows_service_running(name: str, workstation_name: str) -> bool:
             output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
-            ["sc", "query", "stisvc"], workstation_name, interactive=True), True, True).stdout
+            ["sc", "query", name], workstation_name, interactive=True), True, True).stdout
             return output.find("4  RUNNING") != -1
 
         @staticmethod
-        def ping(address_or_ip: str, host: str, count: int = 1, timeout: int = 100):
+        def ping(address_or_ip: str, host: str | None = None, count: int = 1, timeout: int = 100):
             command_list: list[str] = ["ping", "-4",  address_or_ip, "-n",
                                        str(count), "-w", str(timeout)]
             result: CompletedProcess = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(command_list, host, interactive=True), True, True)
             output: str = result.stdout
             return result.returncode == 0 and output.count("(TTL)") < count
           
         @staticmethod
@@ -1972,19 +1992,19 @@
 
         @staticmethod
         def create_remote_process_executor_for_service(role_or_information: ServiceRoles | ServiceInformationBase, interactive: bool | None = False) -> list[str]:
             description: ServiceDescription = ServiceRoles.description(role_or_information)
             return PIH.PSTOOLS.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), description.login, description.password, interactive, description.run_from_system_account)
 
         @staticmethod
-        def execute_command_list(command_list: list[str], show_output: bool, capture_output: bool = False, as_text: bool = True) -> CompletedProcess:
+        def execute_command_list(command_list: list[str] | str, show_output: bool, capture_output: bool = False, as_text: bool = True, as_shell: bool = False) -> CompletedProcess:
             if show_output:
                 if capture_output:
                     process_result = subprocess.run(
-                        command_list, capture_output=True, text=as_text)
+                        command_list, capture_output=True, text=as_text, shell=as_shell)
                 else:
                     process_result = subprocess.run(
                         command_list, text=as_text)
             else:
                 process_result = subprocess.run(
                     command_list, stdout=DEVNULL, stderr=STDOUT, text=as_text)
             return process_result
@@ -2114,14 +2134,18 @@
             
             @staticmethod
             def service_was_started(information: ServiceInformation | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.SERVICE_WAS_STARTED, information, lambda: (information.name,
                                                     information.host, information.port, information.pid,  information))
 
             @staticmethod
+            def action_was_done(action: Actions | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BUILDER.create_event(Events.ACTION_WAS_DONE, action, lambda: (None, EnumTool.get(action).name,))
+
+            @staticmethod
             def chiller_temperature_alert_was_fired() -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED)
 
             @staticmethod
             def polibase_person_set_card_registry_folder(name: str | None = None, person: PolibasePerson | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_WAS_SET_FOR_POLIBASE_PERSON, (name, person), lambda: (DataTool.if_not_empty(person, lambda person: person.pin), name))
@@ -2132,17 +2156,17 @@
                         Events.CARD_REGISTRY_FOLDER_START_CARD_SORTING, name, lambda: (name, ))
 
             @staticmethod
             def card_registry_folder_complete_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_COMPLETE_CARD_SORTING, name, lambda: (PIH.DATA.FORMAT.polibase_person_card_registry_folder(name), ))
 
-            #staticmethod
-            #def chiller_was_turned_off() -> Events | tuple[Events, tuple[Any]]:
-            #    return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_TURNED_OFF)
+            staticmethod
+            def chiller_was_turned_off() -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_TURNED_OFF)
 
             @staticmethod
             def service_was_stopped(information: ServiceInformationBase | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.SERVICE_WAS_STOPPED, information, lambda: (information.name, information) )
             
             @staticmethod
             def polibase_persons_barcodes_old_format_were_detected(person_pin_list: list[int] | None = None) -> Events | tuple[Events, tuple[Any]]:
@@ -2592,21 +2616,22 @@
                       starts_handler: Callable[[IService | None], None] | None = None, 
                       max_workers: int | None = None, 
                       stop_before: bool = True, 
                       depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
                       isolate: bool = False,
                       show_output: bool = True) -> None:
                 service_description: ServiceInformationBase = A.CT_SR.description(role_or_information)
-                if service_description.host_changabled and not A.D.contains(A.OS.host(), service_description.host):
-                    PIH.SERVICE.ADMIN.change_host_on_local(service_description)
-                elif isolate:
-                    PIH.SERVICE.ADMIN.isolate(service_description)
-                if stop_before and not service_description.isolated:
-                    if PIH.SERVICE.check_accessibility(service_description):
-                        PIH.SERVICE.ADMIN.stop(service_description)
+                if isolate:
+                     PIH.SERVICE.ADMIN.isolate(service_description)
+                else:
+                    if service_description.host_changabled and not A.D.contains(A.OS.host(), service_description.host):
+                        PIH.SERVICE.ADMIN.change_host_on_local(service_description)
+                    if stop_before:
+                        if PIH.SERVICE.check_accessibility(service_description):
+                            PIH.SERVICE.ADMIN.stop(service_description)
                 def internal_start_handler(service: IService) -> None:
                     if starts_handler is not None:
                         if starts_handler.__code__.co_argcount == 1:
                             starts_handler(service)
                         else:
                             starts_handler()
                 service: IService = RPC.create_service()
@@ -2798,14 +2823,26 @@
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
         def find_variable(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
         
+        class VARIABLE:
+
+            NAME: str = "variable"
+
+            @staticmethod
+            def get(name: str) -> Any:
+                return PIH.RESULT.DATA_STORAGE.value(name, None, PIH.DATA.VARIABLE.NAME).data
+            
+            @staticmethod
+            def set(name: str, value: Any) -> None:
+                PIH.ACTION.DATA_STORAGE.value(value, name, section=PIH.DATA.VARIABLE.NAME)
+
         class ACTIONS:
 
             @staticmethod
             def get(action_or_name: str | Actions) -> Actions | None:
                 _action: Actions | None = None if isinstance(action_or_name, str) else action_or_name
                 if DataTool.is_none(_action):
                     for item in Actions:
@@ -3117,14 +3154,23 @@
             def to_base64(value: Any) -> str:
                 return base64.b64encode(value)
 
             @staticmethod 
             def bytes_to_string(value: bytes) -> str:
                 return value.decode("utf-8")
             
+        class STATISTICS:
+
+            @staticmethod
+            def for_chiller_filter() -> TimeSeriesStatistics:
+                events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(A.CT_A.CHILLER_FILTER_CHANGING))
+                if ResultTool.is_empty(events_result):
+                    return None
+                return TimeSeriesStatistics(len(events_result), ResultTool.map(events_result, lambda event: event.timestamp).data)
+            
         class CHECK:
 
             @staticmethod
             def polibase_person_has_new_barcode_format(polibase_person: PolibasePerson) -> bool:
                 return not (DataTool.is_empty(polibase_person.barcode) or polibase_person.barcode.find(CONST.POLIBASE.BARCODE.NEW_PREFIX) == -1)
 
             @staticmethod
@@ -3161,37 +3207,50 @@
                 @staticmethod
                 def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
                     return not DataTool.is_empty(value.temperature)
 
         class FORMAT:
 
             @staticmethod
+            def yes_no(value: bool, symbolic: bool = False) -> str:
+                c = DataTool.if_check
+                return c(value, c(symbolic, "✅", "Да"), c(symbolic, "❌", "Нет"))
+
+            @staticmethod
+            def size(value: int) -> str:
+                return str(int(value / 1024 / 1024 / 1024 )) + " Гб"
+
+            @staticmethod
             def printer_report(printer_report: PrinterReport, title_label_function: Callable[[str], str] = lambda value: value) -> str:
                 report_list: list[str] = []
                 if printer_report.name != -401:
-                    report_list.append(f"{title_label_function('Модель')}: {printer_report.model}\n{title_label_function('DNS название')}: {printer_report.ip}\n{title_label_function('Описание')}: {printer_report.description}")
-                    for item in (("Тонер", printer_report.get_toner), ("Драм-юнит", printer_report.get_drum)):
-                        report_list.append(f"\n {A.CT_V.BULLET} {title_label_function(item[0])}")
-                        action: Callable[[str], str] = item[1]
-                        report_list += [f"   {title_label_function(color.upper())}: %d%%" % action(color) for color in ["c", "m", "y", "k"]]
+                    name: str = printer_report.ip.split('.')[0]
+                    report_list.append(f"{title_label_function('Модель')}: {printer_report.model}\n{title_label_function('Название')}: {name}\n{title_label_function('Описание')}: {printer_report.description}")
+                    admin_description_list: list[str] = ("" or printer_report.adminDescription).split(",")
+                    if "infoless" not in admin_description_list:
+                        for item in (("Тонер", printer_report.get_toner), None if "drumless" in admin_description_list else ("Драм-юнит", printer_report.get_drum)  ):
+                            if DataTool.is_not_none(item):
+                                report_list.append(f"\n {A.CT_V.BULLET} {title_label_function(item[0])}")
+                                action: Callable[[str], str] = item[1]
+                                report_list += [f"   {title_label_function(color.upper())}: %d%%" % action(color) for color in (["k"] if "bw" in admin_description_list else ["c", "m", "y", "k"])]
                 else:
                     if not printer_report.accessable:
                         report_list.append("Принтер недоступен")
                     else:
                         report_list.append("Принтер доступен")
                 return "\n".join(report_list)
 
             @staticmethod
             def format(value: str) -> str:
                 fields: list[str] = [name for _, name, _, _ in Formatter().parse(value) if name]
-                my_fields: list[str] = DataTool.to_list(DATA.FORMATTER)
+                #my_fields: list[str] = DataTool.to_list(DATA.FORMATTER)
                 formatter: dict[str, str] = {}
                 for field_item in fields:
-                    if field_item in my_fields:
-                       formatter[field_item] = PIH.DATA.FORMAT.by_formatter_name(field_item, None)
+                    #if field_item in my_fields:
+                    formatter[field_item] = PIH.DATA.FORMAT.by_formatter_name(field_item, None)
                 if DataTool.is_empty(formatter):
                     return value
                 return value.format(**formatter)
 
             @staticmethod
             def index(value: int) -> str:
                 return str(value + 1) if value > 0 else ""
@@ -3231,27 +3290,29 @@
                 if isinstance(datetime, str):
                     datetime = PIH.DATA.datetime_from_string(datetime, CONST.ISO_DATETIME_FORMAT)
                 return PIH.PATH.replace_prohibited_symbols_from_path_with_symbol(PIH.DATA.datetime_to_string(datetime, A.CT.DATETIME_FORMAT))
 
             @staticmethod
             def by_formatter_name(value: Enum | str, data: Any | None) -> str | None:
                 if isinstance(value, str):
-                    value = A.D.get_by_value(DATA.FORMATTER, value)
+                    value = A.D.get_by_value(DATA.FORMATTER, value) or value
+                if isinstance(value, str):
+                    return PIH.SETTINGS.get(value) or PIH.DATA.VARIABLE.get(value)
                 if value == DATA.FORMATTER.MY_DATETIME:
                     return PIH.DATA.FORMAT.datetime(data)
                 if value == DATA.FORMATTER.MY_DATE:
                     return PIH.DATA.FORMAT.date(data)
                 if value == DATA.FORMATTER.CHILLER_FILTER_COUNT:
                     return str(PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT))
                 if value == DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS:
                     result_list: list[str] = [] 
                     for index in range(len(INDICATIONS.CHILLER.INDICATOR_NAME)):
                         if BM.has_index(data, index):
                             result_list.append(f"{A.CT_V.BULLET} {INDICATIONS.CHILLER.INDICATOR_NAME[index]}")
-                    return "\n\n" + "\n".join(result_list) + "\n"
+                    return "\n".join(("\n", "\n".join(result_list), ""))
                 return None
 
             @staticmethod
             def polibase_person_card_registry_folder(value: str) -> str:         
                 return value.upper()
 
             @staticmethod
@@ -3620,16 +3681,27 @@
             @staticmethod
             def key(key: str, default_value: Any | None = None) -> Result[Any]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.get_settings_value, (key, default_value)))
 
             @staticmethod
             def get(settings_item: SETTINGS) -> Result[Any]:
-                settings_value: StorageValue = settings_item.value
-                return PIH.RESULT.SETTINGS.key(settings_value.key_name or settings_item.name, settings_value.default_value)
+                settings_value: StorageValue = EnumTool.get(settings_item)
+                return PIH.RESULT.SETTINGS.get_by_name(settings_value.key_name or settings_item.name, settings_value.default_value)
+            
+            @staticmethod
+            def get_by_name(value: str, default_value: Any | None = None) -> Result[Any]:
+                return PIH.RESULT.SETTINGS.key(value, default_value)
+
+        class SERVERS:
+
+            @staticmethod
+            def all_description() -> Result[list[WorkstationDescription]]:
+                return DataTool.to_result(
+                    PIH.SERVICE.call_command(ServiceCommands.get_all_workstation_description, (AD.SERVERS_CONTAINER_DN,)), WorkstationDescription)
 
         class WORKSTATION:
 
             @staticmethod
             def all_description() -> Result[list[WorkstationDescription]]:
                 return DataTool.to_result(
                     PIH.SERVICE.call_command(ServiceCommands.get_all_workstation_description), WorkstationDescription)
@@ -4246,17 +4318,17 @@
                 return PIH.CHECK.RESOURCE.accessibility_by_ping_with_port(address_or_ip, WINDOWS.PORTS.SMB, host, count, check_for_all)
             
             @staticmethod
             def accessibility_by_ping(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
                 count = count or 4
                 local_ping_commnad_list: list[str] = [PIH.PSTOOLS.get_executor_path(
                     CONST.PSTOOLS.PS_PING), CONST.PSTOOLS.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
-                pocess_result: CompletedProcess = A.PS.execute_command_list(local_ping_commnad_list if host is None else A.PS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
-                if pocess_result.returncode == 0:
-                    out: str = pocess_result.stdout
+                process_result: CompletedProcess = A.PS.execute_command_list(local_ping_commnad_list if host is None else A.PS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
+                if process_result.returncode == 0:
+                    out: str = process_result.stdout
                     lost_marker: str = "Lost = "
                     index: int = out.find(lost_marker)
                     if index != -1:
                         lost_count: int = int(out[index +
                                                 len(lost_marker): out.find(" (", index)])
                         if check_for_all:
                             return lost_count == 0
@@ -5508,21 +5580,23 @@
 
     MIO = root.MIO
 
     IW = root.INPUT_WAIT
 
     R = root.RESULT
     D = root.DATA
+    D_V = D.VARIABLE
     D_TN = D.TELEPHONE_NUMBER
     D_MR = D.MATERIALIZED_RESOURCES
     D_FL = D.FILTER
     D_E = D.EXTRACT
     D_E_E = D_E.EVENT
     D_M = D.MARK
     D_C = D.CHECK
+    D_STAT = D.STATISTICS
     A = root.ACTION
     A_D = A.DOCUMENTS
     A_QR = A.QR_CODE
     A_I = A.INDICATION
     A_I_CT = A_I.CT
     A_I_CH = A_I.CHILLER
     ME = root.MESSAGE
@@ -5588,14 +5662,15 @@
     A_P = A.POLIBASE
     C_E = C.EVENTS
     C_P = C.POLIBASE
     C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
     R_P = R.POLIBASE
     R_PR = R.PRINTER
+    R_SRVS = R.SERVERS
     #
     A_PTH = A.PATH
     A_P_V = A_P.VISIT
     A_P_V_DS = A_P_V.DATA_STORAGE
     R_P_V = R_P.VISIT
     R_P_V_DS = R_P_V.DATA_STORAGE
     A_P_N = A_P.NOTIFICATION
```

### Comparing `pih-1.46001/pih/rpc.py` & `pih-1.46231/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/rpcCommandCall_pb2.py` & `pih-1.46231/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.46231/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/rpc_collection.py` & `pih-1.46231/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/rpc_const.py` & `pih-1.46231/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/service_example.py` & `pih-1.46231/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih/tools.py` & `pih-1.46231/pih/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,19 @@
     sys.path.append("//pih/facade")
 from pih.const import PASSWORD_GENERATION_ORDER, FIELD_COLLECTION_ALIAS, CONST
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
 class EnumTool:
 
     @staticmethod
-    def get(cls: Enum, key: str | None = None, default_value: Any | None = None, return_value: bool = True) -> Any | None:
+    def get(cls: Enum | Any, key: str | None = None, default_value: Any | None = None, return_value: bool = True) -> Any | None:
         if return_value and DataTool.is_empty(key):
-            return cls.value
+            if isinstance(cls, Enum):
+                return cls.value
+            return cls
         if key not in cls._member_map_:
             return default_value
         return cls._member_map_[key]
 
     @staticmethod
     def get_by_value(cls: Enum, value: Any, default_value: Any | None = None) -> Any | None:
         if isinstance(value, Enum):
```

### Comparing `pih-1.46001/pih/widgets.py` & `pih-1.46231/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.46001/pih_setup.py` & `pih-1.46231/pih_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
 setup(
     name=PIH.NAME,
-    version=f"{PIH.VERSION.local()}",
+    version=PIH.VERSION.local(),
     description="PIH library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
```

