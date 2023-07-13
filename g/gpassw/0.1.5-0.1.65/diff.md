# Comparing `tmp/gpassw-0.1.5.tar.gz` & `tmp/gpassw-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpassw-0.1.5.tar", last modified: Thu Jul 13 07:10:43 2023, max compression
+gzip compressed data, was "gpassw-0.1.65.tar", last modified: Thu Jul 13 17:23:32 2023, max compression
```

## Comparing `gpassw-0.1.5.tar` & `gpassw-0.1.65.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.040542 gpassw-0.1.5/
--rw-rw-rw-   0        0        0     1784 2023-07-13 07:10:43.040542 gpassw-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.035530 gpassw-0.1.5/gpassw/
--rw-rw-rw-   0        0        0      817 2023-07-13 07:06:48.000000 gpassw-0.1.5/gpassw/functions.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:10:43.039539 gpassw-0.1.5/gpassw.egg-info/
--rw-rw-rw-   0        0        0     1784 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-13 07:10:43.000000 gpassw-0.1.5/gpassw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-13 07:10:42.000000 gpassw-0.1.5/gpassw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 07:10:43.041545 gpassw-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1924 2023-07-13 07:06:14.000000 gpassw-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:23:32.682522 gpassw-0.1.65/
+-rw-rw-rw-   0        0        0     2723 2023-07-13 17:23:32.683955 gpassw-0.1.65/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 17:23:32.676925 gpassw-0.1.65/gpassw/
+-rw-rw-rw-   0        0        0       13 2023-07-13 15:01:31.000000 gpassw-0.1.65/gpassw/config.py
+-rw-rw-rw-   0        0        0     2014 2023-07-13 17:11:18.000000 gpassw-0.1.65/gpassw/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:23:32.682522 gpassw-0.1.65/gpassw.egg-info/
+-rw-rw-rw-   0        0        0     2723 2023-07-13 17:23:32.000000 gpassw-0.1.65/gpassw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-13 17:23:32.000000 gpassw-0.1.65/gpassw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:23:32.000000 gpassw-0.1.65/gpassw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 17:23:32.000000 gpassw-0.1.65/gpassw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-13 17:23:32.000000 gpassw-0.1.65/gpassw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 17:23:32.683955 gpassw-0.1.65/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2023-07-13 17:23:26.000000 gpassw-0.1.65/setup.py
```

### Comparing `gpassw-0.1.5/PKG-INFO` & `gpassw-0.1.65/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: gpassw
-Version: 0.1.5
+Version: 0.1.65
 Summary: A very easy generator of passwords
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 # gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
+# Тестовая функция
+`password.check(password)` - тестовая функция. Возможно по некоторым причинам будет удалена, и в будущем добавлена с новыми возможностями!
+
 # Минимальный пример использования
 ```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
@@ -20,27 +23,36 @@
     from colorama import Style, Fore, init
     init()
 try: 
     from gpassw.functions import password
 except:
     system("pip install gpassw")
     from gpassw.functions import password
+    import gpassw.config as config
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = password.easy(10) #Генерация лёгкого пароля
-print(f"Мы подобрали тебе пароль - {password}
+passw = password.medium(10) #Генерация среднего пароля
+checking = password.check(passw) #Проверяем пароль на надёжность
+print(checking)
+if checking == None: #Если пароль надёжен на 100%
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+elif len(checking) < 2 or len(checking) == 2: #Если пароль ненадёжен на два пункта или меньше (Из 5)
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+else:
+    print(Fore.RED + "Ваш пароль ненадёжен." + Style.RESET_ALL) #Если пароль нёнадёжен на >2 пункта
+print(f"Мы подобрали тебе пароль - {passw}
 Окей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
 hello_password = input("Пароль: ")
-while hello_password != password:
+while hello_password != passw:
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
```

### Comparing `gpassw-0.1.5/gpassw.egg-info/PKG-INFO` & `gpassw-0.1.65/gpassw.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: gpassw
-Version: 0.1.5
+Version: 0.1.65
 Summary: A very easy generator of passwords
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 # gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
+# Тестовая функция
+`password.check(password)` - тестовая функция. Возможно по некоторым причинам будет удалена, и в будущем добавлена с новыми возможностями!
+
 # Минимальный пример использования
 ```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
@@ -20,27 +23,36 @@
     from colorama import Style, Fore, init
     init()
 try: 
     from gpassw.functions import password
 except:
     system("pip install gpassw")
     from gpassw.functions import password
+    import gpassw.config as config
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = password.easy(10) #Генерация лёгкого пароля
-print(f"Мы подобрали тебе пароль - {password}
+passw = password.medium(10) #Генерация среднего пароля
+checking = password.check(passw) #Проверяем пароль на надёжность
+print(checking)
+if checking == None: #Если пароль надёжен на 100%
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+elif len(checking) < 2 or len(checking) == 2: #Если пароль ненадёжен на два пункта или меньше (Из 5)
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+else:
+    print(Fore.RED + "Ваш пароль ненадёжен." + Style.RESET_ALL) #Если пароль нёнадёжен на >2 пункта
+print(f"Мы подобрали тебе пароль - {passw}
 Окей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
 hello_password = input("Пароль: ")
-while hello_password != password:
+while hello_password != passw:
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
```

### Comparing `gpassw-0.1.5/setup.py` & `gpassw-0.1.65/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup
 
 setup(
     name='gpassw',
-    version='0.1.5',
+    version='0.1.65',
     description='A very easy generator of passwords',
     packages=['gpassw'],
     author="barlin41k",
     author_email='sasaigrypocta@gmail.com',
     zip_safe=False,
     long_description='''# gpassw - генератор паролей!
 `gpassw` - очень простой в использовании генератор паролей для Вашех потребностей.
 
+# Тестовая функция
+`password.check(password)` - тестовая функция. Возможно по некоторым причинам будет удалена, и в будущем добавлена с новыми возможностями!
+
 # Минимальный пример использования
 ```python
 from os import system
 try: 
     from colorama import Style, Fore, init
     init()
 except:
@@ -22,26 +25,35 @@
     from colorama import Style, Fore, init
     init()
 try: 
     from gpassw.functions import password
 except:
     system("pip install gpassw")
     from gpassw.functions import password
+    import gpassw.config as config
 
 name = input("Напиши своё имя: ")
 print(f"Привет, {name}! Сейчас подберём для тебя оптимальный пароль...")
-password = password.easy(10) #Генерация лёгкого пароля
-print(f"Мы подобрали тебе пароль - {password}\nОкей?")
+passw = password.medium(10) #Генерация среднего пароля
+checking = password.check(passw) #Проверяем пароль на надёжность
+print(checking)
+if checking == None: #Если пароль надёжен на 100%
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+elif len(checking) < 2 or len(checking) == 2: #Если пароль ненадёжен на два пункта или меньше (Из 5)
+    print(Fore.GREEN + "Ваш пароль надёжен." + Style.RESET_ALL)
+else:
+    print(Fore.RED + "Ваш пароль ненадёжен." + Style.RESET_ALL) #Если пароль нёнадёжен на >2 пункта
+print(f"Мы подобрали тебе пароль - {passw}\nОкей?")
 answer = input("Да/Нет: ")
 if answer == "Да" or answer == "да":
     print("Теперь напиши пароль, который мы тебе подобрали для входа в аккаунт.")
 else:
     raise SystemExit(1)
 hello_password = input("Пароль: ")
-while hello_password != password:
+while hello_password != passw:
     print(Fore.RED + "Пароль неверный." + Style.RESET_ALL)
     hello_password = input("Пароль: ")
 print("Вы успешно вошли!")
 ```
 
 # Как установить?
 Всего лишь требуеться просто прописать команду в консоли: `pip install gpassw`
```

