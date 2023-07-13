# Comparing `tmp/SempCode-0.5.5-py3-none-any.whl.zip` & `tmp/SempCode-2023.6.5.22.3942-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 7766 bytes, number of entries: 10
+Zip file size: 8961 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-10 12:58 Semp/Command.py
--rw-rw-rw-  2.0 fat     1814 b- defN 23-Jul-12 09:22 Semp/Progressbar.py
+-rw-rw-rw-  2.0 fat     4155 b- defN 23-Jul-13 10:11 Semp/Progressbar.py
 -rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     6606 b- defN 23-Jul-12 09:22 Semp/__init__.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-Jul-13 10:40 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-13 10:11 Semp/test.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jul-11 09:21 Semp/EasyTkinter/__init__.py
--rw-rw-rw-  2.0 fat     1381 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      750 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/RECORD
-10 files, 17860 bytes uncompressed, 6504 bytes compressed:  63.6%
+-rw-rw-rw-  2.0 fat     1643 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      861 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/RECORD
+11 files, 20873 bytes uncompressed, 7511 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: Semp/__init__.py
 Comment: 
 
 Filename: Semp/about.py
 Comment: 
 
+Filename: Semp/test.py
+Comment: 
+
 Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-0.5.5.dist-info/METADATA
+Filename: SempCode-2023.6.5.22.3942.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-0.5.5.dist-info/WHEEL
+Filename: SempCode-2023.6.5.22.3942.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-0.5.5.dist-info/top_level.txt
+Filename: SempCode-2023.6.5.22.3942.dist-info/top_level.txt
 Comment: 
 
-Filename: SempCode-0.5.5.dist-info/RECORD
+Filename: SempCode-2023.6.5.22.3942.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/Progressbar.py

```diff
@@ -1,22 +1,29 @@
 """
     Semp-Progressbar
-    v0.6.5
+    v0.6.9
 """
 from tqdm import trange,tqdm
-from tqdm.gui import tqdm as guitqdm
 from time import sleep
 from requests import get
 from sys import set_int_max_str_digits as max
-from pathlib import Path
 from random import randint
+from pathlib import Path
+from tkinter import *
+from tkinter.ttk import Progressbar
+from warnings import warn
+from ctypes import OleDLL
 
 
 max(0)
-class ChunkError:
+class ChunkError(Exception):
+    def __init__(self,*args,**kwargs):
+        pass
+
+class ProgressbarWarning(Warning):
     def __init__(self,*args,**kwargs):
         pass
 
 def VirtualProgressbar(description:str = ...,time:int = 0.1):
     bar=tqdm(range(100))
     bar.set_description(description)
     for x in bar:
@@ -51,7 +58,56 @@
         else:
             for chuck in res.iter_content(chunk_size=chunk_size):
                 f.write(chuck)
                 pbar.update(len(chuck))
                 kb = chunk_size / 1024
                 pbar.set_postfix_str(f"{str(kb)}KB/s")
             f.close()
+
+
+class TkinterProgressBar:
+    def __init__(self,url:str = ...,desc:str = ...,title:str = ...,name:str = ...,chunk_size:int = 512,bytes: bool = False,is_parent: bool = True,parent:type = None,notice:str = ""):
+        warn("This is Alpha Project in SempCode",ProgressbarWarning, stacklevel=2)
+        self.url,self.name,self.chunk_size,self.description=url,name,chunk_size,desc
+        if is_parent == True:
+            self.root=Tk()
+        else:
+            self.root = Toplevel(parent)
+        self.root.wm_geometry("600x400")
+        self.root.wm_title(title)
+        self.word = StringVar()
+        self.label=Label(self.root,textvariable=self.word,font=("Segoe UI",16))
+        self.label.pack()
+        self.progress = DoubleVar()
+        self.progressbar = Progressbar(self.root, variable=self.progress)
+        self.progressbar.pack(fill=X)
+        self.notice = Label(self.root,text=notice,fg="gray66")
+        self.notice.pack(side=BOTTOM)
+        self.root.wm_resizable(0,0)
+        self.root.wm_protocol("WM_DELETE_WINDOW",lambda :self.wmclose())
+        OleDLL("shcore").SetProcessDpiAwareness(1)
+        if bytes == True:
+            self.Download("wb")
+        else:
+            self.Download("w")
+    def update_progress(self, value):
+        self.progress.set(value)
+        self.root.update()
+
+    def close(self):
+        self.root.destroy()
+
+    def wmclose(self):
+        warn("Cannot close window,please wait to download successfully.",ProgressbarWarning, stacklevel=2)
+    def Download(self,mode:str = ...):
+        self.r=get(self.url,stream=True)
+        self.length=int(self.r.headers["content-length"])
+        self.content=0
+        self.f=open(self.name,mode)
+        self.progressbar.configure(maximum=self.length)
+        for chunk in self.r.iter_content(chunk_size=self.chunk_size):
+            self.content += self.chunk_size
+            self.update_progress(self.content)
+            self.plan=round((self.content/self.length)*100,1)
+            self.word.set(f"{self.description}:{self.plan}% [{self.chunk_size/1024}KB/s]")
+            self.f.write(chunk)
+        self.close()
```

## Semp/__init__.py

```diff
@@ -1,19 +1,19 @@
 """
     Semp Python Tool by Win12Home
-    Version:0.5.3.3 Beta
+    Version:2023.06.05.22.3942 Beta
     
 """
 from PIL import Image,ImageTk
 from requests import *
 from sys import set_int_max_str_digits as max
 from subprocess import Popen
 from random import randint
 from datetime import datetime
-from time import time
+from webbrowser import open_new_tab
 
 
 max(0)
 BINARY_TRUE="BTRUE"
 BINARY_FALSE="BFALSE"
 
 AUTO="AutoEnter"
@@ -26,19 +26,20 @@
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
 class ArgumentError(Exception):
     def __init__(self, *args, **kwargs):
         pass
+
 class OtherError(Exception):
     def __init__(self,*args,**kwargs):
         pass
 
-def PhotoTk(file: str = ...):
+def tkphoto(file: str = ...):
     photo=Image.open(file)
     #Open Photo
     tkphoto=ImageTk.PhotoImage(image=photo)
     #Save Photo
     return tkphoto
 
 def fromsnumber(b_from: int = 0,to: int = ...,passnum: int = 0):
@@ -51,42 +52,42 @@
         try:
             for x in range(b_from, to + 1,passnum):
                 a.append(x)
             return a
         except:
             raise NumberError("Name error.")
 
-def CreatePassword(length: int = ...):
+def createpassword(length: int = ...):
     sslist=["0","1","2","3","4","5","6","7","8","9","^","%","a","A","B","c","C","d","E","f","D","F","g","H","i","j","K","l","M","N","o","P","q","Q","r","s"
           ,"t","U","V","v","T","w","W","x","Y","z","!"]
     password=""
     temps=""
     for __count in range(length):
         for __count in range(5):
             temps=sslist[randint(0,len(sslist)-1)]
         password+=temps
     return password
 
 
 class request_simplifies:
-    def Download(website: str = ...,name: str = ...,binary=...):
+    def download(*,website: str = ...,name: str = ...,binary=...):
         r = get(website)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
         #This method can download JPG file, EXE file, PNG file, etc
         elif binary == False or binary == BINARY_FALSE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
         #This method can download TXT file, JSON file, JS file, etc
         else:
             raise BoolError("Not be "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
-    def ResponseGet(website: str = ...):
+    def responseget(*,website: str = ...):
         r=get(website)
         return {"Status_Code":r.status_code,"URL":r.url,"Text":r.text}
 
 def power_operation(num1: int = ...,num2: int = ...):
     num=num1
     for __count in range(num2-1):
         num*=num1
@@ -98,52 +99,52 @@
     num=1
     for __count in range(to-3):
         num+=numlist[len(numlist)-2]
         numlist.append(num)
     return numlist
 
  
-class Requester:
+class requester:
     def __init__(self,website: str = ...):
         super().__init__()
         self.websitelink=website
-    def Download(self,name: str = ...,binary=False):
+    def download(self,name: str = ...,binary=False):
         self.r = get(self.websitelink)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in self.r.iter_content(chunk_size=512):
                     f.write(chunk)
         #This method can download JPG file, EXE file, PNG file, etc
         elif binary == False or binary == BINARY_FALSE:
             with open(name, "wb") as f:
                 for chunk in self.r.iter_content(chunk_size=512):
                     f.write(chunk)
         #This method can download TXT file, JSON file, JS file, etc
         else:
             raise BoolError("Not "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
-    def ResponseGet(self):
+    def responseget(self):
         self.r=get(self.websitelink)
         return {"status_code":self.r.status_code,"url":self.r.url,"text":self.r.text}
 
  
-def PyPrompt():
+def pythonprompt():
     Popen(
         "python.exe",
         shell=True,
         encoding="utf-8"
     )
 
  
-def CmdPrompt():
+def commandprompt():
     Popen(
         "cmd.exe",
         shell=True
     )
 
-def CreateMarkdown(title: str = ...,text: list[str] = ...,name: str = ...,auto: str = AUTO):
+def createmarkdown(title: str = ...,text: list[str] = ...,name: str = ...,auto: str = AUTO):
     markdown=""
     markdown+=f"---\n{title}\n---\n"
     if auto == AUTO:
         for word in text:
             markdown+=f"{word}<br/>"
             with open(name, "w") as f:
                 f.write(markdown)
@@ -151,28 +152,28 @@
         for word in text:
             markdown+=word
         with open(name,"w") as f:
             f.write(markdown)
     else:
         raise ArgumentError("Not in AUTO or NONE")
 
-def GetTime(format:str = "%Y.%m.%d %I:%M:%S %p"):
+def gettime(format:str = "%Y.%m.%d %I:%M:%S %p"):
     return datetime.now().strftime(format)
 
-def NowDate():
+def nowdate():
     return datetime.now()
 
-def Date(year:int = ...,month:int = ...,day: int = ...):
+def date(year:int = ...,month:int = ...,day: int = ...):
     return datetime(year,month,day)
 
-def DateWeekday(datevar):
+def dateweekday(datevar):
     weekday={1:"Monday",2:"Tuesday",3:"Wednesday",4:"Thursday",5:"Friday",6:"Saturday",7:"Sunday"}
     return weekday[int(datevar.isoweekday())]
 
-def Translator(text: str = ...):
+def translator(text: str = ...):
     url = 'http://fanyi.youdao.com/translate'
     data = {
         "i": text,
         "from": "AUTO",
         "to": "AUTO",
         "smartresult": "dict",
         "client": "fanyideskweb",
@@ -194,14 +195,20 @@
                 inc+=1
             except Exception:
                 break
         return word
     except:
         raise OtherError("Request Error")
 
+class web_search:
+    def BingSearch(self,search:str = ...):
+        open_new_tab(f"https://cn.bing.com/search?q={search}")
+
+    def GoogleSearch(self,search:str = ...):
+        open_new_tab(f"https://www.google.com/search?q={search}")
 """
 Here are some examples.
 Response(variable):
     response=Requester("https://1.1.1.1/")
     response.ResponseGet()
 Response(code):
     request_simplifies.ResponseGet("https://1.1.1.1/")
```

## Comparing `SempCode-0.5.5.dist-info/METADATA` & `SempCode-2023.6.5.22.3942.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: SempCode
-Version: 0.5.5
+Version: 2023.6.5.22.3942
 Summary: Simplified the Python Code
 Author: 是真的Win12Home
 Author-email: mcdhj-work@outlook.com
 License: Mozilla Public License Version 2.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires: requests
 Requires: pillow
 Requires: pathlib
 Requires: subprocess
 Requires: datetime
 Requires: ctypes
 Requires: ttkthemes
 Requires: random
+Requires: tqdm
+Requires: warnings
 Description-Content-Type: text/markdown
 
 ---
 Hello Semp!
 ---
 Semp is can simple some code in Python.\
 **1.Updates**\
+*2023.06.05.22.3942(YearUpdate)*\
+Fix some bugs\
+Add TkinterProgressbar(url:str,desc:str,title:str,name:str,chunk_size:int=512,bytes=True/False,is_parent=True/False,parent=None) in Semp.Progressbar\
 *v0.5.3.3(Update)*\
 Add Translator\
 Add Semp.Progressbar\
 ----Add VirtualProgressbar(description:str,time:int)\
 ----Add EasyProgressbar() Notice:Default VirtualProgressbar\
 ----Add DownloadProgressbar(description:str,website:str,name:str,chunk_size:int=None)\
 *v0.5.2.13(Update)*\
```

