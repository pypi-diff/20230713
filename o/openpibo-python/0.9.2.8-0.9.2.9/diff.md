# Comparing `tmp/openpibo_python-0.9.2.8-py3-none-any.whl.zip` & `tmp/openpibo_python-0.9.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 65538 bytes, number of entries: 30
--rw-r--r--  2.0 unx      796 b- defN 21-Oct-18 06:49 openpibo/__init__.py
+Zip file size: 64337 bytes, number of entries: 30
+-rw-r--r--  2.0 unx      796 b- defN 21-Oct-18 09:32 openpibo/__init__.py
 -rw-r--r--  2.0 unx     3521 b- defN 21-Oct-18 06:42 openpibo/audio.py
 -rw-r--r--  2.0 unx     9850 b- defN 21-Oct-18 06:42 openpibo/collect.py
 -rw-r--r--  2.0 unx    10976 b- defN 21-Oct-18 06:42 openpibo/device.py
--rw-r--r--  2.0 unx    51708 b- defN 21-Oct-18 06:42 openpibo/edu_v1.py
+-rw-r--r--  2.0 unx    46950 b- defN 21-Oct-18 09:31 openpibo/edu_v1.py
 -rw-r--r--  2.0 unx    17342 b- defN 21-Oct-18 06:42 openpibo/motion.py
 -rw-r--r--  2.0 unx     7316 b- defN 21-Oct-18 06:42 openpibo/oled.py
 -rw-r--r--  2.0 unx     8944 b- defN 21-Oct-18 06:42 openpibo/speech.py
 -rw-r--r--  2.0 unx    24149 b- defN 21-Oct-18 06:42 openpibo/vision.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 06:42 openpibo/modules/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 06:42 openpibo/modules/oled/__init__.py
 -rw-r--r--  2.0 unx     4216 b- defN 21-Oct-18 06:42 openpibo/modules/oled/board.py
@@ -21,12 +21,12 @@
 -rw-r--r--  2.0 unx     8364 b- defN 21-Oct-18 06:42 openpibo/modules/oled/ssd1306.py
 -rw-r--r--  2.0 unx     2142 b- defN 21-Oct-18 06:42 openpibo/modules/oled/util.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 06:42 openpibo/modules/speech/__init__.py
 -rw-r--r--  2.0 unx     8770 b- defN 21-Oct-18 06:42 openpibo/modules/speech/constant.py
 -rw-r--r--  2.0 unx    10999 b- defN 21-Oct-18 06:42 openpibo/modules/speech/google_trans_new.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-18 06:42 openpibo/modules/vision/__init__.py
 -rw-r--r--  2.0 unx     1047 b- defN 21-Oct-18 06:42 openpibo/modules/vision/stream.py
--rw-r--r--  2.0 unx     1451 b- defN 21-Oct-18 06:49 openpibo_python-0.9.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-18 06:49 openpibo_python-0.9.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Oct-18 06:49 openpibo_python-0.9.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2529 b- defN 21-Oct-18 06:49 openpibo_python-0.9.2.8.dist-info/RECORD
-30 files, 214883 bytes uncompressed, 61466 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     1409 b- defN 21-Oct-18 09:33 openpibo_python-0.9.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Oct-18 09:33 openpibo_python-0.9.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 21-Oct-18 09:33 openpibo_python-0.9.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2529 b- defN 21-Oct-18 09:33 openpibo_python-0.9.2.9.dist-info/RECORD
+30 files, 210083 bytes uncompressed, 60265 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: openpibo/modules/vision/__init__.py
 Comment: 
 
 Filename: openpibo/modules/vision/stream.py
 Comment: 
 
-Filename: openpibo_python-0.9.2.8.dist-info/METADATA
+Filename: openpibo_python-0.9.2.9.dist-info/METADATA
 Comment: 
 
-Filename: openpibo_python-0.9.2.8.dist-info/WHEEL
+Filename: openpibo_python-0.9.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: openpibo_python-0.9.2.8.dist-info/top_level.txt
+Filename: openpibo_python-0.9.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: openpibo_python-0.9.2.8.dist-info/RECORD
+Filename: openpibo_python-0.9.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openpibo/__init__.py

```diff
@@ -1,13 +1,13 @@
 """
 openpibo-python
 """
 import os, sys, json, shutil
 
-__version__ = '0.9.2.8'
+__version__ = '0.9.2.9'
 
 if os.path.isfile('/home/pi/config.json') == False:
   config = {"DATA_PATH":"/home/pi/openpibo-files", "KAKAO_ACCOUNT":"", "robotId":""}
   with open('/home/pi/config.json', 'w') as f:
     json.dump(config, f)
 else:
   with open('/home/pi/config.json', 'r') as f:
```

## openpibo/edu_v1.py

```diff
@@ -24,30 +24,27 @@
 from .oled import Oled
 from .speech import Speech, Dialog
 from .device import Device
 from .motion import Motion
 from .vision import Camera, Face, Detect
 from .modules.vision.stream import VideoStream
 
-from threading import Thread, Lock
+from threading import Thread
 from queue import Queue
 
 """
 Class:
 :obj:`~openpibo.edu_v1.Pibo`
 """
 
 class Pibo:
   """
 Functions:
 :meth:`~openpibo.edu_v1.Pibo.play_audio`
 :meth:`~openpibo.edu_v1.Pibo.stop_audio`
-:meth:`~openpibo.edu_v1.Pibo.search_wikipedia`
-:meth:`~openpibo.edu_v1.Pibo.search_weather`
-:meth:`~openpibo.edu_v1.Pibo.search_news`
 :meth:`~openpibo.edu_v1.Pibo.eye_on`
 :meth:`~openpibo.edu_v1.Pibo.eye_off`
 :meth:`~openpibo.edu_v1.Pibo.check_device`
 :meth:`~openpibo.edu_v1.Pibo.thread_device`
 :meth:`~openpibo.edu_v1.Pibo.start_thread_device`
 :meth:`~openpibo.edu_v1.Pibo.stop_thread_device`
 :meth:`~openpibo.edu_v1.Pibo.motor`
@@ -86,17 +83,14 @@
 
   ``openpibo`` 의 다양한 기능들을 한번에 사용할 수 있는 클래스 입니다.
 
   다음 클래스의 기능을 모두 사용할 수 있습니다.
 
   * Device
   * Audio
-  * Wikipedia
-  * Weather
-  * News
   * Oled
   * Speech
   * Dialog
   * Motion
   * Camera
   * Face
   * Detect
@@ -122,17 +116,14 @@
   def __init__(self):
     self.camera_loop = False
     self.img = None
     self.device_loop = False
     self.flash = False
     self.device = Device()
     self.audio = Audio()
-    self.wikipedia = Wikipedia()
-    self.weather = Weather()
-    self.news = News()
     self.oled = Oled()
     self.speech = Speech()
     self.dialog = Dialog()
     self.motion = Motion()
     self.camera = Camera()
     self.face = Face()
     self.detect = Detect()
@@ -209,149 +200,14 @@
     try:
       self.audio.stop()
       return self.return_msg(True, "Success", "Success", None)
     except Exception as e:
       return self.return_msg(False, "Exception error", e, None)
 
 
-  # [Collect] - Wikipedia
-  def search_wikipedia(self, topic=None):
-    """
-    위키백과에서 ``topic`` 를 검색합니다.
-
-    example::
-
-      pibo_edu_v1.search_wikipedia('강아지')
-
-    :returns:
-
-      * 성공: ``{"result": True, "errcode": 0, "errmsg": "Success", "data": list 형태의 data}``
-      * 실패: ``{"result": False, "errcode": errcode, "errmsg": "errmsg", "data": None}``
-
-        대부분의 경우 '0'번 항목에 개요를 표시하고, 검색된 내용이 없을 경우 None을 반환합니다.
-
-          example::
-
-            ['0':{
-              'title': '명칭', 
-               'content': "한국어 ‘강아지’는 ‘개’에 어린 짐승을 뜻하는 ‘아지’가 붙은 말이다..."
-            }, ... ]
-            or
-            None
-    """
-
-    try:
-      if topic == None:
-        return self.return_msg(False, "Argument error", "topic is required", None)
-      result = self.wikipedia.search(topic)
-      return self.return_msg(True, "Success", "Success", result)
-    except Exception as e:
-      return self.return_msg(False, "Exception error", e, None)
-
-
-  # [Collect] - Weather
-  def search_weather(self, region=None):
-    """
-    해당 지역(```region```)의 날씨 정보(종합예보, 오늘/내일/모레 날씨)를 가져옵니다.
-
-    example::
-
-      pibo_edu_v1.search_weather('전국')
-
-    :param str search_region: 검색 가능한 지역 (default: 전국)
-
-      검색할 수 있는 지역은 다음과 같습니다::
-
-        '전국', '서울', '인천', '경기', '부산', '울산', '경남', '대구', '경북',
-        '광주', '전남', '전북', '대전', '세종', '충남', '충북', '강원', '제주'
-
-    :returns:
-
-      * 성공: ``{"result": True, "errcode": 0, "errmsg": "Success", "data": dict 형태의 data}``
-      * 실패: ``{"result": False, "errcode": errcode, "errmsg": "errmsg", "data": None}``
-
-      example::
-
-        종합예보와 오늘/내일/모레의 날씨 및 최저/최고기온을 반환합니다.
-        {
-          'forecast': '내일 경기남부 가끔 비, 내일까지 바람 약간 강, 낮과 밤의 기온차 큼'
-          'today':
-          {
-            'weather': '전국 대체로 흐림',
-            'minimum_temp': '15.3 ~ 21.6',
-            'highst_temp': '23.1 ~ 27.6'
-          }
-          'tomorrow':
-          {
-            'weather': '전국 대체로 흐림',
-            'minimum_temp': '15.3 ~ 21.6', 
-            'highst_temp': '23.1 ~ 27.6'
-          }
-          'after_tomorrow':
-          {
-            'weather': '전국 대체로 흐림',
-            'minimum_temp': '15.3 ~ 21.6',
-            'highst_temp': '23.1 ~ 27.6'
-          }
-        }
-        or None
-    """
-
-    try:
-      if region == None:
-        return self.return_msg(False, "Argument error", "region is required", None)
-      result = self.weather.search(region)
-      return self.return_msg(True, "Success", "Success", result)
-    except Exception as e:
-      return self.return_msg(False, "Exception error", e, None)
-
-
-  # [Collect] - News
-  def search_news(self, topic=None):
-    """
-    해당 주제(```topic```)에 맞는 뉴스를 가져옵니다.
-
-    example::
-
-      pibo_edu_v1.search_weather('전국')
-
-    :param str topic: 검색 가능한 뉴스 주제 (default: 뉴스랭킹)
-
-      검색할 수 있는 주제는 다음과 같습니다::
-
-        '속보', '정치', '경제', '사회', '국제', '문화', '연예', '스포츠',
-        '풀영상', '뉴스랭킹', '뉴스룸', '아침&', '썰전 라이브', '정치부회의'
-
-    :returns:
-
-      * 성공: ``{"result": True, "errcode": 0, "errmsg": "Success", "data": list 형태의 data}``
-      * 실패: ``{"result": False, "errcode": errcode, "errmsg": "errmsg", "data": None}``
-
-      example::
-
-        [
-          {
-            'title': '또 소방차 막은 불법주차, 이번엔 가차없이 밀어버렸다', 
-            'link': 'https://news.jtbc.joins.com/article/article.aspx?...',
-            'description': '2019년 4월 소방당국의 불법주정차 강경대응 훈련 모습...,
-            'pubDate': '2021.09.03'
-          },  
-        ]
-        or None
-    """
-
-    try:
-      if topic == None:
-        return self.return_msg(False, "Argument error", "topic is required", None)
-      result = self.news.search(topic)
-      return self.return_msg(True, "Success", "Success", result)
-    except Exception as e:
-      return self.return_msg(False, "Exception error", e, None)
-
-
   # [Neopixel] - LED ON
   def eye_on(self, *color):
     """
     LED를 켭니다.
 
     example::
```

## Comparing `openpibo_python-0.9.2.8.dist-info/METADATA` & `openpibo_python-0.9.2.9.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: openpibo-python
-Version: 0.9.2.8
+Version: 0.9.2.9
 Summary: openpibo-python package.
 Home-page: https://github.com/themakerrobot/openpibo-python
 Author: circulus
 Author-email: leeyunjai@circul.us
 License: UNKNOWN
 Keywords: openpibo
 Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: RPi.gpio (==0.7.0)
 Requires-Dist: beautifulsoup4 (==4.6.0)
-Requires-Dist: dlib (==19.19.0)
+Requires-Dist: dlib (>=19.19.0)
 Requires-Dist: flask-socketio (==5.1.1)
 Requires-Dist: flask (==2.0.1)
 Requires-Dist: future (==0.18.2)
 Requires-Dist: konlpy (==0.5.2)
-Requires-Dist: opencv-contrib-python (==4.1.0.25)
-Requires-Dist: opencv-python (==4.1.0.25)
+Requires-Dist: opencv-contrib-python (>=4.1.0.25)
 Requires-Dist: openpibo-detect-models (>=0.3.1)
 Requires-Dist: openpibo-dlib-models (>=0.3.1)
 Requires-Dist: openpibo-face-models (>=0.3.1)
 Requires-Dist: openpibo-models (>=0.3.1)
 Requires-Dist: pillow (==7.2.0)
 Requires-Dist: pyserial (==3.5)
 Requires-Dist: pytesseract (==0.3.4)
```

## Comparing `openpibo_python-0.9.2.8.dist-info/RECORD` & `openpibo_python-0.9.2.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-openpibo/__init__.py,sha256=d9z9oxHsId4y5jUqdCGLfoy6sdkb8D1TOLiRqp_4U0k,796
+openpibo/__init__.py,sha256=-7rguXlflEjS-aQuz9qHbBXuUTcS8XW0z21pHHfF9JE,796
 openpibo/audio.py,sha256=FDiqy7uOmtZpgFIUUpeGbGw9jyLzPd9R3ybTTBQBCIE,3521
 openpibo/collect.py,sha256=v6uSR8Qi-QZfFTkIvP9lAhJYSDwtCfXGOoGrUW85-G0,9850
 openpibo/device.py,sha256=Ydn-OyAs54P_Szzwmp9j4kiFmIeuV-dpTb2LcfaVLHU,10976
-openpibo/edu_v1.py,sha256=VlMCuI2-sWqwoDM7_sf6y2JXC0lf2Y1lhLTSQOxNiAY,51708
+openpibo/edu_v1.py,sha256=fnKsBK2_rqOKYcnaoTTzGl9U7pRAv_jvwainejUWO1k,46950
 openpibo/motion.py,sha256=IemUpF9j1gcCWhlYh21NTSo0F8Ii_S8nrxrx-0xgY5E,17342
 openpibo/oled.py,sha256=6LOP6y-yP0OVSa-TIaEqqD2hA0sgWg_24-bZc4eIKMg,7316
 openpibo/speech.py,sha256=QmIm7HJ3sKoVrcYLpYLkc_QPLvWEGKnzGrzsNbs901A,8944
 openpibo/vision.py,sha256=SVbKVX-nKAkf-TaZXnlZfoI6YMGp20VbdLgW2iJNRdk,24149
 openpibo/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openpibo/modules/oled/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openpibo/modules/oled/board.py,sha256=6NvmWelw6w52ljOr8m_JjxYElF-BvPwHI30PrBhbO60,4216
@@ -20,11 +20,11 @@
 openpibo/modules/oled/ssd1306.py,sha256=PkCLVEKJ4JFPmPBUPq-i_PACUGaPBjFQDbiviHQrhlQ,8364
 openpibo/modules/oled/util.py,sha256=uWG7qEz-BrANnXifYYir-XA5hfa2SsJ-wR4fJrT_-zU,2142
 openpibo/modules/speech/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openpibo/modules/speech/constant.py,sha256=tEGEMUL9h7oLtANlICownKq_50aXKA9XCNxE7eQKyjs,8770
 openpibo/modules/speech/google_trans_new.py,sha256=qdbzfwCDg8rNux7UQ6xgQi2q7FHQQZpBZLJAU3DjB50,10999
 openpibo/modules/vision/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openpibo/modules/vision/stream.py,sha256=RgW_944_bLWmTYQ5kJxcGmp2eQBG9FqHPn_IlN_Et3w,1047
-openpibo_python-0.9.2.8.dist-info/METADATA,sha256=5VqSLWto9PMcQ-aybFZ3T8NbVsROACkpqAFmOrnqjIw,1451
-openpibo_python-0.9.2.8.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
-openpibo_python-0.9.2.8.dist-info/top_level.txt,sha256=Enmq-yYyH9sryPFacbOC4LfAPAtS7NgjPj4m6-EWP7I,9
-openpibo_python-0.9.2.8.dist-info/RECORD,,
+openpibo_python-0.9.2.9.dist-info/METADATA,sha256=Sc_Ygx1UGYiJaQjJfiuJIfsqxVEWm3pXrENQ77t53h8,1409
+openpibo_python-0.9.2.9.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
+openpibo_python-0.9.2.9.dist-info/top_level.txt,sha256=Enmq-yYyH9sryPFacbOC4LfAPAtS7NgjPj4m6-EWP7I,9
+openpibo_python-0.9.2.9.dist-info/RECORD,,
```

