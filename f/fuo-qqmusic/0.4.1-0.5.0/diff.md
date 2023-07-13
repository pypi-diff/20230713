# Comparing `tmp/fuo_qqmusic-0.4.1.tar.gz` & `tmp/fuo_qqmusic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuo_qqmusic-0.4.1.tar", last modified: Sun Mar 20 16:55:03 2022, max compression
+gzip compressed data, was "fuo_qqmusic-0.5.0.tar", last modified: Thu Jul 13 17:34:43 2023, max compression
```

## Comparing `fuo_qqmusic-0.4.1.tar` & `fuo_qqmusic-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/
--rw-r--r--   0 runner    (1001) docker     (121)     8317 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/excs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11854 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    24355 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/page_explore.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/page_daily_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/fuo_qqmusic/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-20 16:55:02.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-03-20 16:55:02.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-03-20 16:55:03.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-03-20 16:55:02.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-03-20 16:55:02.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-20 16:55:02.000000 fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-03-20 16:55:01.000000 fuo_qqmusic-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:43.574740 fuo_qqmusic-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-13 17:34:43.574740 fuo_qqmusic-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:43.570739 fuo_qqmusic-0.5.0/fuo_qqmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:43.574740 fuo_qqmusic-0.5.0/fuo_qqmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/page_daily_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/page_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/fuo_qqmusic/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:43.574740 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:34:43.000000 fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:34:43.574740 fuo_qqmusic-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-13 17:34:42.000000 fuo_qqmusic-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/schemas.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/assets/icon.svg` & `fuo_qqmusic-0.5.0/fuo_qqmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/models.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/models.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/api.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import time
 
 import requests
 from .excs import QQIOError
 
 logger = logging.getLogger(__name__)
 
-api_base_url = 'http://c.y.qq.com'
-
 
 def djb2(string):
     ''' Hash a word using the djb2 algorithm with the specified base. '''
     h = 5381
     for c in string:
         h = ((h << 5) + h + ord(c)) & 0xffffffff
     return str(2147483647 & h)
@@ -118,60 +116,42 @@
 
         :param type_: 专辑： 2，歌手：1
         """
         return 'http://y.gtimg.cn/music/photo_new/T00{}R800x800M000{}.jpg' \
             .format(type_, mid)
 
     def search(self, keyword, type_=0, limit=20, page=1):
+        # Other supported types: songlist, user, mv, qc, gedantip, zhida.
         if type_ == 0:
             key_ = 'song'
         elif type_ == 8:
             key_ = 'album'
         elif type_ == 9:
             key_ = 'singer'
         else:
-            raise ValueError('invalid type_:%d', type_)
-
-        path = '/soso/fcgi-bin/client_search_cp'
-        url = api_base_url + path
-        params = {
-            # w,n,page are required parameters
-            'w': keyword,
-            't': type_,  # t=0 代表歌曲，专辑:8, 歌手:9, 歌词:7, mv:12
-            'n': limit,
-            'page': page,
-
-            # positional parameters
-            'cr': 1,  # copyright?
-            #
-            'new_json': 1,
-            'format': 'json',
-            'platform': 'yqq.json'
+            raise QQIOError('invalid search type_:%d', type_)
+        payload = {
+            "search": {
+                "method": "DoSearchForQQMusicDesktop",
+                "module": "music.search.SearchCgiService",
+                "param": {
+                    # People said that the max num_per_page is 30.
+                    "num_per_page": max(limit, 30),
+                    "page_num": page,
+                    "search_type": type_,
+                    "query": keyword,
+                }
+            }
         }
-        resp = requests.get(url, params=params, timeout=self._timeout)
-        rv = resp.json()
-        return rv['data'][key_]['list']
+        js = self.rpc(payload)
+        result = js['search']['data']['body'][key_]['list']
+        return result
 
     def search_playlists(self, query, limit=20, page=1):
-        path = '/soso/fcgi-bin/client_music_search_songlist'
-        url = api_base_url + path
-        params = {
-            'query': query,
-            'page_no': page - 1,
-            'num_per_page': limit,
-            'format': 'json',
-            'remoteplace': 'txt.yqq.top',
-            'searchid': 1,
-            'flag_qc': 0,
-        }
-
-        resp = requests.get(url, params=params, headers=self._headers,
-                            timeout=self._timeout)
-        rv = resp.json()
-        return rv['data']['list']
+        raise QQIOError('search api is not available')
 
     def song_detail(self, song_id):
         uin = self._uin
         song_id = int(song_id)
         # 往 payload 添加字段，有可能还可以获取相似歌曲、歌单等
         payload = {
             'comm': {
@@ -207,16 +187,15 @@
             }
         }
         js = self.rpc(payload)
         data_songs = js['simsongs']['data']['songInfoList']
         return data_songs
 
     def artist_detail(self, artist_mid):
-        url = 'https://u.y.qq.com/cgi-bin/musics.fcg'
-        data = {
+        payload = {
             'req_0': {
                 'module': 'music.musichallSinger.SingerInfoInter',
                 'method': 'GetSingerDetail',
                 'param': {
                     'singer_mids': [artist_mid],
                     'pic': 1,
                     'group_singer': 1,
@@ -225,38 +204,26 @@
                 }},
             'comm': {
                 'g_tk': self.get_token_from_cookies(),
                 'uin': self._uin,
                 'format': 'json',
             }
         }
-        data_str = json.dumps(data)
-
-        params = {
-            '_': int(round(time.time() * 1000)),
-            'sign': _get_sign(data_str),
-            'data': data_str
-        }
-
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
-
+        js = self.rpc(payload)
         data = js['req_0']['data']['singer_list'][0]
         data = {
             'singer_id': data['basic_info']['singer_id'],
             'singer_mid': data['basic_info']['singer_mid'],
             'singer_name': data['basic_info']['name'],
             'SingerDesc': data['ex_info']['desc'],
         }
         return data
 
     def artist_songs(self, artist_id, page=1, page_size=50):
-        url = 'https://u.y.qq.com/cgi-bin/musics.fcg'
-        data = {
+        payload = {
             'req_0': {
                 'module': 'music.musichallSong.SongListInter',
                 'method': 'GetSingerSongList',
                 'param': {
                     'singerid': artist_id,
                     'begin': (page - 1) * page_size,
                     'num': page_size,
@@ -265,153 +232,54 @@
                 }},
             'comm': {
                 'g_tk': self.get_token_from_cookies(),
                 'uin': self._uin,
                 'format': 'json',
             }
         }
-        data_str = json.dumps(data)
-
-        params = {
-            '_': int(round(time.time() * 1000)),
-            'sign': _get_sign(data_str),
-            'data': data_str
-        }
-
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
+        js = self.rpc(payload)
         return js['req_0']['data']
 
     def artist_albums(self, artist_id, page=1, page_size=20):
-        url = api_base_url + '/v8/fcg-bin/fcg_v8_singer_album.fcg'
-        params = {
-            'singerid': artist_id,
-            'order': 'time',
-            'begin': (page - 1) * page_size,  # TODO: 这里应该代表偏移量
-            'num': page_size
-        }
-        response = requests.get(url, params=params)
-        js = response.json()
-        return js['data']
+        raise QQIOError('artist_albums api is not available')
 
     def album_detail(self, album_id):
-        url = api_base_url + '/v8/fcg-bin/fcg_v8_album_detail_cp.fcg'
-        params = {
-            'albumid': album_id,
-            'format': 'json',
-            'newsong': 1
-        }
-        resp = requests.get(url, params=params)
-        return resp.json()['data']
+        raise QQIOError('album_detail api is not available')
 
     def playlist_detail(self, pid, offset=0, limit=50):
-        url = api_base_url + '/qzone/fcg-bin/fcg_ucc_getcdinfo_byids_cp.fcg'
-        params = {
-            'type': '1',
-            'utf8': '1',
-            'disstid': pid,
-            'format': 'json',
-            'new_format': '1',  # 需要这个字段来获取file等信息
-            'song_begin': offset,
-            'song_num': limit,
-        }
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
-        if js['code'] != 0:
-            raise CodeShouldBe0(js)
-        return js['cdlist'][0]
+        raise QQIOError('playlist_detail api is not available')
 
     def user_detail(self, uid):
-        """
-        this API can be called only when user has logged in
-        """
-        url = api_base_url + '/rsc/fcgi-bin/fcg_get_profile_homepage.fcg'
-        params = {
-            # 这两个字段意义不明，不过至少固定为此值时可正常使用
-            'cid': 205360838,
-            'reqfrom': 1,
-            'userid': uid
-        }
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
-        if js['code'] != 0:
-            raise CodeShouldBe0(js)
-        return js['data']
+        raise QQIOError('user_detail api is not available')
 
     def user_favorite_artists(self, uid, mid, page=1, page_size=30):
         # FIXME: page/page_size is just a guess
-        url = 'https://u.y.qq.com/cgi-bin/musics.fcg'
-        data = {
+        payload = {
             'req_0': {
                 'module': 'music.concern.RelationList',
                 'method': 'GetFollowSingerList',
                 'param': {
                     'From': page - 1,
                     'Size': page_size,
                     'HostUin': mid
                 }},
             'comm': {
                 'g_tk': self.get_token_from_cookies(),
                 'uin': uid,
                 'format': 'json',
             }
         }
-        data_str = json.dumps(data)
-
-        params = {
-            '_': int(round(time.time() * 1000)),
-            'sign': _get_sign(data_str),
-            'data': data_str
-        }
-
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
+        js = self.rpc(payload)
         return js['req_0']['data']['List']
 
     def user_favorite_albums(self, uid, start=0, end=100):
-        url = api_base_url + '/fav/fcgi-bin/fcg_get_profile_order_asset.fcg'
-        params = {
-            'ct': 20,  # 不知道此字段什么含义
-            'reqtype': 2,
-            'sin': start,  # 每一页的开始
-            'ein': end,  # 每一页的结尾，目前假设最多收藏 30 个专辑
-            'cid': 205360956,
-            'reqfrom': 1,
-            'userid': uid
-        }
-        resp = requests.get(url, params=params, headers=self._headers,
-                            cookies=self._cookies, timeout=self._timeout)
-        js = resp.json()
-        if js['code'] != 0:
-            raise CodeShouldBe0(js)
-        return js['data']['albumlist']
+        raise QQIOError('user_detail api is not available')
 
     def user_favorite_playlists(self, uid, mid, start=0, end=100):
-        url = api_base_url + '/fav/fcgi-bin/fcg_get_profile_order_asset.fcg'
-
-        params = {
-            'loginUin': uid,
-            'userid': mid,
-            'cid': 205360956,
-            'sin': start,
-            'ein': end,
-            'reqtype': 3,
-            'ct': 20,  # 没有该字段 返回中文字符是乱码
-        }
-
-        resp = requests.get(url, params=params, headers=self._headers,
-                            timeout=self._timeout)
-        js = resp.json()
-        if js['code'] != 0:
-            raise CodeShouldBe0(js)
-        return js['data']['cdlist']
+        raise QQIOError('api is not available')
 
     def get_recommend_songs_pid(self):
         data = {
             'req_0': {
                 'module': 'recommend.RecommendFeedServer',
                 'method': 'get_recommend_feed',
                 'param': {
@@ -458,37 +326,26 @@
         }
         js = self.rpc(data)
         ids = [card['id']
                for card in js['req_0']['data']['v_shelf'][index]['v_niche'][0]['v_card']]
         return ids
 
     def get_lyric_by_songmid(self, songmid):
-        url = api_base_url + '/lyric/fcgi-bin/fcg_query_lyric_new.fcg'
-        params = {
-            'songmid': songmid,
-            'pcachetime': int(round(time.time() * 1000)),
-            'format': 'json',
-        }
-        response = requests.get(url, params=params, headers=self._headers,
-                                timeout=self._timeout)
-        js = response.json()
-        CodeShouldBe0.check(js)
-        lyric = js['lyric'] or ''
-        return base64.b64decode(lyric).decode()
+        raise QQIOError('get_lyric_by_songmid is not available')
 
     def rpc(self, payload):
         if 'comm' not in payload:
             payload['comm'] = self.get_common_params()
-        data_str = json.dumps(payload)
+        data_str = json.dumps(payload, ensure_ascii=False)
         params = {
             '_': int(round(time.time() * 1000)),
             'sign': _get_sign(data_str),
             'data': data_str,
         }
-        url = 'http://u.y.qq.com/cgi-bin/musicu.fcg'
+        url = 'https://u.y.qq.com/cgi-bin/musicu.fcg'
         resp = requests.get(url, params=params, headers=self._headers,
                             timeout=self._timeout)
         js = resp.json()
         CodeShouldBe0.check(js)
         return js
 
     def get_common_params(self):
@@ -581,15 +438,15 @@
             "comm": {
                 "uin": uin,
                 "format": "json",
                 "ct": 24,
                 "cv": 0
             }
         }
-        data_str = json.dumps(data)
+        data_str = json.dumps(data, ensure_ascii=False)
         params = {
             '-': 'getplaysongvkey' + str(songvkey),
             'g_tk': 5381,
             'loginUin': uin,
             'hostUin': 0,
             'format': 'json',
             'inCharset': 'utf8',
@@ -692,15 +549,15 @@
             "comm": {
                 "uin": str(uin),
                 "format": "json",
                 "ct": 19,
                 "cv": 0
             }
         }
-        data_str = json.dumps(data)
+        data_str = json.dumps(data, ensure_ascii=False)
 
         sign = _get_sign(data_str)
         params = {
             'sign': sign,
             'g_tk': 5381,
             'loginUin': '',
             'hostUin': 0,
```

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/provider.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/provider.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/page_explore.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/page_explore.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/page_daily_recommendation.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/page_daily_recommendation.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/ui.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/ui.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/__init__.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic/page_fav.py` & `fuo_qqmusic-0.5.0/fuo_qqmusic/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/setup.py` & `fuo_qqmusic-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
 
 setup(
     name='fuo_qqmusic',
-    version='0.4.1',
+    version='0.5.0',
     description='feeluown qqmusic plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=[
         'fuo_qqmusic',
     ],
     package_data={
@@ -23,15 +23,15 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
     ],
     install_requires=[
-        'feeluown>=3.5.2',
+        'feeluown<3.9',
         'requests',
         'marshmallow>=3.0'
     ],
     entry_points={
         'fuo.plugins_v1': [
             'qqmusic = fuo_qqmusic',
         ]
```

### Comparing `fuo_qqmusic-0.4.1/PKG-INFO` & `fuo_qqmusic-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fuo_qqmusic
-Version: 0.4.1
+Version: 0.5.0
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: feeluown,plugin,qqmusic
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/PKG-INFO` & `fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fuo-qqmusic
-Version: 0.4.1
+Version: 0.5.0
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: feeluown,plugin,qqmusic
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fuo_qqmusic-0.4.1/fuo_qqmusic.egg-info/SOURCES.txt` & `fuo_qqmusic-0.5.0/fuo_qqmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-0.4.1/README.md` & `fuo_qqmusic-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # feeluown QQ 音乐插件
 
 [![Build Status](https://travis-ci.com/feeluown/feeluown-qqmusic.svg?branch=master)](https://travis-ci.com/feeluown/feeluown-qqmusic)
 [![PyPI](https://img.shields.io/pypi/v/fuo_qqmusic.svg)](https://pypi.python.org/pypi/fuo-qqmusic)
 [![Coverage Status](https://coveralls.io/repos/github/feeluown/feeluown-qqmusic/badge.svg?branch=master)](https://coveralls.io/github/feeluown/feeluown-qqmusic?branch=master)
 
+
+2023-06-08：该插件可以和老版本 FeelUOwn(\<v3.9) 一起使用。
+
 ## 安装
 
 ```sh
 pip3 install fuo-qqmusic
 ```
 
 ## 使用说明
 
 ### 登录
 在网页登录微信/QQ后（在任意网站），复制请求中的 cookies 至程序登录框，
 [操作示例](https://github.com/feeluown/feeluown-qqmusic/issues/6)。
 
 ## changelog
 
+### 0.5.0 (2023-07-14)
+
+- 修复搜索接口
+- 让部分不可用接口直接报错
+
 ### 0.4.1 (2022-03-21)
 
 - 修复加载歌单时，应用可能会 crash 的问题
 
 ### 0.4.0 (???)
 
 - 修复若干问题
 
 ### 0.3.4 (2022-01-31)
 
 感谢 [@cyliuu](https://github.com/cyliuu)
 
-- 修复若干问题 
+- 修复若干问题
 
 ### 0.3.3 (2021-06-10)
 
 感谢 [@cyliuu](https://github.com/cyliuu)
 
 - 支持展示收藏的歌曲、专辑和歌手
 - 支持获取相似歌曲
```

