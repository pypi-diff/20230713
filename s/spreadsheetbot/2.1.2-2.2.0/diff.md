# Comparing `tmp/spreadsheetbot-2.1.2.tar.gz` & `tmp/spreadsheetbot-2.2.0.tar.gz`

## Comparing `spreadsheetbot-2.1.2.tar` & `spreadsheetbot-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/Makefile
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/drive.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/errors.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/handlers.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/basic/log.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/__init__.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/abstract.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/groups.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/i18n.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/keyboard.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/log.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/notifications.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/registration.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/report.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/settings.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/switch.py
--rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/users.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/LICENSE.txt
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/Makefile
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/__init__.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/spreadsheetbot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/drive.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/errors.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/handlers.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/log.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/basic/scheldue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/__init__.py
+-rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/abstract.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/groups.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/i18n.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/keyboard.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/log.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/notifications.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/registration.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/replysheet.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/report.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/settings.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/switch.py
+-rw-r--r--   0        0        0    24613 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/users.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 spreadsheetbot-2.2.0/PKG-INFO
```

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/__init__.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/spreadsheetbot.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,30 @@
     ApplicationBuilder,
     ChatMemberHandler,
     CommandHandler,
     MessageHandler,
     CallbackQueryHandler,
 )
 
-from spreadsheetbot.sheets import (
-    I18n,
-    LogSheet,
-    Switch,
-    Settings,
-    Groups,
-    Users,
-    Registration,
-    Report,
-    Keyboard,
-    Notifications,
-    PerformAndScheldueNotifications
-)
+from spreadsheetbot.sheets.i18n import I18n
+from spreadsheetbot.sheets.switch import Switch
+from spreadsheetbot.sheets.settings import Settings
+from spreadsheetbot.sheets.registration import Registration
+from spreadsheetbot.sheets.log import LogSheet
+from spreadsheetbot.sheets.groups import Groups
+from spreadsheetbot.sheets.users import Users
+from spreadsheetbot.sheets.report import Report
+from spreadsheetbot.sheets.keyboard import Keyboard
+from spreadsheetbot.sheets.notifications import Notifications
+
+from spreadsheetbot.basic.log import Log
+from logging import INFO, DEBUG
+Log.setLevel(INFO)
 
-from spreadsheetbot.basic import Log, INFO, DEBUG
+from spreadsheetbot.basic.scheldue import PerformAndScheldueNotifications
 from spreadsheetbot.basic.handlers import ErrorHandlerFun, ChatMemberHandlerFun
 
 UPDATE_GROUP_USER_REQUEST  = 0
 UPDATE_GROUP_GROUP_REQUEST = 2
 UPDATE_GROUP_CHAT_MEMBER   = 3
 
 START_COMMAND  = 'start'
@@ -64,15 +65,14 @@
         Switch.scheldue_update(app)
         Settings.scheldue_update(app)
         Groups.scheldue_update(app)
         Users.scheldue_update(app)
         Registration.scheldue_update(app)
         Report.scheldue_update(app)
         Keyboard.scheldue_update(app)
-        Notifications.scheldue_update(app)
         PerformAndScheldueNotifications(app)
 
     async def post_shutdown(self, app: Application) -> None:
         await LogSheet.write(None, "Stopped an application")
 
     def run_polling(self):
         Log.info("Starting...")
@@ -134,26 +134,34 @@
             CommandHandler(START_COMMAND, Users.restart_help_on_registration_complete_handler, filters=Users.HasNoRegistrationStateFilter, block=False),
             CommandHandler(HELP_COMMAND,  Users.restart_help_on_registration_complete_handler, filters=Users.HasNoRegistrationStateFilter, block=False),
         ], group=UPDATE_GROUP_USER_REQUEST)
 
         app.add_handler(MessageHandler(Users.KeyboardKeyInputFilter, Users.keyboard_key_handler, block=False), group=UPDATE_GROUP_USER_REQUEST)
 
         app.add_handlers([
-            CallbackQueryHandler(Users.set_active_state_callback_handler, pattern=Users.CALLBACK_USER_ACTIVE_STATE_PATTERN, block=False),
-            CallbackQueryHandler(Users.change_state_callback_handler,     pattern=Users.CALLBACK_USER_CHANGE_STATE_PATTERN, block=False),
-            CommandHandler(START_COMMAND, Users.restart_help_change_state_handler, filters=Users.HasChangeRegistrationStateFilter, block=False),
-            CommandHandler(HELP_COMMAND,  Users.restart_help_change_state_handler, filters=Users.HasChangeRegistrationStateFilter, block=False),
+            CallbackQueryHandler(Users.set_active_state_callback_handler,          pattern=Users.CALLBACK_USER_ACTIVE_STATE_PATTERN, block=False),
+            CallbackQueryHandler(Users.change_state_callback_handler,              pattern=Users.CALLBACK_USER_CHANGE_STATE_PATTERN, block=False),
+            CommandHandler(START_COMMAND, Users.restart_help_change_state_handler, filters=Users.HasChangeRegistrationStateFilter,   block=False),
+            CommandHandler(HELP_COMMAND,  Users.restart_help_change_state_handler, filters=Users.HasChangeRegistrationStateFilter,   block=False),
             MessageHandler(Users.HasChangeRegistrationStateFilter, Users.change_state_reply_handler, block=False),
         ], group=UPDATE_GROUP_USER_REQUEST)
 
         app.add_handlers([
-            CallbackQueryHandler(Users.notification_set_state_callback_handler, pattern=Notifications.CALLBACK_SET_STATE_PATTERN, block=False),
-            CallbackQueryHandler(Users.notification_answer_callback_handler,    pattern=Notifications.CALLBACK_ANSWER_PATTERN,    block=False),
+            CallbackQueryHandler(Users.notification_set_state_callback_handler,    pattern=Notifications.CALLBACK_SET_STATE_PATTERN,     block=False),
+            CallbackQueryHandler(Users.notification_answer_callback_handler,       pattern=Notifications.CALLBACK_ANSWER_PATTERN,        block=False),
             CommandHandler(START_COMMAND, Users.restart_help_notification_handler, filters=Users.HasNotificationRegistrationStateFilter, block=False),
             CommandHandler(HELP_COMMAND,  Users.restart_help_notification_handler, filters=Users.HasNotificationRegistrationStateFilter, block=False),
-            MessageHandler(Users.HasNotificationRegistrationStateFilter, Users.notification_reply_handler, block=False),
+            MessageHandler(Users.HasNotificationRegistrationStateFilter,           Users.notification_reply_handler,                     block=False),
+        ], group=UPDATE_GROUP_USER_REQUEST)
+
+        app.add_handlers([
+            CallbackQueryHandler(Users.keyboard_set_state_callback_handler,    pattern=Keyboard.CALLBACK_SET_STATE_PATTERN,      block=False),
+            CallbackQueryHandler(Users.keyboard_answer_callback_handler,       pattern=Keyboard.CALLBACK_ANSWER_PATTERN,         block=False),
+            CommandHandler(START_COMMAND, Users.restart_help_keyboard_handler, filters=Users.HasKeyboardRegistrationStateFilter, block=False),
+            CommandHandler(HELP_COMMAND,  Users.restart_help_keyboard_handler, filters=Users.HasKeyboardRegistrationStateFilter, block=False),
+            MessageHandler(Users.HasKeyboardRegistrationStateFilter,           Users.keyboard_reply_handler,                     block=False),
         ], group=UPDATE_GROUP_USER_REQUEST)
         
         app.add_handler(MessageHandler(Users.StrangeErrorFilter, Users.strange_error_handler, block=False), group=UPDATE_GROUP_USER_REQUEST)
 
         app.run_polling()
         Log.info("Done. Goodby!")
```

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/drive.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/basic/drive.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/handlers.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/basic/handlers.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/basic/log.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/basic/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/abstract.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,27 +84,30 @@
             'action': action,
             'name': self.name,
         } | kwargs
     
     def scheldue_update(self, app: Application) -> None:
         app.create_task(self._update(app), self._create_update_context('Whole df update'))
     
+    async def _update_df(self) -> None:
+        await self._connect()
+        self.as_df = await self._get_df()
+    
     async def _update(self, app: Application) -> None:
         await self._pre_update()
         await asyncio.sleep(self.update_sleep_time)
         
         Log.info(f"Prepared to update whole df {self.name}")
         while len(self.mutex) > 0:
             Log.info(f"Halted whole df update at {self.name} with mutex {self.mutex}")
             await asyncio.sleep(self.retry_sleep_time)
         self.scheldue_update(app)
-        self.whole_mutex = True
         
-        await self._connect()
-        self.as_df = await self._get_df()
+        self.whole_mutex = True
+        await self._update_df()
         self.whole_mutex = False
 
         Log.info(f"Updated whole df {self.name}")
         Log.debug(f"\n\n{self.as_df}\n\n")
         await self._post_update()
     
     async def _pre_update(self):
```

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/groups.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/groups.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/i18n.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/i18n.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,12 +8,12 @@
     async def _get_df(self) -> pd.DataFrame:
         return pd.DataFrame(await self.wks.get_all_records())
     
     async def _post_async_init(self) -> None:
         for _,row in self.as_df.iterrows():
             setattr(self, row.key, row.value)
         self.yes_no = [self.yes, self.no]
-        self.yes_no_done = [self.yes, self.no, self.done]
+        self.yes_no_planned_done = [self.yes, self.no, self.planned, self.done]
         self.yes_no_super = [self.yes, self.no, self.super]
         self.yes_super = [self.yes, self.super]
 
 I18n = I18nAdapterClass()
```

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/keyboard.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/keyboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 import pandas as pd
-from spreadsheetbot.sheets.abstract import AbstractSheetAdapter
+from spreadsheetbot.sheets.replysheet import ReplySheet
 
 from telegram import ReplyKeyboardMarkup
 
 from spreadsheetbot.sheets.i18n import I18n
 from spreadsheetbot.sheets.settings import Settings
 
-class KeyboardAdapterClass(AbstractSheetAdapter):
+class KeyboardAdapterClass(ReplySheet):
+    CALLBACK_SET_STATE_PREFIX   = 'notif_state_'
+    CALLBACK_SET_STATE_TEMPLATE = 'notif_state_{state}'
+    CALLBACK_SET_STATE_PATTERN  = 'notif_state_*'
+
+    CALLBACK_ANSWER_PREFIX    = 'notif_answer_'
+    CALLBACK_ANSWER_TEMPLATE  = 'notif_answer_{state}_{answer}'
+    CALLBACK_ANSWER_PATTERN   = 'notif_answer_*'
+    CALLBACK_ANSWER_SEPARATOR = '_'
+
     def __init__(self) -> None:
         super().__init__('keyboard', 'keyboard', initialize_as_df=True)
     
     async def _pre_async_init(self):
         self.sheet_name = I18n.keyboard
         self.REGISTER_FUNCTION = I18n.register
         self.update_sleep_time = Settings.keyboard_update_time
         self.retry_sleep_time  = self.update_sleep_time // 2
     
     async def _get_df(self) -> pd.DataFrame:
         df = pd.DataFrame(await self.wks.get_all_records())
         df = df.drop(index = 0, axis = 0)
+        df = self.reply_buttons_split(df)
         df = df.loc[
             (df.key != "") &
-            (df.is_active == I18n.yes)
+            (df.is_active == I18n.yes) &
+            self.reply_state_get_df_condition(df)
         ]
         return df
     
     async def _process_df_update(self):
+        await super()._process_df_update()
         self.keys = self.as_df.key.values.tolist()
         self.reply_keyboard = ReplyKeyboardMarkup([
             self.keys[idx:idx+2]
             for idx in range(0,len(self.keys),2)
         ] if len(self.keys) > 2 else [[x] for x in self.keys])
         self.registration_keyboard_row = self._get(self.as_df.function == self.REGISTER_FUNCTION)
```

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/log.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/log.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/registration.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/registration.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/report.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/report.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/settings.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/settings.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/switch.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/switch.py`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/src/spreadsheetbot/sheets/users.py` & `spreadsheetbot-2.2.0/src/spreadsheetbot/sheets/users.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
         self.EditedMessageFilter = self.PrivateChatFilter & UpdateType.EDITED_MESSAGE
 
         self.HasActiveRegistrationStateFilter       = self.IsRegisteredFilter & self.HasActiveRegistrationStateClass(outer_obj=self)
         self.HasNoRegistrationStateFilter           = self.IsRegisteredFilter & self.HasNoRegistrationStateClass(outer_obj=self)
         self.HasChangeRegistrationStateFilter       = self.IsRegisteredFilter & self.HasChangeRegistrationStateClass(outer_obj=self)
         self.HasNotificationRegistrationStateFilter = self.IsRegisteredFilter & self.HasNotificationRegistrationStateClass(outer_obj=self)
+        self.HasKeyboardRegistrationStateFilter     = self.IsRegisteredFilter & self.HasKeyboardRegistrationStateClass(outer_obj=self)
 
         self.IsNotRegisteredFilter    = ~self.IsRegisteredFilter
 
         self.IsRegistrationOverFilter = self.PrivateChatFilter & ~self.IsRegistrationOpenedFilter & self.IsNotRegisteredFilter
         self.StartRegistrationFilter  = self.PrivateChatFilter &  self.IsRegistrationOpenedFilter & self.IsNotRegisteredFilter
         
         self.KeyboardKeyInputFilter = self.HasNoRegistrationStateFilter & self.InputInKeyboardKeysClass(outer_obj=self)
@@ -140,15 +141,15 @@
                                         send_photo: str = None, state: str = None,
                                         condition: str = None):
         condition_column = 'is_active' if condition in [None, ''] else condition
         self._send_to_all_uids(
             self.selector_condition(condition_column),
             app, message, parse_mode,
             send_photo,
-            reply_markup=Notifications.get_keyboard(state)
+            reply_markup=Notifications.get_inline_keyboard_by_state(state)
         )
     
     class PrivateChatClass(AbstractSheetAdapter.AbstractFilter):
         def filter(self, message: Message) -> bool:
             return message.chat.type == Chat.PRIVATE
     
     class IsRegistrationOpenedClass(AbstractSheetAdapter.AbstractFilter):
@@ -186,14 +187,22 @@
     class HasNotificationRegistrationStateClass(AbstractSheetAdapter.AbstractFilter):
         def filter(self, message: Message) -> bool:
             df = self.outer_obj.as_df
             return not df.loc[
                 (self.outer_obj.selector(message.chat_id)) &
                 (df.state.isin(Notifications.states))
             ].empty
+
+    class HasKeyboardRegistrationStateClass(AbstractSheetAdapter.AbstractFilter):
+        def filter(self, message: Message) -> bool:
+            df = self.outer_obj.as_df
+            return not df.loc[
+                (self.outer_obj.selector(message.chat_id)) &
+                (df.state.isin(Keyboard.states))
+            ].empty
     
     class InputInKeyboardKeysClass(AbstractSheetAdapter.AbstractFilter):
         def filter(self, message: Message) -> bool:
             return message.text in Keyboard.keys
     
     async def registration_is_over_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         await update.message.reply_markdown(Settings.registration_is_over, reply_markup=ReplyKeyboardRemove())
@@ -271,34 +280,51 @@
         keyboard_row = Keyboard.get(update.message.text)
         if keyboard_row.function == Keyboard.REGISTER_FUNCTION:
             user = self._get(self.selector(update.effective_chat.id))
             await update.message.reply_markdown(
                 keyboard_row.text_markdown.format(user=self.user_data_markdown(user)),
                 reply_markup=self.user_data_inline_keyboard(user)
             )
-        elif keyboard_row.send_picture == '':
+            return
+
+        condition_column = 'is_active' if keyboard_row.condition in [None, ''] else keyboard_row.condition
+        show_button = not self.as_df.loc[
+            self.selector(update.message.chat_id) &
+            self.selector_condition(condition_column)
+        ].empty
+
+        reply_keyboard = Keyboard.reply_keyboard
+        if keyboard_row.state not in [None, ''] and show_button == True:
+            reply_keyboard = Keyboard.get_inline_keyboard_by_state(keyboard_row.state)
+        
+        if keyboard_row.send_picture == '':
             await update.message.reply_markdown(
                 keyboard_row.text_markdown,
-                reply_markup=Keyboard.reply_keyboard
+                reply_markup=reply_keyboard
             )
-        elif keyboard_row.send_picture != '' and len(keyboard_row.text_markdown) <= 1024:
+            return
+
+        if keyboard_row.send_picture != '' and len(keyboard_row.text_markdown) <= 1024:
             await update.message.reply_photo(
                 keyboard_row.send_picture,
                 caption=keyboard_row.text_markdown,
                 parse_mode=ParseMode.MARKDOWN,
-                reply_markup=Keyboard.reply_keyboard
+                reply_markup=reply_keyboard
             )
-        elif keyboard_row.send_picture != '' and len(keyboard_row.text_markdown) > 1024:
+            return
+
+        if keyboard_row.send_picture != '' and len(keyboard_row.text_markdown) > 1024:
             await update.message.reply_markdown(
                 keyboard_row.text_markdown
             )
             await update.message.reply_photo(
                 keyboard_row.send_picture,
-                reply_markup=Keyboard.reply_keyboard
+                reply_markup=reply_keyboard
             )
+            return
     
     async def set_active_state_callback_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         await update.callback_query.answer()
         await context.bot.send_message(
             update.effective_chat.id,
             I18n.has_been_set_inactive if update.callback_query.data == self.CALLBACK_USER_SET_INACTIVE else I18n.has_been_set_active,
             reply_markup=Keyboard.reply_keyboard,
@@ -360,60 +386,110 @@
         )
         await self._change_message_after_callback(update.effective_chat.id, message_id, context.application)
     
     async def restart_help_notification_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         template = Settings.user_template_from_update(update)
         state = self.state(update.effective_chat.id)
         await update.message.reply_markdown(
-            template.format(template = Notifications.get_text_markdown(state)),
-            reply_markup=Notifications.get_keyboard(state)
+            template.format(template = Notifications.get_text_markdown_by_state(state)),
+            reply_markup=Notifications.get_inline_keyboard_by_state(state)
+        )
+    
+    async def restart_help_keyboard_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        template = Settings.user_template_from_update(update)
+        state = self.state(update.effective_chat.id)
+        await update.message.reply_markdown(
+            template.format(template = Keyboard.get_text_markdown_by_state(state)),
+            reply_markup=Keyboard.get_inline_keyboard_by_state(state)
         )
     
     async def notification_set_state_callback_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         await update.callback_query.answer()
         state = update.callback_query.data.removeprefix(Notifications.CALLBACK_SET_STATE_PREFIX)
         await context.bot.send_message(
             update.effective_chat.id,
-            Notifications.get_button_answer(state),
+            Notifications.get_button_answer_by_state(state),
+            parse_mode=ParseMode.MARKDOWN,
+            reply_markup=ReplyKeyboardRemove()
+        )
+        await self._update_record(update.effective_chat.id, 'state', state)
+    
+    async def keyboard_set_state_callback_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        await update.callback_query.answer()
+        state = update.callback_query.data.removeprefix(Keyboard.CALLBACK_SET_STATE_PREFIX)
+        await context.bot.send_message(
+            update.effective_chat.id,
+            Keyboard.get_button_answer_by_state(state),
             parse_mode=ParseMode.MARKDOWN,
             reply_markup=ReplyKeyboardRemove()
         )
         await self._update_record(update.effective_chat.id, 'state', state)
     
     async def notification_answer_callback_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         await update.callback_query.answer()
         state,answer_idx = update.callback_query.data\
             .removeprefix(Notifications.CALLBACK_ANSWER_PREFIX)\
             .split(Notifications.CALLBACK_ANSWER_SEPARATOR)
-        text,answer = Notifications.get_button_answer(state, int(answer_idx))
+        text,answer = Notifications.get_button_answer_by_state(state, int(answer_idx))
+        await context.bot.send_message(
+            update.effective_chat.id,
+            text,
+            parse_mode=ParseMode.MARKDOWN,
+            reply_markup=Keyboard.reply_keyboard
+        )
+        await self._update_record(update.effective_chat.id, state, answer)
+    
+    async def keyboard_answer_callback_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        await update.callback_query.answer()
+        state,answer_idx = update.callback_query.data\
+            .removeprefix(Keyboard.CALLBACK_ANSWER_PREFIX)\
+            .split(Keyboard.CALLBACK_ANSWER_SEPARATOR)
+        text,answer = Keyboard.get_button_answer_by_state(state, int(answer_idx))
         await context.bot.send_message(
             update.effective_chat.id,
             text,
             parse_mode=ParseMode.MARKDOWN,
             reply_markup=Keyboard.reply_keyboard
         )
         await self._update_record(update.effective_chat.id, state, answer)
     
     async def notification_reply_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         user    = self.get(update.effective_chat.id)
         state   = user.state
         save_as = user[Settings.user_document_name_field]
-        notification = Notifications.get(state)
+        notification = Notifications.get_by_state(state)
 
         state_val, save_to = self._prepare_state_to_save(update.message, notification.document_link)
         if state_val == None:
             await update.message.reply_markdown(notification.button_answer[0], reply_markup=ReplyKeyboardRemove())
             return
 
         await update.message.reply_markdown(notification.button_answer[1], reply_markup=Keyboard.reply_keyboard)
         await self._batch_update_or_create_record(update.effective_chat.id, save_to=save_to, save_as=save_as, app=context.application,
             state = '',
             **{state: state_val}
         )
     
+    async def keyboard_reply_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        user         = self.get(update.effective_chat.id)
+        state        = user.state
+        save_as      = user[Settings.user_document_name_field]
+        keyboard_row = Keyboard.get_by_state(state)
+
+        state_val, save_to = self._prepare_state_to_save(update.message, keyboard_row.document_link)
+        if state_val == None:
+            await update.message.reply_markdown(keyboard_row.button_answer[0], reply_markup=ReplyKeyboardRemove())
+            return
+
+        await update.message.reply_markdown(keyboard_row.button_answer[1], reply_markup=Keyboard.reply_keyboard)
+        await self._batch_update_or_create_record(update.effective_chat.id, save_to=save_to, save_as=save_as, app=context.application,
+            state = '',
+            **{state: state_val}
+        )
+    
     async def strange_error_handler(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         await update.message.reply_markdown(Settings.strange_user_error, reply_markup=ReplyKeyboardRemove())
         chat_id = update.effective_chat.id
         message = (
             f"Strange error on user with id `{chat_id}` "
             f"and username `{update.effective_chat.username}` "
             f"- user is not registered, but the bot is active"
```

### Comparing `spreadsheetbot-2.1.2/.gitignore` & `spreadsheetbot-2.2.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Byte-compiled / optimized / DLL files
-**.__pycache__/
+**/__pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
```

### Comparing `spreadsheetbot-2.1.2/LICENSE.txt` & `spreadsheetbot-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/README.md` & `spreadsheetbot-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spreadsheetbot-2.1.2/pyproject.toml` & `spreadsheetbot-2.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spreadsheetbot"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Google Spreadsheet-based Telegram Bot Package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `spreadsheetbot-2.1.2/PKG-INFO` & `spreadsheetbot-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spreadsheetbot
-Version: 2.1.2
+Version: 2.2.0
 Summary: Google Spreadsheet-based Telegram Bot Package
 Project-URL: Homepage, https://github.com/twobrowin-study/spreadsheetbot-lib
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/spreadsheetbot-lib/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

