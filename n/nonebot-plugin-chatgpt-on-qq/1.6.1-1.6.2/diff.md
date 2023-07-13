# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.6.1.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.6.1.tar", last modified: Tue Jun 13 04:36:04 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.6.2.tar", last modified: Thu Jul 13 17:03:46 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1.tar` & `nonebot-plugin-chatgpt-on-qq-1.6.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.369549 nonebot-plugin-chatgpt-on-qq-1.6.1/
--rw-rw-rw-   0        0        0      770 2023-06-13 04:36:04.367540 nonebot-plugin-chatgpt-on-qq-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.336542 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    22213 2023-06-13 04:30:27.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     1293 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py
--rw-rw-rw-   0        0        0    12934 2023-05-14 08:12:38.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/sessions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 04:36:04.361541 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-06-13 04:36:04.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 04:36:04.369549 nonebot-plugin-chatgpt-on-qq-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-06-13 04:32:16.000000 nonebot-plugin-chatgpt-on-qq-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:03:46.940813 nonebot-plugin-chatgpt-on-qq-1.6.2/
+-rw-rw-rw-   0        0        0      770 2023-07-13 17:03:46.938335 nonebot-plugin-chatgpt-on-qq-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-13 17:03:46.896070 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    23169 2023-07-13 17:03:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1772 2023-07-13 17:03:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/apikey.py
+-rw-rw-rw-   0        0        0     1136 2023-07-13 17:03:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    14372 2023-07-13 17:03:20.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:03:46.931136 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-07-13 17:03:46.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-13 17:03:46.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:03:46.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-07-13 17:03:46.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-13 17:03:46.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 17:03:46.940813 nonebot-plugin-chatgpt-on-qq-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-07-13 17:02:48.000000 nonebot-plugin-chatgpt-on-qq-1.6.2/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.6.1
+Version: 1.6.2
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 import re
+import json
 from datetime import datetime
 from json import JSONDecodeError
 from typing import Dict, List, Any, Type
 
 from nonebot.adapters.onebot.v11.utils import unescape
 from nonebot.adapters.onebot.v11.permission import GROUP
 from nonebot.adapters.onebot.v11 import (Bot, MessageEvent,
@@ -12,36 +12,36 @@
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from nonebot.plugin import on_regex
 from nonebot.params import ArgPlainText, RegexDict, EventMessage
 from nonebot.permission import SUPERUSER, Permission
 from nonebot.plugin import PluginMetadata
 
-from .config import Config, plugin_config
+from .config import Config, plugin_config, APIKeyPool
 from .loadpresets import presets_str
 from .custom_errors import NeedCreatSession
 from .sessions import session_container, Session, get_group_id
 
 customize_prefix: str = plugin_config.customize_prefix
 customize_talk_cmd: str = plugin_config.customize_talk_cmd
 # 因为电脑端的qq在输入/chat xxx时候经常被转换成表情，所以支持自定义指令前缀替换"chat"
 change_chat_to: str = plugin_config.change_chat_to
 prefix_str = customize_prefix if customize_prefix is not None else '/'
 chat_str = f'(chat|{change_chat_to})' if change_chat_to else 'chat'
 talk_cmd_str = customize_talk_cmd if customize_talk_cmd else 'talk'
 pattern_str = prefix_str + chat_str
-menu_chat_str=prefix_str+f'{change_chat_to}' if change_chat_to else 'chat'
+menu_chat_str = prefix_str + f'{change_chat_to}' if change_chat_to else 'chat'
 
 __usage__: str = (
     "指令表：\n"
     f"    {menu_chat_str} help 获取指令帮助菜单\n"
     f"    {menu_chat_str} auth 获取当前群会话管理权限状态\n"
     f"    {menu_chat_str} auth on 设置当前群仅管理员可以管理会话\n"
     f"    {menu_chat_str} auth off 设置当前群所有人均可管理会话\n"
-    f"    /talk <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
+    f"    {prefix_str}{talk_cmd_str} <会话内容> 在当前会话中进行会话(同样不需要括号，后面直接接你要说的话就行)\n"
     ">> 增\n"
     f"    {menu_chat_str} new  根据预制模板prompt创建并加入一个新的会话\n"
     f"    {menu_chat_str} new <自定义prompt> 根据自定义prompt创建并加入一个新的会话\n"
     f"    {menu_chat_str} json 根据历史会话json来创建一个会话，输入该命令后会提示你在下一个消息中输入json\n"
     f"    {menu_chat_str} cp 根据当前会话创建并加入一个新的会话\n"
     f"    {menu_chat_str} cp <id> 根据会话<id>为模板进行复制新建加入（id为{menu_chat_str} list中的序号）\n"
     ">> 删\n"
@@ -54,36 +54,36 @@
     f"    {menu_chat_str} rename <name> 重命名当前会话\n"
     ">> 查\n"
     f"    {menu_chat_str} who 查看当前会话信息\n"
     f"    {menu_chat_str} list 获取当前群所有存在的会话的序号及创建时间\n"
     f"    {menu_chat_str} list <@user> 获取当前群查看@的用户创建的会话\n"
     f"    {menu_chat_str} prompt 查看当前会话的prompt\n"
     f"    {menu_chat_str} dump 导出当前会话json字符串格式的上下文信息，可以用于{menu_chat_str} json导入\n"
+    f"    {menu_chat_str} keys 脱敏显示当前失效api key，仅主人"
 
 )
 __plugin_meta__ = PluginMetadata(
     name="多功能ChatGPT插件",
     description="基于chatGPT-3.5-turbo API的nonebot插件",
     usage=__usage__,
     config=Config,
     extra={
         "License": "BSD License",
         "Author": "颜曦",
-        "version": "1.6.0",
+        "version": "1.6.1",
     },
 )
 
 allow_private: bool = plugin_config.allow_private
-api_keys: List[str] = session_container.api_keys
+api_keys: APIKeyPool = session_container.api_keys
 temperature: float = plugin_config.temperature
 model: str = plugin_config.model_name
 max_tokens: int = plugin_config.max_tokens
 auto_create_preset_info: bool = plugin_config.auto_create_preset_info
-
-
+at_sender: bool = plugin_config.at_sender
 
 
 async def _allow_private_checker(event: MessageEvent) -> bool:
     return isinstance(event, GroupMessageEvent) or allow_private
 
 
 ALLOW_PRIVATE = Permission(_allow_private_checker)
@@ -106,167 +106,176 @@
 ReName = on_regex(rf"^{pattern_str}\s+rename\s+(?P<name>.+)$", permission=ALLOW_PRIVATE)  # 重命名当前会话
 ChatPrompt = on_regex(rf"^{pattern_str}\s+prompt$", permission=ALLOW_PRIVATE)
 ChatClear = on_regex(rf"{pattern_str}\s+clear$", permission=ALLOW_PRIVATE)
 ChatClearAt = on_regex(rf"{pattern_str}\s+clear\s*\S+$", permission=ALLOW_PRIVATE)
 SetAuthOn = on_regex(rf'^{pattern_str}\s+auth on$', permission=GROUP)
 SetAuthOff = on_regex(rf'^{pattern_str}\s+auth off$', permission=GROUP)
 ShowAuth = on_regex(rf'^{pattern_str}\s+auth$', permission=GROUP)
+ShowFailKey = on_regex(rf'^{pattern_str}\s+keys$', permission=SUPERUSER)
+
+
+@ShowFailKey.handle()
+async def _(event: MessageEvent):
+    await ShowFailKey.finish(api_keys.show_fail_keys(), at_sender=True)
 
 
 @ShowAuth.handle()
 async def _(event: GroupMessageEvent):
     group_id: str = get_group_id(event)
     if session_container.get_group_auth(group_id):
-        await ShowAuth.finish("当前仅有管理员有权限管理会话")
-    await ShowAuth.finish("当前所有人均有权限管理会话")
+        await ShowAuth.finish("当前仅有管理员有权限管理会话", at_sender=True)
+    await ShowAuth.finish("当前所有人均有权限管理会话", at_sender=True)
 
 
 async def auth_check(matcher: Type[Matcher], bot: Bot, event: MessageEvent, group_id: str) -> None:
     if isinstance(event, PrivateMessageEvent):
         return
     if session_container.get_group_auth(group_id) and not (await admin_check(bot, event)):
-        await matcher.finish('该群仅有管理员可以管理会话')
+        await matcher.finish('该群仅有管理员可以管理会话', at_sender=True)
 
 
 async def admin_check(bot: Bot, event: MessageEvent) -> bool:
     if not isinstance(event, GroupMessageEvent):
         return True
     return (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
 
 
 @SetAuthOff.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     group_id: str = get_group_id(event)
     perm_check = await admin_check(bot, event)
     if not perm_check:
-        await SetAuthOff.finish("只有群主或管理员才能设置权限管理")
+        await SetAuthOff.finish("只有群主或管理员才能设置权限管理", at_sender=True)
     session_container.set_group_auth(group_id, False)
-    await SetAuthOff.finish("设置成功，当前所有人均有权限管理会话")
+    await SetAuthOff.finish("设置成功，当前所有人均有权限管理会话", at_sender=True)
 
 
 @SetAuthOn.handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     group_id: str = get_group_id(event)
     perm_check = await admin_check(bot, event)
     if not perm_check:
-        await SetAuthOn.finish("只有群主或管理员才能设置权限管理")
+        await SetAuthOn.finish("只有群主或管理员才能设置权限管理", at_sender=True)
     session_container.set_group_auth(group_id, True)
-    await SetAuthOn.finish("设置成功，当前仅有管理员有权限管理会话")
+    await SetAuthOn.finish("设置成功，当前仅有管理员有权限管理会话", at_sender=True)
 
 
 @ChatClear.handle()
 async def _(bot: Bot, event: MessageEvent):
     group_id: str = get_group_id(event)
     perm_check = await admin_check(bot, event)
     if not perm_check:
-        await ChatClear.finish("只有群主或管理员才能清空本群全部会话!")
+        await ChatClear.finish("只有群主或管理员才能清空本群全部会话!", at_sender=True)
     session_list: List[Session] = session_container.get_group_sessions(group_id)
     num = len(session_list)
     for session in session_list:
         await session_container.delete_session(session, group_id)
-    await ChatClear.finish(f"成功删除全部共{num}条会话")
+    await ChatClear.finish(f"成功删除全部共{num}条会话", at_sender=True)
 
 
 @ChatClearAt.handle()
 async def _(bot: Bot, event: MessageEvent, message: Message = EventMessage()):
     if isinstance(event, PrivateMessageEvent):
         await ChatClearAt.finish()
     segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
     if not segments:
         await ChatClearAt.finish()
     perm_check = await admin_check(bot, event)
     sender_id: int = int(event.get_user_id())
     user_id: int = int(segments[0].data.get("qq", ""))
     group_id: str = get_group_id(event)
     if user_id != sender_id and not perm_check:
-        await ChatClearAt.finish("您不是该会话的创建者或管理员!")
-    session_list: List[Session] = [s for s in session_container.sessions if s.group == group_id and s.creator == user_id]
+        await ChatClearAt.finish("您不是该会话的创建者或管理员!", at_sender=True)
+    session_list: List[Session] = [s for s in session_container.sessions if
+                                   s.group == group_id and s.creator == user_id]
     num = len(session_list)
     if num == 0:
-        await ChatClearAt.finish(f"本群用户 {user_id} 还没有创建过会话哦")
+        await ChatClearAt.finish(f"本群用户 {user_id} 还没有创建过会话哦", at_sender=True)
     for session in session_list:
         await session_container.delete_session(session, group_id)
-    await ChatClearAt.finish(f"成功删除本群用户 {user_id} 创建的全部会话共{num}条")
+    await ChatClearAt.finish(f"成功删除本群用户 {user_id} 创建的全部会话共{num}条", at_sender=True)
 
 
 @ChatCP.handle()
 async def _(bot: Bot, event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(ChatCP, bot, event, group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if user_id not in group_usage:
-        await ChatCP.finish(f'请先加入一个会话，再进行复制当前会话 或者使用 {menu_chat_str} cp <id> 进行复制')
+        await ChatCP.finish(f'请先加入一个会话，再进行复制当前会话 或者使用 {menu_chat_str} cp <id> 进行复制',
+                            at_sender=True)
     session: Session = group_usage[user_id]
     group_usage[user_id].del_user(user_id)
     new_session: Session = session_container.create_with_session(session, user_id, group_id)
     await ChatCP.finish(f"创建并加入会话 '{new_session.name}' 成功!", at_sender=True)
 
 
 @ChatPrompt.handle()
 async def _(event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if user_id not in group_usage:
-        await ChatPrompt.finish('请先加入一个会话，再进行重命名')
+        await ChatPrompt.finish('请先加入一个会话，再进行重命名', at_sender=True)
     session: Session = group_usage[user_id]
-    await ChatPrompt.finish(f'会话：{session.name}\nprompt：{session.prompt}')
+    await ChatPrompt.finish(f'会话：{session.name}\nprompt：{session.prompt}', at_sender=True)
 
 
 @ReName.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(ReName, bot, event, group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if user_id not in group_usage:
-        await ReName.finish('请先加入一个会话，再进行重命名')
+        await ReName.finish('请先加入一个会话，再进行重命名', at_sender=True)
     perm_check = await admin_check(bot, event)
     session: Session = group_usage[user_id]
     name: str = unescape(info.get('name', '').strip())
     if session.creator == user_id or perm_check:
         session.rename(name[:32])
-        await ReName.finish(f'当前会话已命名为 {session.name}')
-    logger.info(f'重命名群 {group_id} 会话 {session.name} 失败：权限不足')
-    await ReName.finish("您不是该会话的创建者或管理员!")
+        await ReName.finish(f'当前会话已命名为 {session.name}', at_sender=True)
+    logger.info(f'重命名群 {group_id} 会话 {session.name} 失败：权限不足', at_sender=True)
+    await ReName.finish("您不是该会话的创建者或管理员!", at_sender=True)
 
 
 @ChatUserList.handle()
 async def _(event: MessageEvent, message: Message = EventMessage()):
     if isinstance(event, PrivateMessageEvent):
         await ChatUserList.finish()
     segments: List[MessageSegment] = [s for s in message if s.type == 'at' and s.data.get("qq", "all") != 'all']
     if not segments:
         await ChatUserList.finish()
     user_id: int = int(segments[0].data.get("qq", ""))
     group_id: str = get_group_id(event)
-    session_list: List[Session] = [s for s in session_container.sessions if s.group == group_id and s.creator == user_id]
+    session_list: List[Session] = [s for s in session_container.sessions if
+                                   s.group == group_id and s.creator == user_id]
     msg: str = f"在群中创建会话{len(session_list)}条：\n"
     for index, session in enumerate(session_list):
         msg += f" 名称:{session.name[:10]} " \
                f"创建者:{session.creator} " \
                f"时间:{datetime.fromtimestamp(session.creation_time)}\n"
-    await ChatUserList.finish(MessageSegment.at(user_id) + msg)
+    await ChatUserList.finish(MessageSegment.at(user_id) + msg, at_sender=True)
 
 
 @ChatWho.handle()
 async def _(event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     if user_id not in group_usage:
-        await ChatWho.finish('当前没有加入任何会话，请加入或创建一个会话')
+        await ChatWho.finish('当前没有加入任何会话，请加入或创建一个会话', at_sender=True)
     session: Session = group_usage[user_id]
     msg = f'当前所在会话信息:\n' \
           f"名称:{session.name[:10]}\n" \
           f"创建者:{session.creator}\n" \
           f"时间:{datetime.fromtimestamp(session.creation_time)}\n" \
           f"可以使用 {menu_chat_str} dump 导出json字符串格式的上下文信息"
-    await ChatWho.finish(msg)
+    await ChatWho.finish(msg, at_sender=True)
 
 
 @ChatCopy.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
@@ -286,17 +295,17 @@
 
 @Dump.handle()
 async def _(event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     try:
         session: Session = session_container.get_user_usage(group_id, user_id)
-        await Dump.finish(session.dump2json_str())
+        await Dump.finish(session.dump2json_str(), at_sender=True)
     except NeedCreatSession:
-        await Dump.finish('请先加入一个会话')
+        await Dump.finish('请先加入一个会话', at_sender=True)
 
 
 @Chat.handle()
 async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     content: str = unescape(info.get('content', '').strip())
     if not content:
         await Chat.finish("输入不能为空!", at_sender=True)
@@ -307,17 +316,15 @@
         session: Session = session_container.create_with_template('1', user_id, group_id)
         logger.info(f"{user_id} 自动创建并加入会话 '{session.name}'")
         if auto_create_preset_info:
             await Chat.send(f"自动创建并加入会话 '{session.name}' 成功", at_sender=True)
     else:
         session: Session = group_usage[user_id]
     answer: str = await session.ask_with_content(api_keys, content, 'user', temperature, model, max_tokens)
-    if answer:
-        await Chat.finish(answer)
-    await Chat.finish('连接失败...报错信息请查看日志')
+    await Chat.finish(answer, at_sender=at_sender)
 
 
 @Join.handle()
 async def _(event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id: int = int(info.get('id', '').strip())
     group_id: str = get_group_id(event)
     group_sessions: List[Session] = session_container.get_group_sessions(group_id)
@@ -345,42 +352,42 @@
 async def _(bot: Bot, event: MessageEvent):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(DelSelf, bot, event, group_id)
     group_usage: Dict[int, Session] = session_container.get_group_usage(group_id)
     session: Session = group_usage.pop(user_id, None)
     if not session:
-        await DelSelf.finish("当前不存在会话")
+        await DelSelf.finish("当前不存在会话", at_sender=True)
     perm_check = await admin_check(bot, event)
     if session.creator == user_id or perm_check:
         await session_container.delete_session(session, group_id)
-        await DelSelf.finish("删除成功!")
-    logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足')
-    await DelSelf.finish("您不是该会话的创建者或管理员!")
+        await DelSelf.finish("删除成功!", at_sender=True)
+    logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足', at_sender=True)
+    await DelSelf.finish("您不是该会话的创建者或管理员!", at_sender=True)
 
 
 @Delete.handle()
 async def _(bot: Bot, event: MessageEvent, info: Dict[str, Any] = RegexDict()):
     session_id = int(info.get('id', '').strip())
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     await auth_check(Delete, bot, event, group_id)
     group_sessions: List[Session] = session_container.get_group_sessions(group_id)
     if not group_sessions:
-        await Delete.finish("当前不存在会话")
+        await Delete.finish("当前不存在会话", at_sender=True)
     if session_id < 1 or session_id > len(group_sessions):
         await Delete.finish("序号超出!", at_sender=True)
     session: Session = group_sessions[session_id - 1]
     perm_check = await admin_check(bot, event)
     if session.creator == user_id or perm_check:
         await session_container.delete_session(session, group_id)
-        await Delete.finish("删除成功!")
+        await Delete.finish("删除成功!", at_sender=True)
     else:
-        logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足')
-        await Delete.finish("您不是该会话的创建者或管理员!")
+        logger.info(f'删除群 {group_id} 会话 {session.name} 失败：权限不足', at_sender=True)
+        await Delete.finish("您不是该会话的创建者或管理员!", at_sender=True)
 
 
 # 暂时已完成
 
 
 @ShowList.handle()
 async def _(event: MessageEvent):
@@ -418,15 +425,15 @@
 
 
 @CreateConversationWithTemplate.got(key="template")
 async def Create(event: MessageEvent, template_id: str = ArgPlainText("template")):
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     if not template_id.isdigit():
-        await CreateConversationWithTemplate.finish("输入ID无效！")
+        await CreateConversationWithTemplate.finish("输入ID无效！", at_sender=True)
     session: Session = session_container.create_with_template(template_id, user_id, group_id)
     await CreateConversationWithTemplate.send(f"使用模板 '{template_id}' 创建并加入会话 '{session.name}' 成功!",
                                               at_sender=True)
 
 
 @CreateConversationWithJson.handle()
 async def CreateConversation(bot: Bot, event: MessageEvent):
@@ -437,15 +444,15 @@
 
 @CreateConversationWithJson.got("jsonStr", "请直接输入json")
 async def GetJson(event: MessageEvent, json_str: str = ArgPlainText("jsonStr")):
     try:
         chat_log = json.loads(json_str)
     except JSONDecodeError:
         logger.error("json字符串错误!")
-        await CreateConversationWithJson.finish("Json错误！")
+        await CreateConversationWithJson.finish("Json错误！", at_sender=True)
     if not chat_log[0].get("role"):
-        await CreateConversationWithJson.finish("Json错误！")
+        await CreateConversationWithJson.finish("Json错误！", at_sender=True)
     user_id: int = int(event.get_user_id())
     group_id: str = get_group_id(event)
     session: Session = session_container.create_with_chat_log(chat_log, user_id, group_id,
                                                               name=chat_log[0].get('content', '')[:5])
     await CreateConversationWithJson.send(f"创建并加入会话 '{session}' 成功!", at_sender=True)
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/config.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from typing import List, Union
 
 from nonebot import get_driver
 from pydantic import Extra, BaseModel, validator
 
-from .custom_errors import ApiKeyError, NoApiKeyError
+from .apikey import APIKeyPool
 
 
-class Config(BaseModel, extra=Extra.ignore):
-    api_key: Union[str, List[str]] = None
+class Config(BaseModel, extra=Extra.ignore, arbitrary_types_allowed=True):
+    api_key: Union["APIKeyPool", str, List[str]] = None
     key_load_balancing: bool = False
     history_save_path: Path = Path("data/ChatHistory").absolute()
     preset_path: Path = Path("data/Presets").absolute()
     openai_proxy: str = None
     openai_api_base: str = None
     chat_memory_max: int = 10
     history_max: int = 100
@@ -22,20 +22,15 @@
     change_chat_to: str = None
     max_tokens: int = 1024
     auto_create_preset_info: bool = True
     customize_prefix: str = '/'
     customize_talk_cmd: str = 'talk'
     timeout: int = 10
     default_only_admin: bool = False
+    at_sender: bool = True
 
     @validator('api_key')
-    def api_key_validator(cls, v) -> List[str]:
-        if not v:
-            raise NoApiKeyError('请输入APIKEY')
-        if isinstance(v, list):
-            return v
-        if isinstance(v, str):
-            return [v]
-        raise ApiKeyError('请输入正确的APIKEY')
+    def api_key_validator(cls, v) -> APIKeyPool:
+        return APIKeyPool(v)
 
 
 plugin_config: Config = Config.parse_obj(get_driver().config)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq/sessions.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq/sessions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import copy
 import json
-import random
 import datetime
 from pathlib import Path
 from typing import List, Dict, Optional, Union, Set
 
 import openai
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
+from openai.error import InvalidAPIType, AuthenticationError, PermissionError, RateLimitError
 
 from .config import plugin_config
+from .apikey import APIKeyPool, APIKey
 from .loadpresets import templateDict
 from .custom_errors import NeedCreatSession, NoResponseError
 
 type_user_id = int
 type_group_id = str
 PRIVATE_GROUP: str = "Private"
 
@@ -31,17 +32,17 @@
     if isinstance(event, GroupMessageEvent):  # 当在群聊中时
         return str(event.group_id)
     else:  # 当在私聊中时
         return PRIVATE_GROUP + f'_{event.get_user_id()}'
 
 
 class SessionContainer:
-    def __init__(self, api_keys: List[str], chat_memory_max: int, history_max: int, dir_path: Path,
+    def __init__(self, api_keys: APIKeyPool, chat_memory_max: int, history_max: int, dir_path: Path,
                  default_only_admin: bool):
-        self.api_keys: List[str] = api_keys
+        self.api_keys: APIKeyPool = api_keys
         self.chat_memory_max: int = chat_memory_max
         self.history_max: int = history_max
         self.dir_path: Path = dir_path
         self.sessions: List[Session] = []
         self.session_usage: Dict[type_group_id, Dict[type_user_id, Session]] = {}
         self.default_only_admin: bool = default_only_admin
         self.group_auth: Dict[str, bool] = {}
@@ -88,15 +89,20 @@
     def old_version_check(session: "Session"):
         if session.group == PRIVATE_GROUP:
             session.file_path.unlink(missing_ok=True)
             session.group = PRIVATE_GROUP + f'_{session.creator}'
             session.save()
 
     def load(self) -> None:
-        for file in list(self.dir_path.glob('*.json')):
+        files: List[Path] = list(self.dir_path.glob('*.json'))
+        try:
+            files.remove(self.group_auth_file_path)
+        except ValueError:
+            pass
+        for file in files:
             session = Session.reload_from_file(file)
             if not session:
                 continue
             self.old_version_check(session)
             self.sessions.append(session)
             group = self.get_group_usage(session.group)
             for user in session.users:
@@ -193,64 +199,79 @@
 
     @property
     def chat_memory(self) -> List[Dict[str, str]]:
         return self.history[:self.basic_len] + self.history[self.basic_len - self.chat_memory_max:]
 
     async def ask_with_content(
             self,
-            api_keys: List[str],
+            api_keys: APIKeyPool,
             content: str,
             role: str = 'user',
             temperature: float = 0.5,
             model: str = 'gpt-3.5-turbo',
             max_tokens=1024,
     ) -> str:
         self.update(content, role)
         return await self.ask(api_keys, temperature, model, max_tokens)
 
     async def ask(
             self,
-            api_keys: List[str],
+            api_keys: APIKeyPool,
             temperature: float = 0.5,
             model: str = 'gpt-3.5-turbo',
             max_tokens=1024,
     ) -> str:
-        if not api_keys:
-            logger.error(
-                f'当前不存在api key，请在配置文件里进行配置...')
-            return ''
+        if api_keys.valid_num <= 0:
+            logger.error(f'当前不存在api key，请在配置文件里进行配置...')
+            return '当前不存在可用apikey，请联系管理员检查apikey信息'
         if _key_load_balancing:
-            random.shuffle(api_keys)
-        for num, key in enumerate(api_keys):
-            openai.api_key = key
-            logger.debug(f'当前使用 Api Key [{key[:4]}...{key[-4:]}]')
+            api_keys.shuffle()
+        for num, api_key in enumerate(api_keys):
+            api_key: APIKey
+            log_info = f'Api Key([{num + 1}/{len(api_keys)}]): {api_key.show()}'
+            if not api_key.status:
+                logger.warning(f'{log_info} 被标记失效，已跳过... \n失效原因:{api_key.fail_res}')
+                continue
+            openai.api_key = api_key.key
+            logger.debug(f'当前使用 {log_info}')
             try:
                 completion: dict = await openai.ChatCompletion.acreate(
                     model=model,
                     messages=self.chat_memory,
                     temperature=temperature,
                     max_tokens=max_tokens,
                     timeout=_timeout,
                 )
-                self.update_from_completion(completion)
                 if completion.get("choices") is None:
                     raise NoResponseError("未返回任何choices")
                 if len(completion["choices"]) == 0:
                     raise NoResponseError("返回的choices长度为0")
                 if completion["choices"][0].get("message") is None:
                     raise NoResponseError("未返回任何文本!")
-                logger.debug(f'使用当前 Api Key: [{key[:4]}...{key[-4:]}] 请求成功')
+                self.update_from_completion(completion)
+                logger.debug(f'{log_info} 请求成功')
                 return completion["choices"][0]["message"]["content"]
+            except RateLimitError as e:
+                if 'You exceeded your current quota, please check your plan and billing details.' in e.user_message:
+                    logger.warning(f'{log_info} 额度耗尽，已失效，尝试使用下一个...')
+                    logger.warning(f'{type(e)}: {e}')
+                    api_key.fail(f'{type(e).__name__}: {e}')
+                    api_keys.valid_num -= 1
+                else:
+                    logger.warning(f'{log_info} 请求速率过快，尝试使用下一个...')
+                    logger.warning(f'{e}')
+            except (InvalidAPIType, AuthenticationError, PermissionError) as e:
+                logger.warning(f'{log_info} 格式或权限错误，已失效，尝试使用下一个...')
+                logger.warning(f'{e}')
+                api_key.fail(f'{type(e).__name__}: {e}')
+                api_keys.valid_num -= 1
             except Exception as e:
-                logger.warning(
-                    f'当前 Api Key([{num + 1}/{len(api_keys)}]): [{key[:4]}...{key[-4:]}] 请求错误，尝试使用下一个...')
-                logger.warning(
-                    f'{type(e)}:{e}'
-                )
-        return ''
+                logger.warning(f'{log_info} 请求出现其他错误，尝试使用下一个...')
+                logger.warning(f'{type(e)}: {e}')
+        return '请求失败...请联系管理员查看错误日志和apikey信息'
 
     def update(self, content: str, role: str = 'user') -> None:
         self.history.append({'role': role, 'content': content})
         while len(self.history) > self.history_max:
             self.history.pop(0)
         self.save()
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.6.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.6.1
+Version: 1.6.2
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.6.1/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.6.1',
+    version='1.6.2',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

