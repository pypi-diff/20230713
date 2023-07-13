# Comparing `tmp/SempCode-2023.6.5.22.3942-py3-none-any.whl.zip` & `tmp/SempCode-2023.6.5.22.4886-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8961 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-10 12:58 Semp/Command.py
--rw-rw-rw-  2.0 fat     4155 b- defN 23-Jul-13 10:11 Semp/Progressbar.py
--rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-Jul-13 10:40 Semp/__init__.py
+Zip file size: 8775 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     1759 b- defN 23-Jul-13 12:01 Semp/Command.py
+-rw-rw-rw-  2.0 fat     4140 b- defN 23-Jul-13 12:12 Semp/Progressbar.py
+-rw-rw-rw-  2.0 fat     3341 b- defN 23-Jul-13 12:02 Semp/SempWrite.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-Jul-13 11:35 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
 -rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-13 10:11 Semp/test.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jul-11 09:21 Semp/EasyTkinter/__init__.py
--rw-rw-rw-  2.0 fat     1643 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      861 b- defN 23-Jul-13 10:40 SempCode-2023.6.5.22.3942.dist-info/RECORD
-11 files, 20873 bytes uncompressed, 7511 bytes compressed:  64.0%
+-rw-rw-rw-  2.0 fat     1750 b- defN 23-Jul-13 12:13 SempCode-2023.6.5.22.4886.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 12:13 SempCode-2023.6.5.22.4886.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-13 12:13 SempCode-2023.6.5.22.4886.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      861 b- defN 23-Jul-13 12:13 SempCode-2023.6.5.22.4886.dist-info/RECORD
+11 files, 21236 bytes uncompressed, 7325 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: Semp/test.py
 Comment: 
 
 Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-2023.6.5.22.3942.dist-info/METADATA
+Filename: SempCode-2023.6.5.22.4886.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-2023.6.5.22.3942.dist-info/WHEEL
+Filename: SempCode-2023.6.5.22.4886.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-2023.6.5.22.3942.dist-info/top_level.txt
+Filename: SempCode-2023.6.5.22.4886.dist-info/top_level.txt
 Comment: 
 
-Filename: SempCode-2023.6.5.22.3942.dist-info/RECORD
+Filename: SempCode-2023.6.5.22.4886.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/Command.py

```diff
@@ -1,22 +1,19 @@
-"""
-    SempCommand Alpha
-    Version:a109
-"""
 from subprocess import run
 from pathlib import Path
 from datetime import datetime
 from os import system
 
 
 EXIST_TRUE=True
 EXIST_FALSE=False
 class ModeError(Exception):
     def __init__(self, *args, **kwargs):
         pass
+
 class Commander:
     def __init__(self):
         super().__init__()
     def RunCommand(self,command: str = ...,shell: bool = True):
         run(command,shell=shell)
     def path_exist(self,path: str = ...):
         if Path(path).exists():
```

## Semp/Progressbar.py

```diff
@@ -1,11 +1,7 @@
-"""
-    Semp-Progressbar
-    v0.6.9
-"""
 from tqdm import trange,tqdm
 from time import sleep
 from requests import get
 from sys import set_int_max_str_digits as max
 from random import randint
 from pathlib import Path
 from tkinter import *
@@ -50,15 +46,15 @@
             pbar.set_postfix_str(f"{str(kb)}KB/s")
             f.write(chuck)
         f.close()
     else:
         try:
             temp=chunk_size+114514
         except:
-            raise ChunkError("Not a integer value")
+            raise ChunkError()
         else:
             for chuck in res.iter_content(chunk_size=chunk_size):
                 f.write(chuck)
                 pbar.update(len(chuck))
                 kb = chunk_size / 1024
                 pbar.set_postfix_str(f"{str(kb)}KB/s")
             f.close()
@@ -78,15 +74,15 @@
         self.label=Label(self.root,textvariable=self.word,font=("Segoe UI",16))
         self.label.pack()
         self.progress = DoubleVar()
         self.progressbar = Progressbar(self.root, variable=self.progress)
         self.progressbar.pack(fill=X)
         self.notice = Label(self.root,text=notice,fg="gray66")
         self.notice.pack(side=BOTTOM)
-        self.root.wm_resizable(0,0)
+        self.root.wm_resizable(False,False)
         self.root.wm_protocol("WM_DELETE_WINDOW",lambda :self.wmclose())
         OleDLL("shcore").SetProcessDpiAwareness(1)
         if bytes == True:
             self.Download("wb")
         else:
             self.Download("w")
     def update_progress(self, value):
@@ -94,20 +90,22 @@
         self.root.update()
 
     def close(self):
         self.root.destroy()
 
     def wmclose(self):
         warn("Cannot close window,please wait to download successfully.",ProgressbarWarning, stacklevel=2)
+
     def Download(self,mode:str = ...):
         self.r=get(self.url,stream=True)
         self.length=int(self.r.headers["content-length"])
         self.content=0
         self.f=open(self.name,mode)
         self.progressbar.configure(maximum=self.length)
         for chunk in self.r.iter_content(chunk_size=self.chunk_size):
             self.content += self.chunk_size
             self.update_progress(self.content)
             self.plan=round((self.content/self.length)*100,1)
-            self.word.set(f"{self.description}:{self.plan}% [{self.chunk_size/1024}KB/s]")
+            self.w="{0}:{1}% [{2}KB/s]".format(self.description,self.plan,self.chunk_size/1024)
+            self.word.set(self.w)
             self.f.write(chunk)
         self.close()
```

## Semp/SempWrite.py

```diff
@@ -1,17 +1,36 @@
-"""
-    Semp Write & Reader
-    Version:v0.2.6 Beta
-"""
-from . import Requester
+from requests import *
 
 
 BINARY_TRUE="binary_true_T_WriteBinary"
 BINARY_FALSE="binary_false_F_OnlyWrite"
 
+class Requester:
+    def __init__(self, website: str = ...):
+        super().__init__()
+        self.websitelink = website
+
+    def download(self, name: str = ..., binary=False):
+        self.r = get(self.websitelink)
+        if binary == True or binary == BINARY_TRUE:
+            with open(name, "wb") as f:
+                for chunk in self.r.iter_content(chunk_size=512):
+                    f.write(chunk)
+        # This method can download JPG file, EXE file, PNG file, etc
+        elif binary == False or binary == BINARY_FALSE:
+            with open(name, "wb") as f:
+                for chunk in self.r.iter_content(chunk_size=512):
+                    f.write(chunk)
+        # This method can download TXT file, JSON file, JS file, etc
+        else:
+            raise ValueError("Not " + str(name) + ".Expected BINARY_TRUE or BINARY_FALSE")
+
+    def responseget(self):
+        self.r = get(self.websitelink)
+        return {"status_code": self.r.status_code, "url": self.r.url, "text": self.r.text}
 
 class SempWrite:
     def __init__(self,filename,encoding="utf-8"):
         super().__init__()
         self.name_filename=filename
         self.encoding=encoding
     def ReadAndDeleteAllWord(self,binary=BINARY_FALSE):
@@ -27,20 +46,20 @@
             with open(self.name_filename,"wb",encoding=self.encoding) as f:
                 f.write("")
             return self.variable
         else:
             raise ValueError("Not be " + str(binary) + ".Expected BINARY_TRUE or BINARY_FALSE")
     def ResponseAndAddFile(self,website):
         self.response=Requester(website)
-        self.returned=self.response.ResponseGet()["text"]
+        self.returned=self.response.responseget()["text"]
         with open(self.name_filename,"a",encoding=self.encoding) as f:
             f.writelines(self.returned)
     def ResponseAndWriteFile(self,website):
         self.response=Requester(website)
-        self.returned=self.response.ResponseGet()["text"]
+        self.returned=self.response.responseget()["text"]
         with open(self.name_filename,"w",encoding=self.encoding) as f:
             f.write(self.returned)
     def OnlyRead(self):
         with open(self.name_filename,"r") as f:
             return f.read()
     def OnlyWrite(self,text):
         with open(self.name_filename,"w",encoding=self.encoding) as f:
@@ -53,10 +72,8 @@
             self.copy=f.read()
         with open(self.name_filename,"w",encoding=self.encoding) as f:
             f.write(self.copy)
     def config(self,filename=None,encoding=None):
         if filename != None:
             self.name_filename=filename
         if encoding != None:
-            self.encoding=encoding
-
-writer=SempWrite
+            self.encoding=encoding
```

## Semp/__init__.py

```diff
@@ -1,233 +1,213 @@
-"""
-    Semp Python Tool by Win12Home
-    Version:2023.06.05.22.3942 Beta
-    
-"""
-from PIL import Image,ImageTk
-from requests import *
-from sys import set_int_max_str_digits as max
-from subprocess import Popen
+from webbrowser import open_new_tab
+from requests import post, get
+from PIL import Image, ImageTk
+from subprocess import *
 from random import randint
 from datetime import datetime
-from webbrowser import open_new_tab
 
+BINARY_TRUE = "BTRUE"
+BINARY_FALSE = "BFALSE"
 
-max(0)
-BINARY_TRUE="BTRUE"
-BINARY_FALSE="BFALSE"
+AUTO = "AutoEnter"
+NONE = "NoEnter"
 
-AUTO="AutoEnter"
-NONE="NoEnter"
 
 class NumberError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
+
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
+
 class ArgumentError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
+
 class OtherError(Exception):
-    def __init__(self,*args,**kwargs):
+    def __init__(self, *args, **kwargs):
         pass
 
+
+class web_search:
+    def BingSearch(search):
+        open_new_tab(f"https://www.bing.com/search?q={search}")
+
+    def GoogleSearch(search):
+        open_new_tab(f"https://www.google.com/search?q={search}")
+
+
+def translator(text: str = ...):
+    url = 'http://fanyi.youdao.com/translate'
+    data = {
+        "i": text,
+        "from": "AUTO",
+        "to": "AUTO",
+        "smartresult": "dict",
+        "client": "fanyideskweb",
+        "salt": "16081210430989",
+        "doctype": "json",
+        "version": "2.1",
+        "keyfrom": "fanyi.web",
+        "action": "FY_BY_CLICKBUTTION"
+    }
+    try:
+        res = post(url, data=data).json()
+        sys = res['translateResult'][0][0]
+        inc = 0
+        word = ""
+        for __count in range(1000):
+            try:
+                word += res['translateResult'][0][inc]["tgt"]
+                word += " "
+                inc += 1
+            except:
+                break
+        return word
+    except:
+        raise OtherError("Request Error")
+
+
 def tkphoto(file: str = ...):
-    photo=Image.open(file)
-    #Open Photo
-    tkphoto=ImageTk.PhotoImage(image=photo)
-    #Save Photo
+    photo = Image.open(file)
+    # Open Photo
+    tkphoto = ImageTk.PhotoImage(image=photo)
+    # Save Photo
     return tkphoto
 
-def fromsnumber(b_from: int = 0,to: int = ...,passnum: int = 0):
-    a=[]
+
+def fromsnumber(b_from: int = 0, to: int = ..., passnum: int = 0):
+    a = []
     if passnum == None or passnum == 0:
-        for x in range(b_from,to+1):
+        for x in range(b_from, to + 1):
             a.append(x)
         return a
     else:
         try:
-            for x in range(b_from, to + 1,passnum):
+            for x in range(b_from, to + 1, passnum):
                 a.append(x)
             return a
         except:
             raise NumberError("Name error.")
 
+
 def createpassword(length: int = ...):
-    sslist=["0","1","2","3","4","5","6","7","8","9","^","%","a","A","B","c","C","d","E","f","D","F","g","H","i","j","K","l","M","N","o","P","q","Q","r","s"
-          ,"t","U","V","v","T","w","W","x","Y","z","!"]
-    password=""
-    temps=""
+    sslist = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "^", "%", "a", "A", "B", "c", "C", "d", "E", "f", "D",
+              "F", "g", "H", "i", "j", "K", "l", "M", "N", "o", "P", "q", "Q", "r", "s"
+        , "t", "U", "V", "v", "T", "w", "W", "x", "Y", "z", "!"]
+    password = ""
+    temps = ""
     for __count in range(length):
         for __count in range(5):
-            temps=sslist[randint(0,len(sslist)-1)]
-        password+=temps
+            temps = sslist[randint(0, len(sslist) - 1)]
+        password += temps
     return password
 
 
 class request_simplifies:
-    def download(*,website: str = ...,name: str = ...,binary=...):
+    def download(website: str = ..., name: str = ..., binary=...):
         r = get(website)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
-        #This method can download JPG file, EXE file, PNG file, etc
+        # This method can download JPG file, EXE file, PNG file, etc
         elif binary == False or binary == BINARY_FALSE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
-        #This method can download TXT file, JSON file, JS file, etc
+        # This method can download TXT file, JSON file, JS file, etc
         else:
-            raise BoolError("Not be "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
-    def responseget(*,website: str = ...):
-        r=get(website)
-        return {"Status_Code":r.status_code,"URL":r.url,"Text":r.text}
-
-def power_operation(num1: int = ...,num2: int = ...):
-    num=num1
-    for __count in range(num2-1):
-        num*=num1
+            raise BoolError("Not be " + str(name) + ".Expected BINARY_TRUE or BINARY_FALSE")
+
+    def responseget(website: str = ...):
+        r = get(website)
+        return {"Status_Code": r.status_code, "URL": r.url, "Text": r.text}
+
+
+def power_operation(num1: int = ..., num2: int = ...):
+    num = num1
+    for __count in range(num2 - 1):
+        num *= num1
     return num
 
- 
+
 def fibonacci_sequence(to: int = ...):
-    numlist=[1,1,1]
-    num=1
-    for __count in range(to-3):
-        num+=numlist[len(numlist)-2]
+    numlist = [1, 1, 1]
+    num = 1
+    for __count in range(to - 3):
+        num += numlist[len(numlist) - 2]
         numlist.append(num)
     return numlist
 
- 
+
 class requester:
-    def __init__(self,website: str = ...):
+    def __init__(self, website: str = ...):
         super().__init__()
-        self.websitelink=website
-    def download(self,name: str = ...,binary=False):
+        self.websitelink = website
+
+    def download(self, name: str = ..., binary=False):
         self.r = get(self.websitelink)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in self.r.iter_content(chunk_size=512):
                     f.write(chunk)
-        #This method can download JPG file, EXE file, PNG file, etc
+        # This method can download JPG file, EXE file, PNG file, etc
         elif binary == False or binary == BINARY_FALSE:
             with open(name, "wb") as f:
                 for chunk in self.r.iter_content(chunk_size=512):
                     f.write(chunk)
-        #This method can download TXT file, JSON file, JS file, etc
+        # This method can download TXT file, JSON file, JS file, etc
         else:
-            raise BoolError("Not "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
+            raise BoolError("Not " + str(name) + ".Expected BINARY_TRUE or BINARY_FALSE")
+
     def responseget(self):
-        self.r=get(self.websitelink)
-        return {"status_code":self.r.status_code,"url":self.r.url,"text":self.r.text}
+        self.r = get(self.websitelink)
+        return {"status_code": self.r.status_code, "url": self.r.url, "text": self.r.text}
+
 
- 
 def pythonprompt():
     Popen(
         "python.exe",
         shell=True,
         encoding="utf-8"
     )
 
- 
+
 def commandprompt():
     Popen(
         "cmd.exe",
         shell=True
     )
 
-def createmarkdown(title: str = ...,text: list[str] = ...,name: str = ...,auto: str = AUTO):
-    markdown=""
-    markdown+=f"---\n{title}\n---\n"
+def createmarkdown(title: str = ..., text: list[str] = ..., name: str = ..., auto: str = AUTO):
+    markdown = ""
+    markdown += f"---\n{title}\n---\n"
     if auto == AUTO:
         for word in text:
-            markdown+=f"{word}<br/>"
+            markdown += f"{word}<br/>"
             with open(name, "w") as f:
                 f.write(markdown)
     elif auto == NONE:
         for word in text:
-            markdown+=word
-        with open(name,"w") as f:
+            markdown += word
+        with open(name, "w") as f:
             f.write(markdown)
     else:
         raise ArgumentError("Not in AUTO or NONE")
 
-def gettime(format:str = "%Y.%m.%d %I:%M:%S %p"):
+def gettime(format: str = "%Y.%m.%d %I:%M:%S %p"):
     return datetime.now().strftime(format)
 
 def nowdate():
     return datetime.now()
 
-def date(year:int = ...,month:int = ...,day: int = ...):
-    return datetime(year,month,day)
+def date(year: int = ..., month: int = ..., day: int = ...):
+    return datetime(year, month, day)
 
 def dateweekday(datevar):
-    weekday={1:"Monday",2:"Tuesday",3:"Wednesday",4:"Thursday",5:"Friday",6:"Saturday",7:"Sunday"}
-    return weekday[int(datevar.isoweekday())]
-
-def translator(text: str = ...):
-    url = 'http://fanyi.youdao.com/translate'
-    data = {
-        "i": text,
-        "from": "AUTO",
-        "to": "AUTO",
-        "smartresult": "dict",
-        "client": "fanyideskweb",
-        "salt": "16081210430989",
-        "doctype": "json",
-        "version": "2.1",
-        "keyfrom": "fanyi.web",
-        "action": "FY_BY_CLICKBUTTION"
-    }
-    try:
-        res = post(url, data=data).json()
-        sys = res['translateResult'][0][0]
-        inc=0
-        word=""
-        for __count in range(1000):
-            try:
-                word += res['translateResult'][0][inc]["tgt"]
-                word += " "
-                inc+=1
-            except Exception:
-                break
-        return word
-    except:
-        raise OtherError("Request Error")
-
-class web_search:
-    def BingSearch(self,search:str = ...):
-        open_new_tab(f"https://cn.bing.com/search?q={search}")
-
-    def GoogleSearch(self,search:str = ...):
-        open_new_tab(f"https://www.google.com/search?q={search}")
-"""
-Here are some examples.
-Response(variable):
-    response=Requester("https://1.1.1.1/")
-    response.ResponseGet()
-Response(code):
-    request_simplifies.ResponseGet("https://1.1.1.1/")
-Fibonacci Sequence:
-    fibonacci_sequence(10)
-Power:
-    power_operation(10,5)
-All Numbers:
-    fromsnumber(5,135)
-Photo TK:
-    from tkinter import *
-    root=Tk()
-    root.title("Test")
-    img=PhotoTk("C:/test.jpg")
-    a=Label(self,image=img)
-    a.pack()
-    root.mainloop()
-Markdown Creator:
-    CreateMarkdown("Hello World!",["They are some example","They are some example"],"README.md")
-Translator:
-    Translator("Hello World!")
-"""
+    weekday = {1: "Monday", 2: "Tuesday", 3: "Wednesday", 4: "Thursday", 5: "Friday", 6: "Saturday", 7: "Sunday"}
+    return weekday[int(datevar.isoweekday())]
```

## Comparing `SempCode-2023.6.5.22.3942.dist-info/METADATA` & `SempCode-2023.6.5.22.4886.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SempCode
-Version: 2023.6.5.22.3942
+Version: 2023.6.5.22.4886
 Summary: Simplified the Python Code
 Author: 是真的Win12Home
 Author-email: mcdhj-work@outlook.com
 License: Mozilla Public License Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Requires: requests
 Requires: pillow
@@ -17,16 +17,18 @@
 Requires: tqdm
 Requires: warnings
 Description-Content-Type: text/markdown
 
 ---
 Hello Semp!
 ---
-Semp is can simple some code in Python.\
+Semp was simplified some code in Python.\
 **1.Updates**\
+*2023.06.05.22.4886(YearUpdate)*\
+Use pyi simplified Semp,Semp.Progressbar,Semp.SempWrite,Semp.Command\
 *2023.06.05.22.3942(YearUpdate)*\
 Fix some bugs\
 Add TkinterProgressbar(url:str,desc:str,title:str,name:str,chunk_size:int=512,bytes=True/False,is_parent=True/False,parent=None) in Semp.Progressbar\
 *v0.5.3.3(Update)*\
 Add Translator\
 Add Semp.Progressbar\
 ----Add VirtualProgressbar(description:str,time:int)\
```

