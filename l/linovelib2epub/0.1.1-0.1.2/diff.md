# Comparing `tmp/linovelib2epub-0.1.1-py3-none-any.whl.zip` & `tmp/linovelib2epub-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 36091 bytes, number of entries: 18
+Zip file size: 37729 bytes, number of entries: 18
 -rw-r--r--  2.0 fat       23 b- defN 20-Feb-02 00:00 linovelib2epub/__about__.py
 -rw-r--r--  2.0 fat       62 b- defN 20-Feb-02 00:00 linovelib2epub/__init__.py
 -rw-r--r--  2.0 fat      120 b- defN 20-Feb-02 00:00 linovelib2epub/exceptions.py
--rw-r--r--  2.0 fat    15260 b- defN 20-Feb-02 00:00 linovelib2epub/linovel.py
--rw-r--r--  2.0 fat     5086 b- defN 20-Feb-02 00:00 linovelib2epub/logger.py
--rw-r--r--  2.0 fat     2680 b- defN 20-Feb-02 00:00 linovelib2epub/models.py
+-rw-r--r--  2.0 fat    17331 b- defN 20-Feb-02 00:00 linovelib2epub/linovel.py
+-rw-r--r--  2.0 fat     2799 b- defN 20-Feb-02 00:00 linovelib2epub/logger.py
+-rw-r--r--  2.0 fat     3349 b- defN 20-Feb-02 00:00 linovelib2epub/models.py
 -rw-r--r--  2.0 fat     1246 b- defN 20-Feb-02 00:00 linovelib2epub/settings.py
 -rw-r--r--  2.0 fat     3522 b- defN 20-Feb-02 00:00 linovelib2epub/utils.py
 -rw-r--r--  2.0 fat      331 b- defN 20-Feb-02 00:00 linovelib2epub/spider/__init__.py
--rw-r--r--  2.0 fat     8818 b- defN 20-Feb-02 00:00 linovelib2epub/spider/base_spider.py
--rw-r--r--  2.0 fat    16015 b- defN 20-Feb-02 00:00 linovelib2epub/spider/linovelib_mobile_spider.py
+-rw-r--r--  2.0 fat     9144 b- defN 20-Feb-02 00:00 linovelib2epub/spider/base_spider.py
+-rw-r--r--  2.0 fat    23200 b- defN 20-Feb-02 00:00 linovelib2epub/spider/linovelib_mobile_spider.py
 -rw-r--r--  2.0 fat      812 b- defN 20-Feb-02 00:00 linovelib2epub/styles/chapter.css
 -rw-r--r--  2.0 fat      295 b- defN 20-Feb-02 00:00 linovelib2epub/styles/cover.css
 -rw-r--r--  2.0 fat      368 b- defN 20-Feb-02 00:00 linovelib2epub/styles/nav.css
-?rw-r--r--  2.0 fat    10452 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat    35176 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     1537 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.1.dist-info/RECORD
-18 files, 101890 bytes uncompressed, 33557 bytes compressed:  67.1%
+?rw-r--r--  2.0 fat    11153 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat    35176 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     1537 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/RECORD
+18 files, 110555 bytes uncompressed, 35195 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: linovelib2epub/styles/cover.css
 Comment: 
 
 Filename: linovelib2epub/styles/nav.css
 Comment: 
 
-Filename: linovelib2epub-0.1.1.dist-info/METADATA
+Filename: linovelib2epub-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: linovelib2epub-0.1.1.dist-info/WHEEL
+Filename: linovelib2epub-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: linovelib2epub-0.1.1.dist-info/licenses/LICENSE
+Filename: linovelib2epub-0.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: linovelib2epub-0.1.1.dist-info/RECORD
+Filename: linovelib2epub-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## linovelib2epub/__about__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

## linovelib2epub/linovel.py

```diff
@@ -42,14 +42,17 @@
         author = novel.author
         cover_file = self.epub_settings["image_download_folder"] + "/" + novel.book_cover_local
 
         if not self.epub_settings["divide_volume"]:
             self._write_epub(book_title, author, novel.volumes, cover_file)
         else:
             for volume in novel.volumes:
+                # if volume image folder is not empty, then use the first image as the cover
+                if volume["volume_cover"]:
+                    cover_file = f'{self.epub_settings["image_download_folder"]}/{volume["volume_cover"]}'
                 self._write_epub(f'{book_title}_{volume["title"]}', author, volume, cover_file)
 
         # tips: show output file folder
         output_folder = os.path.join(os.getcwd(), self._get_output_folder())
         self.logger.info('(Perf metrics) Write epub took: {} seconds'.format(time.perf_counter() - start))
         rich_print(f"The output epub is located in [link={output_folder}]this folder[/link]. "
                    f"(You can see the link if you use a modern shell.)")
@@ -57,15 +60,15 @@
     def _write_epub(self, title, author, volumes, cover_file, cover_filename: str = None):
         """
 
         :param title: for one epub has many volumes, the title should be book title.
            for one epub per volume, the title should be volume title.
         :param author:
         :param volumes: if divide_volume is False, this parameter should be volume list(List[LightNovelVolume]).
-           if divide_volume is True, it should be one volum(LightNovelVolume).
+           if divide_volume is True, it should be one volume(LightNovelVolume).
         :param cover_file: local image file path
         :param cover_filename: cover_filename has no format suffix such as ".jpg"
         :return:
         """
 
         book = epub.EpubBook()
         # epub basic info
@@ -89,56 +92,82 @@
         def _write_volume(book, custom_style_chapter, default_style_chapter, volume, volume_title):
             # reset content
             write_content = ""
             # use outer scope counters
             nonlocal chapter_index
             nonlocal file_index
 
-            html_volume_title = "<h1>" + volume_title + "</h1>"
-            write_content += html_volume_title
-            book.toc.append([epub.Section(volume_title), []])
+            if not self.epub_settings["divide_volume"]:
+                # volume_title as h1
+                html_volume_title = "<h1>" + volume_title + "</h1>"
+                write_content += html_volume_title
+                book.toc.append([epub.Link(f"{file_index + 1}.xhtml", volume_title, str(uuid.uuid4())), []])
+
             chapter_index += 1
             for chapter in volume['chapters']:
                 file_index += 1
                 chapter_title = chapter['title']
 
-                html_chapter_title = "<h2>" + chapter_title + "</h2>"
-                write_content += html_chapter_title + str(chapter["content"]).replace(
-                    """<div class="acontent" id="acontent">""", "")
+                if not self.epub_settings["divide_volume"]:
+                    # chapter_title as h2
+                    html_chapter_title = "<h2>" + chapter_title + "</h2>"
+                    write_content += html_chapter_title + str(chapter["content"]).replace(
+                        """<div class="acontent" id="acontent">""", "")
+                else:
+                    # chapter_title as h1
+                    html_chapter_title = "<h1>" + chapter_title + "</h1>"
+                    write_content += html_chapter_title + str(chapter["content"]).replace(
+                        """<div class="acontent" id="acontent">""", "")
+
                 write_content = write_content.replace('png', 'jpg')
 
                 page = epub.EpubHtml(title=chapter_title, file_name=f"{file_index}.xhtml", lang="zh")
                 page.set_content(write_content)
 
                 # add `<link>` tag to page `<head>` section.
                 self._set_page_style(book, custom_style_chapter, default_style_chapter, page)
 
-                book.toc[chapter_index][1].append(page)
+                if not self.epub_settings["divide_volume"]:
+                    # volume_title as h1
+                    book.toc[chapter_index][1].append(page)
+                else:
+                    # chapter_title as h1
+                    book.toc.append(epub.Link(f"{file_index}.xhtml", chapter_title, str(uuid.uuid4())))
+
                 book.spine.append(page)
 
                 write_content = ""
 
         if not self.epub_settings["divide_volume"]:
+            volume_img_folders = ""
             for volume in volumes:
                 volume_title = volume['title']
                 _write_volume(book, custom_style_chapter, default_style_chapter, volume, volume_title)
         else:
             create_folder_if_not_exists(self._novel_book_title)
             volume = volumes
             volume_title = title
+            volume_img_folders = volume['volume_img_folders']
             _write_volume(book, custom_style_chapter, default_style_chapter, volume, volume_title)
 
         # DEFAULT CHAPTER STYLE & CUSTOM CHAPTER STYLE
         book.add_item(default_style_chapter)
         if custom_style_chapter:
             book.add_item(custom_style_chapter)
 
         # IMAGES
         images_folder = self.epub_settings["image_download_folder"]
-        self._add_images(book, images_folder)
+        # handle volume_img_folders
+        if volume_img_folders == "":
+            volume_img_folder = volume_img_folders
+            self._add_images(book, images_folder, volume_img_folder)
+        else:
+            # now volume_img_folders is a collection
+            for folder in volume_img_folders:
+                self._add_images(book, images_folder, folder)
 
         book.add_item(epub.EpubNcx())
         book.add_item(epub.EpubNav())
 
         # COVER STYLE
         cover_html = book.get_item_with_id('cover')
         self._set_default_cover_style(book, cover_html)
@@ -150,45 +179,59 @@
         self._set_default_nav_style(book, nav_html)
         if self.epub_settings["custom_style_nav"]:
             self._set_custom_nav_style(book, nav_html)
 
         # FINAL WRITE
         # if divide volume, create a folder named title, or leave folder as "“
         out_folder = self._get_output_folder()
-        epub.write_epub(sanitize_pathname(out_folder) + "/" + sanitize_pathname(title) + '.epub', book)
+        if not self.epub_settings["divide_volume"]:
+            prefix = ""
+        else:
+            prefix = "%02d." % volume['vid']
+
+        epub.write_epub(sanitize_pathname(out_folder) + "/" + prefix + sanitize_pathname(title) + '.epub', book)
 
     @staticmethod
     def _set_page_style(book, custom_style_chapter, default_style_chapter, page):
         page.add_item(default_style_chapter)
         if custom_style_chapter:
             page.add_item(custom_style_chapter)
         book.add_item(page)
 
-    def _add_images(self, book, images_folder):
+    def _add_images(self, book, images_folder, volume_img_folder):
+        def _add_image(image_file):
+            if not ((".jpg" or ".png" or ".webp" or ".jpeg" or ".bmp" or "gif") in str(image_file)):
+                return
+            try:
+                img = Image.open(f'{images_folder}/{volume_img_folder}/{image_file}')
+            except (Exception,):
+                return
+
+            b = io.BytesIO()
+            img = img.convert('RGB')
+            img.save(b, 'jpeg')
+            data_img = b.getvalue()
+
+            new_image_file = image_file.replace('png', 'jpg')
+            img = epub.EpubItem(file_name=f'{images_folder}/{volume_img_folder}/{new_image_file}',
+                                media_type="image/jpeg",
+                                content=data_img)
+            book.add_item(img)
+
         if self.epub_settings["has_illustration"]:
-            image_files = os.listdir(images_folder)
-            # THINK: if enable multi Linovel instances, need to make sure images_folder corresponds to a seperate instance.
-            # Or it will add all images into a certain epub.
-            for image_file in image_files:
-                if not ((".jpg" or ".png" or ".webp" or ".jpeg" or ".bmp" or "gif") in str(image_file)):
-                    continue
-                try:
-                    img = Image.open(images_folder + '/' + image_file)
-                except (Exception,):
-                    continue
-
-                b = io.BytesIO()
-                img = img.convert('RGB')
-                img.save(b, 'jpeg')
-                data_img = b.getvalue()
-
-                new_image_file = image_file.replace('png', 'jpg')
-                img = epub.EpubItem(file_name=f"{images_folder}/{new_image_file}", media_type="image/jpeg",
-                                    content=data_img)
-                book.add_item(img)
+            if not self.epub_settings["divide_volume"]:
+                # grab all images under all [volume_img_folder]
+                for volume_img_folder in os.listdir(images_folder):
+                    for image_file in os.listdir(f'{images_folder}/{volume_img_folder}'):
+                        _add_image(image_file)
+            else:
+                # only grab images under current [volume_img_folder]
+                if volume_img_folder != "":
+                    for image_file in os.listdir(f'{images_folder}/{volume_img_folder}'):
+                        _add_image(image_file)
 
     def _get_output_folder(self):
         if self.epub_settings['divide_volume']:
             out_folder = str(self._novel_book_title)
         else:
             out_folder = '.'
         return out_folder
```

## linovelib2epub/logger.py

```diff
@@ -8,14 +8,15 @@
 from time import localtime, strftime
 from typing import Optional
 
 from rich.logging import RichHandler
 
 DEFAULT_LOG_FOLDER = os.path.join(os.path.dirname(os.getcwd()), 'logs')
 
+
 class Logger:
     LEVEL_MAP = {
         'INFO': INFO,
         'DEBUG': DEBUG,
         'WARN': WARN,
         'WARNING': WARNING,
         'ERROR': ERROR,
@@ -76,73 +77,7 @@
 
         self.logger.handlers.clear()
         self.logger.addHandler(shell_handler)
         self.logger.addHandler(file_handler)
 
     def get_logger(self):
         return self.logger
-
-
-class MultiprocessingLogHelper:
-
-    def __init__(self, queue, log_name, log_file_path = None):
-        self.queue = queue
-        self.log_name = log_name
-        self.log_file_path = log_file_path or DEFAULT_LOG_FOLDER
-        self.logger = self.listener_configurer()
-
-    def listener_configurer(self):
-        """ Configures and returns a log file based on
-        the given name
-
-        Arguments:
-            log_name (str): String of the log name to use
-            log_file_path (str): String of the log file path
-
-        Returns:
-            logger: configured logging object
-        """
-        logger = logging.getLogger(self.log_name)
-
-        # fh = logging.FileHandler(
-        #     path.join(self.log_file_path, f'{self.log_name}.log'), encoding='utf-8')
-        # fmtr = logging.Formatter(
-        #     '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        # fh.setFormatter(fmtr)
-        logger.setLevel(logging.INFO)
-
-        # current_fh_names = [fh.__dict__.get(
-        #     'baseFilename', '') for fh in logger.handlers]
-        # if not fh.__dict__['baseFilename'] in current_fh_names:  # This prevents multiple logs to the same file
-        #     logger.addHandler(fh)
-
-        stream_hanlder = StreamHandler()
-        # logger.addHandler(fh)
-        logger.addHandler(stream_hanlder)
-
-        return logger
-
-    def listener_process(self):
-        """ Listener process is a target for a multiprocess process
-        that runs and listens to a queue for logging events.
-
-        Arguments:
-            queue (multiprocessing.manager.Queue): queue to monitor
-            configurer (func): configures loggers
-            log_name (str): name of the log to use
-
-        Returns:
-            None
-        """
-        self.listener_configurer()
-
-        while True:
-            try:
-                record = self.queue.get()
-                if record is None:
-                    break
-                print(f'record: {record}')
-                logger = logging.getLogger(record.name)
-                logger.handle(record)
-            except Exception:
-                print('Failure in listener_process', file=sys.stderr)
-                traceback.print_last(limit=1, file=sys.stderr)
```

## linovelib2epub/models.py

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, Set
 
 
 @dataclass
 class LightNovelChapter:
     cid: Union[int, str]
     title: str = ''
     content: str = ''
@@ -11,14 +11,23 @@
 
 @dataclass
 class LightNovelVolume:
     vid: Union[int, str]
     title: str = ''
     chapters: list = field(default_factory=list)
 
+    # The set "volume_img_folders" is used to extract images in specific volume when "divide_volume=True"
+    volume_img_folders: set = field(default_factory=set)
+    # volume_cover is used as the cover image in specific volume when "divide_volume=True"
+    volume_cover: str = ''
+
+    # example: https://img.linovelib.com/0/682/117077/50675.jpg
+    # volume_img_folder = {"117077","117900"} or {"117097"}
+    # volume_cover = "117077/50677.jpg"
+
     def add_chapter(self, cid: Union[int, str], title: str = '', content: str = ''):
         new_chapter = {
             'cid': cid,
             'title': title,
             'content': content
         }
         self.chapters.append(new_chapter)
@@ -68,19 +77,22 @@
     def get_illustration_set(self):
         image_set = set()
         for values in self.illustration_dict.values():
             for value in values:
                 image_set.add(value)
         return image_set
 
-    def add_volume(self, vid: Union[int, str], title: str = '', chapters: List = None):
+    def add_volume(self, vid: Union[int, str], title: str = '', chapters: List = None, volume_img_folders: Set = None,
+                   volume_cover: str = ''):
         new_volume = {
             'vid': vid,
             'title': title,
-            'chapters': chapters if chapters else []
+            'chapters': chapters if chapters else [],
+            'volume_img_folders': volume_img_folders if volume_img_folders else set(),
+            'volume_cover': volume_cover,
         }
         self.volumes.append(new_volume)
 
     def get_volume_by_vid(self, vid):
         for volume in self.volumes:
             if volume.vid == vid:
                 return volume
```

## linovelib2epub/spider/base_spider.py

```diff
@@ -52,20 +52,21 @@
         error_links = process_pool.map(self._download_image_legacy, urls)
 
         while sorted_error_links := list(filter(None, error_links)):
             self.logger.info('Some errors occurred when download images. Retry those links that failed to request.')
             self.logger.info(f'Retry image links: {sorted_error_links}')
             error_links = process_pool.map(self._download_image_legacy, sorted_error_links)
 
-        # downloading image: https://img.linovelib.com/0/682/117082/50748.jpg to [folder]/0-682-117082-50748.jpg
+        # downloading image: https://img.linovelib.com/0/682/117082/50748.jpg to [image_download_folder]/[117082]/50748.jpg
         # re-check image download result:
         # - happy result: urls_set - self.image_download_folder == 0
         # - ? result: urls_set - self.image_download_folder < 0 , maybe you put some other images in this folder.
         # - bad result: urls_set - self.image_download_folder > 0
-        download_image_miss_quota = len(urls) - len(os.listdir(self.spider_settings['image_download_folder']))
+
+        download_image_miss_quota = len(urls) - sum([len(files) for root, dirs, files in os.walk(self.spider_settings['image_download_folder'])])
         self.logger.info(f'download_image_miss_quota: {download_image_miss_quota}. Quota <=0 is ok.')
         if download_image_miss_quota <= 0:
             self.logger.info('The result of downloading pictures is perfect.')
         else:
             self.logger.warn('Some pictures to download are missing. Maybe this is a bug. You can Retry.')
 
     def _download_image_legacy(self, url: str) -> Optional[str]:
@@ -76,22 +77,24 @@
         :return: original url if failed, or None if succeeded.
         """
         if not is_valid_image_url(url):
             return
 
         filename = self.get_image_filename(url)
         save_path = f"{self.spider_settings['image_download_folder']}/{filename}"
+        if not os.path.exists(os.path.dirname(save_path)):
+            os.makedirs(os.path.dirname(save_path))
 
         filename_path = Path(save_path)
         if filename_path.exists():
             return
 
         # url is valid and never downloaded
         try:
-            resp = self.session.get(url, headers={}, timeout=self.spider_settings['http_timeout'])
+            resp = self.session.get(url, headers=self.request_headers(), timeout=self.spider_settings['http_timeout'])
 
             expected_length = resp.headers and resp.headers.get('Content-Length')
             actual_length = resp.raw.tell()
             check_image_integrity(expected_length, actual_length)
         except (Exception, ProxyError,) as e:
             # SAD PATH
             return url
@@ -144,22 +147,24 @@
 
     async def _download_image(self, session: ClientSession, url: str) -> None:
         if not is_valid_image_url(url):
             return
 
         filename = self.get_image_filename(url)
         save_path = f"{self.spider_settings['image_download_folder']}/{filename}"
+        if not os.path.exists(os.path.dirname(save_path)):
+            os.makedirs(os.path.dirname(save_path))
 
         filename_path = Path(save_path)
         if filename_path.exists():
             self.logger.info(f"The image to download is alreay downloaded at {filename_path}.skip.")
             return
 
         timeout = aiohttp.ClientTimeout(total=30, connect=15)  # per request timeout
-        async with session.get(url, timeout=timeout) as resp:
+        async with session.get(url, headers=self.request_headers(), timeout=timeout) as resp:
             if resp.status < 400:
                 image = await resp.read()
 
                 # check image integrity here, if get partial, MUST raise error
                 expected_get = resp.headers.get('Content-Length')
                 actual_get = len(image)
                 self.logger.debug(f'check_image_integrity: expected_get:{expected_get} vs actual_get: {actual_get}')
```

## linovelib2epub/spider/linovelib_mobile_spider.py

```diff
@@ -37,15 +37,18 @@
         start = time.perf_counter()
         novel_whole = self._fetch()
         self.logger.info('(Perf metrics) Fetch Book took: {} seconds'.format(time.perf_counter() - start))
 
         return novel_whole
 
     def get_image_filename(self, url):
-        return '-'.join(url.split("/")[-4:])
+        # example: https://img.linovelib.com/0/682/117077/50675.jpg => 117077/50677.jpg
+        # "117077" will be treated as a folder
+        # "50677.jpg" is the image filename
+        return '/'.join(url.split("/")[-2:])
 
     def _init_http_client(self):
         self.session = requests.Session()
 
         if self.spider_settings["disable_proxy"]:
             self.session.trust_env = False
 
@@ -78,14 +81,143 @@
 
             except (Exception,):
                 self.logger.error(f'Failed to parse basic info of book_id: {self.spider_settings["book_id"]}')
 
         return None
 
     def _crawl_book_content(self, catalog_url):
+        def _anti_js_obfuscation(html):
+            """
+            recover original text of the novel content.
+
+            :param html:
+            :return: html after anti-js obfuscation
+            """
+            mapping_dict = {
+                '“': "「",
+                '’': "』",
+                "": "是",
+                "": "不",
+                "": "他",
+                "": "个",
+                "": "来",
+                "": "大",
+                "": "子",
+                "": "说",
+                "": "年",
+                "": "那",
+                "": "她",
+                "": "得",
+                "": "自",
+                "": "家",
+                "": "而",
+                "": "去",
+                "": "小",
+                "": "于",
+                "": "么",
+                "": "好",
+                "": "发",
+                "": "成",
+                "": "事",
+                "": "用",
+                "": "道",
+                "": "种",
+                "": "乳",
+                "": "茎",
+                "": "肉",
+                "": "胸",
+                "": "淫",
+                "": "射",
+                "": "骚",
+                '”': "」",
+                "": "的",
+                "": "了",
+                "": "人",
+                "": "有",
+                "": "上",
+                "": "到",
+                "": "地",
+                "": "中",
+                "": "生",
+                "": "着",
+                "": "和",
+                "": "出",
+                "": "里",
+                "": "以",
+                "": "可",
+                "": "过",
+                "": "能",
+                "": "多",
+                "": "心",
+                "": "之",
+                "": "看",
+                "": "当",
+                "": "只",
+                "": "把",
+                "": "第",
+                "": "想",
+                "": "开",
+                "": "阴",
+                "": "欲",
+                "": "交",
+                "": "私",
+                "": "臀",
+                "": "脱",
+                "": "唇",
+                '‘': "『",
+                "": "一",
+                "": "我",
+                "": "在",
+                "": "这",
+                "": "们",
+                "": "时",
+                "": "为",
+                "": "你",
+                "": "国",
+                "": "就",
+                "": "要",
+                "": "也",
+                "": "后",
+                "": "会",
+                "": "下",
+                "": "天",
+                "": "对",
+                "": "然",
+                "": "学",
+                "": "都",
+                "": "起",
+                "": "没",
+                "": "如",
+                "": "还",
+                "": "样",
+                "": "作",
+                "": "美",
+                "": "液",
+                "": "呻",
+                "": "性",
+                "": "穴",
+                "": "舔",
+                "": "裸",
+            }
+
+            table = str.maketrans(mapping_dict)
+            res = html.translate(table)
+            return res
+
+        def _sanitize_html(html):
+            """
+            strip useless script on body tag by reg or soup library method.
+
+            e.g. <script>zation();</script>
+
+            :param html:
+            :return:
+            """
+            return re.sub(r'<script.+?</script>', '', html, flags=re.DOTALL)
+
         book_catalog_rs = None
         try:
             book_catalog_rs = request_with_retry(self.session,
                                                  catalog_url,
                                                  headers=self.request_headers(),
                                                  retry_max=self.spider_settings['http_retries'],
                                                  timeout=self.spider_settings["http_timeout"],
@@ -124,14 +256,15 @@
                 new_volume.title = volume['volume_title']
 
                 self.logger.info(f'volume: {volume["volume_title"]}')
 
                 illustration_dict.setdefault(volume['vid'], [])
 
                 chapter_id = -1
+                chapter_list = []  # store chapter for removing duplicate images in the first chapter
                 for chapter in volume['chapters']:
                     chapter_content = ''
                     chapter_title = chapter[0]
                     chapter_id += 1
 
                     new_chapter = LightNovelChapter(cid=chapter_id)
                     new_chapter.title = chapter_title
@@ -180,45 +313,108 @@
                         if page_resp:
                             soup = BeautifulSoup(page_resp.text, 'lxml')
                         else:
                             raise Exception(f'[ERROR]: request {page_link} failed.')
 
                         images = soup.find_all('img')
                         article = str(soup.find(id="acontent"))
-
                         for _, image in enumerate(images):
-                            # img tag format: <img src="https://img.linovelib.com/0/682/117078/50677.jpg" border="0" class="imagecontent">
-                            image_src = image['src']
-                            illustration_dict[volume['vid']].append(image_src)
-                            src_value = re.search(r"(?<=src=\").*?(?=\")", str(image))
 
-                            # example: https://img.linovelib.com/0/682/117077/50675.jpg => [folder]/0-682-117078-50677.jpg
-                            # here we convert its path `0/682/117078/50677.jpg` to `0-682-117078-50677.jpg` as filename.
-                            local_image_uri = self.get_image_filename(src_value.group())
+                            # images in the first chapter are lazyload, their urls are inside "data-src"
+                            # img tag format: <img class="imagecontent lazyload" data-src="https://img1.readpai.com/0/28/109869/146248.jpg" src="/images/photon.svg"/>
+                            image_src = image.get("data-src")
+                            if image_src:
+                                data_src_value = re.search('(?<= data-src=").*?(?=")', str(image))
+                                src_value = re.search('(?<= src=").*?(?=")', str(image))
+                                local_image_uri = self.get_image_filename(data_src_value.group())
+                            # <img border="0" class="imagecontent" src="https://img1.readpai.com/0/28/109869/146254.jpg"/>
+                            else:
+                                image_src = image.get("src")
+                                src_value = re.search('(?<= src=").*?(?=")', str(image))
+                                local_image_uri = self.get_image_filename(src_value.group())
+
+                            # local_image_uri is "[volume_img_folder]/[filename]"
+                            # example: https://img.linovelib.com/0/682/117077/50675.jpg => [image_download_folder]/117077/50677.jpg
+                            # 117077 is [volume_img_folder]
+                            # 50677.jpg is the [filename]
+
                             replace_value = f'{self.spider_settings["image_download_folder"]}/' + local_image_uri
+                            new_image = str(image).replace(str(src_value.group()), replace_value)
+
                             # replace all remote images src to local file path
-                            article = article.replace(str(src_value.group()), str(replace_value))
+                            article = article.replace(str(image), new_image)
+
+                            illustration_dict[volume['vid']].append(image_src)
 
-                        article = self._sanitize_html(article)
+                        article = _sanitize_html(article)
+                        article = _anti_js_obfuscation(article)
                         chapter_content += article
 
                         self.logger.info(f'Processing page... {page_link}')
 
                     # Here, current chapter's content has been solved
                     new_chapter.content = chapter_content
-                    new_volume.add_chapter(cid=new_chapter.cid,
-                                           title=new_chapter.title,
-                                           content=new_chapter.content)
-
-                new_novel.add_volume(vid=new_volume.vid,
-                                     title=new_volume.title,
-                                     chapters=new_volume.chapters)
+                    chapter_list.append(new_chapter)
 
-            new_novel.set_illustration_dict(illustration_dict)
+                # removing duplicate images in the first chapter
+                def _filter_duplicate_images(match, img_src_list):
+                    img = match.group()
+                    img_src = re.search('(?<= src=").*?(?=")', match.group()).group()
+                    if img_src in img_src_list:
+                        self.logger.info(f'Remove duplicate image in the first chapter... {img_src}')
+                        return ""
+
+                    else:
+                        return img
+
+                img_src_list = []
+                for chapter in chapter_list[1:]:
+                    img_src_list.extend(
+                        [re.search('(?<= src=").*?(?=")', i).group() for i in re.findall('<img.*?/>', chapter.content)]
+                    )
+                chapter_list[0].content = re.sub('<img.*?/>',
+                                                 lambda match: _filter_duplicate_images(match, img_src_list),
+                                                 chapter_list[0].content)
+
+                for chapter in chapter_list:
+                    new_volume.add_chapter(
+                        cid=chapter.cid,
+                        title=chapter.title,
+                        content=chapter.content
+                    )
+
+                def _resolve_img_folders(img_list) -> set:
+                    unique_folders = set()
+                    for idx, image in enumerate(img_list):
+                        path = self.get_image_filename(image)
+                        folder, _ = path.split("/")
+                        unique_folders.add(folder)
+                    return unique_folders
+
+                # store [volume_img_folders] and [volume_cover] in volume dict
+                if illustration_dict[volume['vid']]:
+                    volume_images = illustration_dict[volume['vid']]
+
+                    cover_image_url = volume_images[0]
+                    path = self.get_image_filename(cover_image_url)
+                    new_volume.volume_cover = path
+
+                    # BUG case: https://w.linovelib.com/novel/3728/catalog 后记章节，图片缺失
+                    # 这里代码有问题，一卷也可以存在多个volume_id，folder应该定义为list
+                    new_volume.volume_img_folders = _resolve_img_folders(volume_images)
+
+                new_novel.add_volume(
+                    vid=new_volume.vid,
+                    title=new_volume.title,
+                    chapters=new_volume.chapters,
+                    volume_img_folders=new_volume.volume_img_folders,
+                    volume_cover=new_volume.volume_cover
+                )
 
+            new_novel.set_illustration_dict(illustration_dict)
             return new_novel
 
         else:
             self.logger.error(f'Failed to get the catalog of book_id: {self.spider_settings["book_id"]}')
 
         return None
 
@@ -249,26 +445,14 @@
         ]
         # user input
         # answers: {'Selecting volumes': [3, 6]}
         answers = inquirer.prompt(questions)
         catalog_list = _reduce_catalog_by_selection(catalog_list, answers[question_name])
         return catalog_list
 
-    @staticmethod
-    def _sanitize_html(html):
-        """
-        strip useless script on body tag by reg or soup method.
-
-        e.g. <script>zation();</script>
-
-        :param html:
-        :return:
-        """
-        return re.sub(r'<script.+?</script>', '', html, flags=re.DOTALL)
-
     def _convert_to_catalog_list(self, catalog_html_lis):
         # return example:
         # [{vid:1,volume_title: "XX", chapters:[[xxx,u1,u2,u3],[xx,u1,u2],[...] ]},{},{}]
 
         catalog_list = []
         current_volume = []
         current_volume_text = catalog_html_lis[0].text
@@ -338,8 +522,8 @@
         novel_whole.book_title = book_title
         novel_whole.author = author
         novel_whole.description = book_summary
         novel_whole.book_cover = book_cover
         novel_whole.book_cover_local = self.get_image_filename(book_cover)
         novel_whole.mark_basic_info_ready()
 
-        return novel_whole
+        return novel_whole
```

## Comparing `linovelib2epub-0.1.1.dist-info/METADATA` & `linovelib2epub-0.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linovelib2epub
-Version: 0.1.1
+Version: 0.1.2
 Summary: Craw light novel from [哔哩轻小说(linovelib)](https://w.linovelib.com/) and convert to epub.
 Project-URL: Homepage, https://github.com/wdpm/linovelib2epub
 Project-URL: Source, https://github.com/wdpm/linovelib2epub
 Project-URL: Tracker, https://github.com/wdpm/linovelib2epub/issues
 Author-email: wdpm <1137299673@qq.com>
 License-File: LICENSE
 Keywords: ebook,epub,library,light novel,哔哩轻小说
@@ -165,25 +165,27 @@
 ## Todo
 
 - [ ] quality: setup pytest and codecov
 - [ ] quality: setup more formatter and linter for maintainability
 
 ## Contributors
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GOUKOU007"><img src="https://avatars.githubusercontent.com/u/40916324?v=4?s=100" width="100px;" alt="GokouRuri"/><br /><sub><b>GokouRuri</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/issues?q=author%3AGOUKOU007" title="Bug reports">🐛</a> <a href="https://github.com/lightnovel-center/linovelib2epub/commits?author=GOUKOU007" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/xxxfhy"><img src="https://avatars.githubusercontent.com/u/40598925?v=4?s=100" width="100px;" alt="xxxfhy"/><br /><sub><b>xxxfhy</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/issues?q=author%3Axxxfhy" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GOUKOU007"><img src="https://avatars.githubusercontent.com/u/40916324?v=4?s=60" width="60px;" alt="GokouRuri"/><br /><sub><b>GokouRuri</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/issues?q=author%3AGOUKOU007" title="Bug reports">🐛</a> <a href="https://github.com/lightnovel-center/linovelib2epub/commits?author=GOUKOU007" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/xxxfhy"><img src="https://avatars.githubusercontent.com/u/40598925?v=4?s=60" width="60px;" alt="xxxfhy"/><br /><sub><b>xxxfhy</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/issues?q=author%3Axxxfhy" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://foxlesbiao.github.io/"><img src="https://avatars.githubusercontent.com/u/41581909?v=4?s=60" width="60px;" alt="lesfox"/><br /><sub><b>lesfox</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/issues?q=author%3Afoxlesbiao" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://dongliteahouse.wordpress.com"><img src="https://avatars.githubusercontent.com/u/56831381?v=4?s=60" width="60px;" alt="Holence"/><br /><sub><b>Holence</b></sub></a><br /><a href="https://github.com/lightnovel-center/linovelib2epub/commits?author=Holence" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

## Comparing `linovelib2epub-0.1.1.dist-info/licenses/LICENSE` & `linovelib2epub-0.1.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `linovelib2epub-0.1.1.dist-info/RECORD` & `linovelib2epub-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-linovelib2epub/__about__.py,sha256=zGU39ZwaRkNKxWLnAB7Zte9ZtfyfMEsBJp-bHUfQTyA,23
+linovelib2epub/__about__.py,sha256=TWY2HHBr7soKzDojVTmRRRQj8LWtiK2CcaOJolf0kU0,23
 linovelib2epub/__init__.py,sha256=8CCbmojIlWmlU7B-linDBDGXcs3FOCtsl4-Ojqvu0yU,62
 linovelib2epub/exceptions.py,sha256=lFhHpmN0tJFrNGLg4Le5TxrNzuRxsQN8atGnsJ8FMdg,120
-linovelib2epub/linovel.py,sha256=hkfH7QxcEWUmTNFJ-JSVbp51F65nA78iVFoYcLJoB9w,15260
-linovelib2epub/logger.py,sha256=snGJwPB5wyd2YZeyAB1-urUHU6mE4ZbKTVE9PjFaY90,5086
-linovelib2epub/models.py,sha256=dqdoOUA8oalb2RGU489alxDTYmyGETOciKwIFi7eOtE,2680
+linovelib2epub/linovel.py,sha256=Vynuc0MGUpFsTRvQHXD-OO4iIFLddfTIeDySId4sjjY,17331
+linovelib2epub/logger.py,sha256=jJ9XRppJw_XnK7miTacLe51zdxQU4g6Ad8EyhH_GYo0,2799
+linovelib2epub/models.py,sha256=roTMd2xK7edAtYhoXMZfLhHOh1SFKyiebgmyrHyc3so,3349
 linovelib2epub/settings.py,sha256=joZ6dJ0SAY_tKlnYAnrtmbs0EJCUH_x7QEt4XxGw3ts,1246
 linovelib2epub/utils.py,sha256=dD50_YpNMXg3kCyrf8UQXl4wAdO1-Y_55q9K1AcBun0,3522
 linovelib2epub/spider/__init__.py,sha256=LAW6YwlEprVWfQ60XiQGdt38MacuKRlkbfeY-kYp57I,331
-linovelib2epub/spider/base_spider.py,sha256=lwHIzUlylH_9o_sFP-1z_qvnB7geuAHXp8UiPykA2zM,8818
-linovelib2epub/spider/linovelib_mobile_spider.py,sha256=FHQwK_7mbQjgneZgRVao6oiprY2WY8whV0xp-QmVyFs,16015
+linovelib2epub/spider/base_spider.py,sha256=pUrDsTJFRKLcVKdILBHufppTYsWGLl50N5D_rBcLolA,9144
+linovelib2epub/spider/linovelib_mobile_spider.py,sha256=r4UuRkRCzXwo1ACBZI-JW_o7os5mDXrIL4YiZ1sFTUI,23200
 linovelib2epub/styles/chapter.css,sha256=Y9B1m4Az_POEmBCmTi7-VRZtZ2rKtAJiUXQgXfkhD6I,812
 linovelib2epub/styles/cover.css,sha256=XNLJieS0z6pM-N7JmzlIbPB8zHDJTlYzj8up5gRSlng,295
 linovelib2epub/styles/nav.css,sha256=lYOD7xRWIQeTFPxZb3DusjhhssYGIBICjokDjiQW-lo,368
-linovelib2epub-0.1.1.dist-info/METADATA,sha256=pYsEOXZdmuinlZIMMpCi5Xu379TlP4ZqtW5vDLYUS5s,10452
-linovelib2epub-0.1.1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-linovelib2epub-0.1.1.dist-info/licenses/LICENSE,sha256=kn2aD5kGS5Dv7OCGNVznr_sf1puJqE85rLQaqVwZFG8,35176
-linovelib2epub-0.1.1.dist-info/RECORD,,
+linovelib2epub-0.1.2.dist-info/METADATA,sha256=mhRIa0xRPKMSwwM4BAxmifTFmMZ_GRYtMKGDahl9d8s,11153
+linovelib2epub-0.1.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+linovelib2epub-0.1.2.dist-info/licenses/LICENSE,sha256=kn2aD5kGS5Dv7OCGNVznr_sf1puJqE85rLQaqVwZFG8,35176
+linovelib2epub-0.1.2.dist-info/RECORD,,
```

