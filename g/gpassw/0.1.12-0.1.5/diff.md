# Comparing `tmp/gpassw-0.1.12.tar.gz` & `tmp/gpassw-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpassw-0.1.12.tar", last modified: Wed Jul 12 13:26:30 2023, max compression
+gzip compressed data, was "gpassw-0.1.5.tar", last modified: Thu Jul 13 07:10:43 2023, max compression
```

## Comparing `gpassw-0.1.12.tar` & `gpassw-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:26:30.140628 gpassw-0.1.12/
--rw-rw-rw-   0        0        0     1773 2023-07-12 13:26:30.140628 gpassw-0.1.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 13:26:30.135963 gpassw-0.1.12/gpassw/
--rw-rw-rw-   0        0        0      366 2023-07-12 13:07:39.000000 gpassw-0.1.12/gpassw/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:26:30.139628 gpassw-0.1.12/gpassw.egg-info/
--rw-rw-rw-   0        0        0     1773 2023-07-12 13:26:30.000000 gpassw-0.1.12/gpassw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-12 13:26:30.000000 gpassw-0.1.12/gpassw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:26:30.000000 gpassw-0.1.12/gpassw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-12 13:16:52.000000 gpassw-0.1.12/gpassw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-12 13:26:30.000000 gpassw-0.1.12/gpassw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:26:30.141813 gpassw-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0     1913 2023-07-12 13:26:22.000000 gpassw-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.040542 gpassw-0.1.5/
+-rw-rw-rw-   0        0        0     1784 2023-07-13 07:10:43.040542 gpassw-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.035530 gpassw-0.1.5/gpassw/
+-rw-rw-rw-   0        0        0      817 2023-07-13 07:06:48.000000 gpassw-0.1.5/gpassw/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.039539 gpassw-0.1.5/gpassw.egg-info/
+-rw-rw-rw-   0        0        0     1784 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-13 07:10:43.000000 gpassw-0.1.5/gpassw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:10:43.041545 gpassw-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1924 2023-07-13 07:06:14.000000 gpassw-0.1.5/setup.py
```

### Comparing `gpassw-0.1.12/PKG-INFO` & `gpassw-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: gpassw
-Version: 0.1.12
+Version: 0.1.5
 Summary: A very easy generator of passwords
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 # gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
 # Минимальный пример использования
-```
+```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
     system("pip install colorama")
     from colorama import Style, Fore, init
     init()
 try: 
-    from gpassw.functions import Password
+    from gpassw.functions import password
 except:
     system("pip install gpassw")
-    from gpassw.functions import Password
+    from gpassw.functions import password
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = Password.get(10) #Генерация пароля из букв
+password = password.easy(10) #Генерация лёгкого пароля
 print(f"Мы подобрали тебе пароль - {password}
 Окей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
@@ -40,8 +40,10 @@
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
+
+
```

### Comparing `gpassw-0.1.12/gpassw.egg-info/PKG-INFO` & `gpassw-0.1.5/gpassw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: gpassw
-Version: 0.1.12
+Version: 0.1.5
 Summary: A very easy generator of passwords
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 # gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
 # Минимальный пример использования
-```
+```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
     system("pip install colorama")
     from colorama import Style, Fore, init
     init()
 try: 
-    from gpassw.functions import Password
+    from gpassw.functions import password
 except:
     system("pip install gpassw")
-    from gpassw.functions import Password
+    from gpassw.functions import password
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = Password.get(10) #Генерация пароля из букв
+password = password.easy(10) #Генерация лёгкого пароля
 print(f"Мы подобрали тебе пароль - {password}
 Окей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
@@ -40,8 +40,10 @@
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
+
+
```

### Comparing `gpassw-0.1.12/setup.py` & `gpassw-0.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from setuptools import setup
 
 setup(
     name='gpassw',
-    version='0.1.12',
+    version='0.1.5',
     description='A very easy generator of passwords',
     packages=['gpassw'],
     author="barlin41k",
     author_email='sasaigrypocta@gmail.com',
     zip_safe=False,
     long_description='''# gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
 # Минимальный пример использования
-```
+```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
     system("pip install colorama")
     from colorama import Style, Fore, init
     init()
 try: 
-    from gpassw.functions import Password
+    from gpassw.functions import password
 except:
     system("pip install gpassw")
-    from gpassw.functions import Password
+    from gpassw.functions import password
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = Password.get(10) #Генерация пароля из букв
+password = password.easy(10) #Генерация лёгкого пароля
 print(f"Мы подобрали тебе пароль - {password}\nОкей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
 hello_password = input("Пароль: ")
@@ -41,10 +41,12 @@
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
+
+
     ''',
     long_description_content_type="text/markdown",
     )
```

