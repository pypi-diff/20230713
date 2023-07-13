# Comparing `tmp/dpys-5.5.8.tar.gz` & `tmp/dpys-5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpys-5.5.8.tar", last modified: Sun May 29 05:18:40 2022, max compression
+gzip compressed data, was "dpys-5.5.9.tar", last modified: Thu Jul 13 14:05:12 2023, max compression
```

## Comparing `dpys-5.5.8.tar` & `dpys-5.5.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-05-29 05:18:40.228279 dpys-5.5.8/
--rw-rw-rw-   0        0        0     1094 2022-01-04 00:41:35.000000 dpys-5.5.8/LICENSE
--rw-rw-rw-   0        0        0    19117 2022-05-29 05:18:40.227278 dpys-5.5.8/PKG-INFO
--rw-rw-rw-   0        0        0    18612 2022-05-29 04:54:34.000000 dpys-5.5.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-29 05:18:40.210986 dpys-5.5.8/dpys/
--rw-rw-rw-   0        0        0    49130 2022-05-29 05:18:28.000000 dpys-5.5.8/dpys/__init__.py
--rw-rw-rw-   0        0        0     2510 2022-05-28 20:24:29.000000 dpys-5.5.8/dpys/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-29 05:18:40.226136 dpys-5.5.8/dpys.egg-info/
--rw-rw-rw-   0        0        0    19117 2022-05-29 05:18:40.000000 dpys-5.5.8/dpys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2022-05-29 05:18:40.000000 dpys-5.5.8/dpys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-29 05:18:40.000000 dpys-5.5.8/dpys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-05-29 05:18:40.000000 dpys-5.5.8/dpys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-05-29 05:18:40.000000 dpys-5.5.8/dpys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-29 05:18:40.228279 dpys-5.5.8/setup.cfg
--rw-rw-rw-   0        0        0      917 2022-05-29 05:18:36.000000 dpys-5.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:05:12.987377 dpys-5.5.9/
+-rw-rw-rw-   0        0        0     1094 2022-01-04 00:41:35.000000 dpys-5.5.9/LICENSE
+-rw-rw-rw-   0        0        0    19135 2023-07-13 14:05:12.987377 dpys-5.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0    18630 2023-07-13 13:57:27.000000 dpys-5.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 14:05:12.956126 dpys-5.5.9/dpys/
+-rw-rw-rw-   0        0        0    48810 2023-07-13 14:05:00.000000 dpys-5.5.9/dpys/__init__.py
+-rw-rw-rw-   0        0        0     2510 2022-05-28 20:24:29.000000 dpys-5.5.9/dpys/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:05:12.987377 dpys-5.5.9/dpys.egg-info/
+-rw-rw-rw-   0        0        0    19135 2023-07-13 14:05:12.000000 dpys-5.5.9/dpys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-07-13 14:05:12.000000 dpys-5.5.9/dpys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:05:12.000000 dpys-5.5.9/dpys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-13 14:05:12.000000 dpys-5.5.9/dpys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-13 14:05:12.000000 dpys-5.5.9/dpys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 14:05:12.987377 dpys-5.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-07-13 14:05:03.000000 dpys-5.5.9/setup.py
```

### Comparing `dpys-5.5.8/LICENSE` & `dpys-5.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dpys-5.5.8/PKG-INFO` & `dpys-5.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpys
-Version: 5.5.8
+Version: 5.5.9
 Summary: A library to simplify discord.py
 Home-page: https://jgltechnologies.com/dpys
 Author: George Luca
 Author-email: fixingg@gmail.com
 License: MIT
 Keywords: discord
 Platform: UNKNOWN
@@ -53,17 +53,17 @@
 <br>
 
 ```python
 import dpys
 from disnake.ext import commands
 
 bot = commands.AutoShardedBot(command_prefix="!")
-TOKEN = "Your Token
+TOKEN = "Your Token"
 
-bot.loop.create_task(dpys.setup(bot, DIR))
+bot.loop.create_task(dpys.setup(bot, "database directory"))
 bot.run()
 ```
 
 <br>
 
 Reaction role example
 
@@ -169,15 +169,15 @@
 ```
 
 <br>
 <br>
 
 # Documentation
 
-You will here 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
+You will hear 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
 muted, and added back when they are unmuted.
 
 ## Admin class
 
 Kick:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dpys Version: 5.5.8 Summary: A library to simplify
+Metadata-Version: 2.1 Name: dpys Version: 5.5.9 Summary: A library to simplify
 discord.py Home-page: https://jgltechnologies.com/dpys Author: George Luca
 Author-email: fixingg@gmail.com License: MIT Keywords: discord Platform:
 UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Description-Content-Type: text/
 markdown License-File: LICENSE [https://discord.com/api/guilds/
 844418702430175272/embed.png] # DPYS ## The goal of DPYS is to make basic
@@ -15,16 +15,16 @@
 can be given in [our Discord server](https://jgltechnologies.com/disnake). If
 you see any problems in the code or want to add a feature, create a pull
 request on [our Github repository](https://jgltechnologies.com/dpys/src).
 Install from pypi ``` python -m pip install dpys ```
 Install from github ``` python -m pip install git+https://github.com/
 JGLTechnologies/dpys ``` Setup
 ```python import dpys from disnake.ext import commands bot =
-commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token
-bot.loop.create_task(dpys.setup(bot, DIR)) bot.run() ```
+commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token"
+bot.loop.create_task(dpys.setup(bot, "database directory")) bot.run() ```
 Reaction role example
 ```python import dpys from disnake.ext import commands import disnake bot =
 commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token" # Do not type
 hint disnake.Role for the role argument # Command to create the reaction role
 @bot.slash_command(name="rr") async def reaction_role_command(inter:
 disnake.ApplicationCommandInteraction, emoji: str = commands.Param
 ( description="An emoji or list of emojis"), role: str = commands.Param
@@ -64,15 +64,15 @@
 when its message is deleted in channel.purge() @bot.listen
 ("on_raw_bulk_message_delete") async def rr_clear_on_raw_bulk_message_delete
 (payload): await dpys.rr.clear_on_raw_bulk_message_delete(payload) # Clears all
 DPYS data for a guild when it is removed @bot.listen("on_guild_remove") async
 def clear_on_guild_remove(guild): await dpys.misc.clear_data_on_guild_remove
 (guild) bot.loop.create_task(dpys.setup(bot, DIR)) bot.run(TOKEN) ```
 
-# Documentation You will here 'mute remove role' mentioned a lot. This is just
+# Documentation You will hear 'mute remove role' mentioned a lot. This is just
 an optional role that gets removed when a member is muted, and added back when
 they are unmuted. ## Admin class Kick: ```python async def kick(inter:
 disnake.ApplicationCommandInteraction, member: disnake.Member, reason:
 typing.Optional[str] = None, msg: str = None) -> None ``` ```python import dpys
 @bot.slash_command(name="kick") @commands.has_permissions(kick_members=True)
 async def kick(inter, member: disnake.Member = commands.Param(), reason: str =
 commands.Param(default=None)): await dpys.admin.kick(inter, member, reason) ```
```

### Comparing `dpys-5.5.8/README.md` & `dpys-5.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 <br>
 
 ```python
 import dpys
 from disnake.ext import commands
 
 bot = commands.AutoShardedBot(command_prefix="!")
-TOKEN = "Your Token
+TOKEN = "Your Token"
 
-bot.loop.create_task(dpys.setup(bot, DIR))
+bot.loop.create_task(dpys.setup(bot, "database directory"))
 bot.run()
 ```
 
 <br>
 
 Reaction role example
 
@@ -152,15 +152,15 @@
 ```
 
 <br>
 <br>
 
 # Documentation
 
-You will here 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
+You will hear 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
 muted, and added back when they are unmuted.
 
 ## Admin class
 
 Kick:
 
 ```python
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 Discord server](https://jgltechnologies.com/disnake). If you see any problems
 in the code or want to add a feature, create a pull request on [our Github
 repository](https://jgltechnologies.com/dpys/src).
 Install from pypi ``` python -m pip install dpys ```
 Install from github ``` python -m pip install git+https://github.com/
 JGLTechnologies/dpys ``` Setup
 ```python import dpys from disnake.ext import commands bot =
-commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token
-bot.loop.create_task(dpys.setup(bot, DIR)) bot.run() ```
+commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token"
+bot.loop.create_task(dpys.setup(bot, "database directory")) bot.run() ```
 Reaction role example
 ```python import dpys from disnake.ext import commands import disnake bot =
 commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token" # Do not type
 hint disnake.Role for the role argument # Command to create the reaction role
 @bot.slash_command(name="rr") async def reaction_role_command(inter:
 disnake.ApplicationCommandInteraction, emoji: str = commands.Param
 ( description="An emoji or list of emojis"), role: str = commands.Param
@@ -58,15 +58,15 @@
 when its message is deleted in channel.purge() @bot.listen
 ("on_raw_bulk_message_delete") async def rr_clear_on_raw_bulk_message_delete
 (payload): await dpys.rr.clear_on_raw_bulk_message_delete(payload) # Clears all
 DPYS data for a guild when it is removed @bot.listen("on_guild_remove") async
 def clear_on_guild_remove(guild): await dpys.misc.clear_data_on_guild_remove
 (guild) bot.loop.create_task(dpys.setup(bot, DIR)) bot.run(TOKEN) ```
 
-# Documentation You will here 'mute remove role' mentioned a lot. This is just
+# Documentation You will hear 'mute remove role' mentioned a lot. This is just
 an optional role that gets removed when a member is muted, and added back when
 they are unmuted. ## Admin class Kick: ```python async def kick(inter:
 disnake.ApplicationCommandInteraction, member: disnake.Member, reason:
 typing.Optional[str] = None, msg: str = None) -> None ``` ```python import dpys
 @bot.slash_command(name="kick") @commands.has_permissions(kick_members=True)
 async def kick(inter, member: disnake.Member = commands.Param(), reason: str =
 commands.Param(default=None)): await dpys.admin.kick(inter, member, reason) ```
```

### Comparing `dpys-5.5.8/dpys/__init__.py` & `dpys-5.5.9/dpys/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from disnake.ext import commands
 from disnake import ApplicationCommandInteraction
 from .utils import GuildData
 
 RED = 0xD40C00
 BLUE = 0x0000FF
 GREEN = 0x32C12C
-version = "5.5.8"
+version = "5.5.9"
 EPHEMERAL = True
 warnings_db: aiosqlite.Connection
 muted_db: aiosqlite.Connection
 rr_db: aiosqlite.Connection
 curse_db: aiosqlite.Connection
 
 print("We recommend that you read https://jgltechnologies.com/dpys before you use DPYS.")
@@ -110,47 +110,47 @@
 
 class admin:
 
     @staticmethod
     async def mute(inter: ApplicationCommandInteraction, member: discord.Member, role_add: int,
                    role_remove: typing.Optional[int] = None, reason: str = None, msg: str = None) -> None:
         if inter.guild.get_role(role_add) in member.roles:
-            await inter.response.send_message(f"{member.name}#{member.discriminator} is already muted.",
+            await inter.response.send_message(f"{member.display_name} is already muted.",
                                               ephemeral=EPHEMERAL)
             return
         if len(str(reason)) > 256:
             reason = reason[:256]
         if not isinstance(inter.guild.get_role(role_add), discord.Role):
             return
         await member.add_roles(inter.guild.get_role(role_add))
         if role_remove is not None:
             with contextlib.suppress(discord.Forbidden, discord.HTTPException):
                 await member.remove_roles(inter.guild.get_role(role_remove))
         if reason is None:
-            await inter.response.send_message(msg or f"Muted {str(member)}.", ephemeral=EPHEMERAL)
+            await inter.response.send_message(msg or f"Muted {member.display_name}.", ephemeral=EPHEMERAL)
         else:
             await inter.response.send_message(
-                msg or f"Muted {member.name}#{member.discriminator}. Reason: {reason}",
+                msg or f"Muted {member.display_name}. Reason: {reason}",
                 ephemeral=EPHEMERAL)
 
     @staticmethod
     async def unmute(inter: ApplicationCommandInteraction, member: discord.Member, role_remove: int,
                      role_add: typing.Optional[int] = None, msg: str = None) -> bool:
         if inter.guild.get_role(role_remove) not in member.roles:
-            await inter.response.send_message(f"{member.name}#{member.discriminator} is not muted.",
+            await inter.response.send_message(f"{member.display_name} is not muted.",
                                               ephemeral=EPHEMERAL)
             return False
         else:
             if not isinstance(inter.guild.get_role(role_remove), discord.Role):
                 return False
             await member.remove_roles(inter.guild.get_role(role_remove))
             if role_add is not None:
                 with contextlib.suppress(discord.Forbidden, discord.HTTPException):
                     await member.add_roles(inter.guild.get_role(role_add))
-            await inter.response.send_message(msg or f"Unmuted {member.name}#{member.discriminator}.",
+            await inter.response.send_message(msg or f"Unmuted {member.display_name}.",
                                               ephemeral=EPHEMERAL)
             return True
 
     @staticmethod
     async def clear(inter: ApplicationCommandInteraction, amount: typing.Optional[int] = 99999999999999999,
                     msg: str = None) -> int:
         limit = datetime.datetime.now() - datetime.timedelta(weeks=2)
@@ -166,29 +166,29 @@
     @staticmethod
     async def kick(inter: ApplicationCommandInteraction, member: discord.Member,
                    reason: typing.Optional[str] = None, msg: str = None) -> None:
         if len(str(reason)) > 256:
             reason = reason[:256]
         await member.kick(reason=reason)
         if reason is None:
-            message = msg or f"Kicked {member.name}#{member.discriminator}."
+            message = msg or f"Kicked {member.display_name}."
         else:
-            message = msg or f"Kicked {member.name}#{member.discriminator}. Reason: {reason}"
+            message = msg or f"Kicked {member.display_name}. Reason: {reason}"
         await inter.response.send_message(message, ephemeral=EPHEMERAL)
 
     @staticmethod
     async def ban(inter: ApplicationCommandInteraction, member: discord.Member,
                   reason: typing.Optional[str] = None, msg: str = None) -> None:
         if len(str(reason)) > 256:
             reason = reason[:256]
         await member.ban(reason=reason)
         if reason is None:
-            message = msg or f"Banned {member.name}#{member.discriminator}."
+            message = msg or f"Banned {member.display_name}."
         else:
-            message = msg or f"Banned {member.name}#{member.discriminator}. Reason: {reason}"
+            message = msg or f"Banned {member.display_name}. Reason: {reason}"
         await inter.response.send_message(message, ephemeral=EPHEMERAL)
 
     @staticmethod
     async def timeout(inter: ApplicationCommandInteraction, member: discord.Member,
                       duration: Union[float, datetime.timedelta] = None, until: datetime.datetime = None,
                       reason: typing.Optional[str] = None, msg: str = None) -> None:
         if len(str(reason)) > 256:
@@ -201,47 +201,42 @@
                 end_timeout = utils.get_discord_date(
                     (datetime.datetime.now() + datetime.timedelta(seconds=duration)).timestamp())
         elif until is not None:
             await member.timeout(until=until, reason=reason)
             end_timeout = utils.get_discord_date(until.timestamp())
         else:
             await member.timeout(reason=reason)
-            await inter.response.send_message(f"Removed timeout from {str(member)}.", ephemeral=EPHEMERAL)
+            await inter.response.send_message(f"Removed timeout from {member.display_name}.", ephemeral=EPHEMERAL)
             return
         if reason is None:
-            message = msg or f"Timed out {str(member)} until {end_timeout}."
+            message = msg or f"Timed out {member.display_name} until {end_timeout}."
         else:
-            message = msg or f"Timed out {str(member)} until {end_timeout}. Reason: {reason}"
+            message = msg or f"Timed out {member.display_name} until {end_timeout}. Reason: {reason}"
         await inter.response.send_message(message, ephemeral=EPHEMERAL)
 
     @staticmethod
     async def softban(inter: ApplicationCommandInteraction, member: discord.Member,
                       reason: typing.Optional[str] = None, msg: str = None) -> None:
         if len(str(reason)) > 256:
             reason = reason[:256]
         await member.ban(reason=reason)
         if reason is None:
-            message = msg or f"Soft banned {member.name}#{member.discriminator}."
+            message = msg or f"Soft banned {member.display_name}."
         else:
-            message = msg or f"Soft banned {member.name}#{member.discriminator}. Reason: {reason}"
+            message = msg or f"Soft banned {member.display_name}. Reason: {reason}"
         await inter.response.send_message(message, ephemeral=EPHEMERAL)
         await member.unban()
 
     @staticmethod
     async def unban(inter: ApplicationCommandInteraction, member: typing.Union[str, int], msg: str = None) -> bool:
         bans = inter.guild.bans()
         if isinstance(member, int):
             ban = [ban async for ban in bans if ban.user.id == member]
         else:
-            try:
-                name, discrim = member.split("#")
-            except ValueError:
-                raise commands.errors.UserNotFound(member)
-            ban = [ban async for ban in bans if ban.user.discriminator ==
-                   discrim and ban.user.name == name]
+            ban = [ban async for ban in bans if ban.user.global_name == member]
         if not ban:
             await inter.response.send_message(f"{member} is not banned.", ephemeral=EPHEMERAL)
             return False
         await inter.guild.unban(ban[0].user)
         await inter.response.send_message(msg or f"Unbanned {member}.", ephemeral=EPHEMERAL)
         return True
 
@@ -751,15 +746,15 @@
                     if not isinstance(guild, discord.Guild):
                         async with db.execute("DELETE FROM tempban WHERE guild = ?", (str(guild_id),)):
                             pass
                         continue
                     time = datetime.datetime.fromisoformat(time_str)
                     if datetime.datetime.now() >= time:
                         async with db.execute("DELETE FROM tempban WHERE guild = ? and member = ? and time = ?",
-                                              (str(guild.id), str(member), time_str)):
+                                              (str(guild.id), member.display_name, time_str)):
                             pass
                         with contextlib.suppress(discord.Forbidden, discord.HTTPException):
                             await guild.unban(discord.Object(id=int(member)))
                 await db.commit()
 
     @staticmethod
     async def expire_loop() -> None:
```

### Comparing `dpys-5.5.8/dpys/utils.py` & `dpys-5.5.9/dpys/utils.py`

 * *Files identical despite different names*

### Comparing `dpys-5.5.8/dpys.egg-info/PKG-INFO` & `dpys-5.5.9/dpys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpys
-Version: 5.5.8
+Version: 5.5.9
 Summary: A library to simplify discord.py
 Home-page: https://jgltechnologies.com/dpys
 Author: George Luca
 Author-email: fixingg@gmail.com
 License: MIT
 Keywords: discord
 Platform: UNKNOWN
@@ -53,17 +53,17 @@
 <br>
 
 ```python
 import dpys
 from disnake.ext import commands
 
 bot = commands.AutoShardedBot(command_prefix="!")
-TOKEN = "Your Token
+TOKEN = "Your Token"
 
-bot.loop.create_task(dpys.setup(bot, DIR))
+bot.loop.create_task(dpys.setup(bot, "database directory"))
 bot.run()
 ```
 
 <br>
 
 Reaction role example
 
@@ -169,15 +169,15 @@
 ```
 
 <br>
 <br>
 
 # Documentation
 
-You will here 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
+You will hear 'mute remove role' mentioned a lot. This is just an optional role that gets removed when a member is
 muted, and added back when they are unmuted.
 
 ## Admin class
 
 Kick:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dpys Version: 5.5.8 Summary: A library to simplify
+Metadata-Version: 2.1 Name: dpys Version: 5.5.9 Summary: A library to simplify
 discord.py Home-page: https://jgltechnologies.com/dpys Author: George Luca
 Author-email: fixingg@gmail.com License: MIT Keywords: discord Platform:
 UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Description-Content-Type: text/
 markdown License-File: LICENSE [https://discord.com/api/guilds/
 844418702430175272/embed.png] # DPYS ## The goal of DPYS is to make basic
@@ -15,16 +15,16 @@
 can be given in [our Discord server](https://jgltechnologies.com/disnake). If
 you see any problems in the code or want to add a feature, create a pull
 request on [our Github repository](https://jgltechnologies.com/dpys/src).
 Install from pypi ``` python -m pip install dpys ```
 Install from github ``` python -m pip install git+https://github.com/
 JGLTechnologies/dpys ``` Setup
 ```python import dpys from disnake.ext import commands bot =
-commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token
-bot.loop.create_task(dpys.setup(bot, DIR)) bot.run() ```
+commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token"
+bot.loop.create_task(dpys.setup(bot, "database directory")) bot.run() ```
 Reaction role example
 ```python import dpys from disnake.ext import commands import disnake bot =
 commands.AutoShardedBot(command_prefix="!") TOKEN = "Your Token" # Do not type
 hint disnake.Role for the role argument # Command to create the reaction role
 @bot.slash_command(name="rr") async def reaction_role_command(inter:
 disnake.ApplicationCommandInteraction, emoji: str = commands.Param
 ( description="An emoji or list of emojis"), role: str = commands.Param
@@ -64,15 +64,15 @@
 when its message is deleted in channel.purge() @bot.listen
 ("on_raw_bulk_message_delete") async def rr_clear_on_raw_bulk_message_delete
 (payload): await dpys.rr.clear_on_raw_bulk_message_delete(payload) # Clears all
 DPYS data for a guild when it is removed @bot.listen("on_guild_remove") async
 def clear_on_guild_remove(guild): await dpys.misc.clear_data_on_guild_remove
 (guild) bot.loop.create_task(dpys.setup(bot, DIR)) bot.run(TOKEN) ```
 
-# Documentation You will here 'mute remove role' mentioned a lot. This is just
+# Documentation You will hear 'mute remove role' mentioned a lot. This is just
 an optional role that gets removed when a member is muted, and added back when
 they are unmuted. ## Admin class Kick: ```python async def kick(inter:
 disnake.ApplicationCommandInteraction, member: disnake.Member, reason:
 typing.Optional[str] = None, msg: str = None) -> None ``` ```python import dpys
 @bot.slash_command(name="kick") @commands.has_permissions(kick_members=True)
 async def kick(inter, member: disnake.Member = commands.Param(), reason: str =
 commands.Param(default=None)): await dpys.admin.kick(inter, member, reason) ```
```

### Comparing `dpys-5.5.8/setup.py` & `dpys-5.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 REQUIREMENTS = [
     "aiosqlite",
     "aiohttp",
     "disnake",
 ]
 DOCS = "https://jgltechnologies.com/dpys"
-VERSION = "5.5.8"
+VERSION = "5.5.9"
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
```

