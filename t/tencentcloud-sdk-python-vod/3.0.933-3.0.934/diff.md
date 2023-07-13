# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.933.tar", last modified: Wed Jul 12 00:45:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.934.tar", last modified: Thu Jul 13 00:37:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.933.tar` & `tencentcloud-sdk-python-vod-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   182690 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1853917 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   182739 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:37:44.000000 tencentcloud-sdk-python-vod-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:37:45.000000 tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vod-3.0.933/setup.py` & `tencentcloud-sdk-python-vod-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/vod_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3819,37 +3819,41 @@
         - 指定文件封装格式集合 MediaTypes（见输入参数），返回满足集合中任意封装格式的媒体。例如：封装格式有 MP4、AVI、MP3 等。如果 MediaTypes 指定了 MP4 和 MP3，那么符合这些封装格式的媒体都会被检索出来。
         - 指定文件状态集合 Status（见输入参数），返回满足集合中任意状态的媒体。例如：文件状态有 Normal（正常）、SystemForbidden（平台封禁）、Forbidden（主动封禁）。如果 Status 指定了 Normal 和 Forbidden 2种文件状态，那么符合这些状态的媒体都会被检索出来。
         - 指定文件审核结果集合 ReviewResults（见输入参数），返回满足集合中任意状态的媒体。例如：文件审核结果有 pass（通过）、block（违规）等。如果 ReviewResults 指定了 pass 和 block 2种审核结果，那么符合这些审核结果的媒体都会被检索出来。
         - 指定直播推流码集合 StreamIds（见输入参数）筛选直播录制的媒体。
         - 指定媒体的创建时间范围筛选媒体。
         - 指定 TRTC 应用 ID 集合筛选媒体。
         - 指定 TRTC 房间 ID 集合筛选媒体。
-        - （不推荐：应使用 Names、NamePrefixes 或 Descriptions 替代）指定单个文本 Text 对媒体文件名或描述信息进行模糊搜索。
-        - （不推荐：应使用 SourceTypes 替代）指定单个媒体文件来源 SourceType 进行搜索。
-        - （不推荐：应使用 StreamIds 替代）指定单个推流直播码 StreamId 进行搜索。
-        - （不推荐：应使用 CreateTime 替代）指定单个起始创建时间 StartTime 进行搜索。
-        - （不推荐：应使用 CreateTime 替代）指定单个结尾创建时间 EndTime 进行搜索。
+
         - 以上参数之间可以任意组合进行检索。例如：筛选创建时间在2018年12月1日12:00:00到2018年12月8日12:00:00之间、分类为电影或电视剧、带有宫斗和悬疑标签的媒体。注意，任何支持数组输入的参数，其元素之间的搜索逻辑为‘或’。所有参数之间的逻辑关系为‘与’。
 
-        - 允许对结果根据创建时间进行排序并分页返回，通过 Offset 和 Limit （见输入参数）来控制分页。
         - 允许通过 Filters 控制返回的媒体信息种类（默认返回所有信息）。可选输入包括：
             1. 基础信息（basicInfo）：包括媒体名称、分类、播放地址、封面图片等。
             2. 元信息（metaData）：包括大小、时长、视频流信息、音频流信息等。
             3. 转码结果信息（transcodeInfo）：包括该媒体转码生成的各种规格的媒体地址、视频流参数、音频流参数等。
             4. 转动图结果信息（animatedGraphicsInfo）：对视频转动图（如 gif）后的动图信息。
             5. 采样截图信息（sampleSnapshotInfo）：对视频采样截图后的截图信息。
             6. 雪碧图信息（imageSpriteInfo）：对视频截取雪碧图后的雪碧图信息。
             7. 指定时间点截图信息（snapshotByTimeOffsetInfo）：对视频依照指定时间点截图后，的截图信息。
             8. 视频打点信息（keyFrameDescInfo）：对视频设置的打点信息。
             9. 转自适应码流信息（adaptiveDynamicStreamingInfo）：包括规格、加密类型、打包格式等相关信息。
 
+        - 允许对结果根据创建时间进行排序并分页返回，通过 Offset 和 Limit （见输入参数）来控制分页。
+
         <div id="maxResultsDesc">接口返回结果数限制：</div>
         - <b><a href="#p_offset">Offset</a> 和 <a href="#p_limit">Limit</a> 两个参数影响单次分页查询结果数。特别注意：当这2个值都缺省时，本接口最多只返回10条查询结果。</b>
         - <b>最大支持返回5000条搜索结果，超出部分不再支持查询。如果搜索结果量太大，建议使用更精细的筛选条件来减少搜索结果。</b>
 
+        <br>不推荐使用的条件筛选：
+        - （不推荐：应使用 Names、NamePrefixes 或 Descriptions 替代）指定单个文本 Text 对媒体文件名或描述信息进行模糊搜索。
+        - （不推荐：应使用 SourceTypes 替代）指定单个媒体文件来源 SourceType 进行搜索。
+        - （不推荐：应使用 StreamIds 替代）指定单个推流直播码 StreamId 进行搜索。
+        - （不推荐：应使用 CreateTime 替代）指定单个起始创建时间 StartTime 进行搜索。
+        - （不推荐：应使用 CreateTime 替代）指定单个结尾创建时间 EndTime 进行搜索。
+
         :param request: Request instance for SearchMedia.
         :type request: :class:`tencentcloud.vod.v20180717.models.SearchMediaRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.SearchMediaResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.934/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -31416,15 +31416,18 @@
 
     def __init__(self):
         r"""
         :param _Type: 所指定的删除部分。如果未填写该字段则参数无效。可选值有：
 <li>OriginalFiles（删除原文件，删除后无法发起转码、微信发布等任何视频处理操作）；</li>
 <li>TranscodeFiles（删除转码文件）；</li>
 <li>AdaptiveDynamicStreamingFiles（删除转自适应码流文件）；</li>
-<li>WechatPublishFiles（删除微信发布文件）。</li>
+<li>WechatPublishFiles（删除微信发布文件）；</li>
+<li>WechatMiniProgramPublishFiles（删除微信小程序发布文件）。</li>
+<font color=red>注意：</font> <li>取值为OriginalFiles时，文件上传时携带的封面文件会被删除；</li>
+<li>取值为TranscodeFiles时，媒体处理产生的封面文件会被删除。</li>
         :type Type: str
         :param _Definition: 删除由Type参数指定的种类下的视频模板号，模板定义参见[转码模板](https://cloud.tencent.com/document/product/266/33478#.3Cspan-id-.3D-.22zm.22-.3E.3C.2Fspan.3E.E8.BD.AC.E7.A0.81.E6.A8.A1.E6.9D.BF)。
 默认值为0，表示删除参数Type指定种类下所有的视频。
         :type Definition: int
         """
         self._Type = None
         self._Definition = None
@@ -49723,36 +49726,14 @@
         :type StreamIds: list of str
         :param _CreateTime: 匹配创建时间在此时间段内的文件。
 <li>包含所指定的头尾时间点。</li>
         :type CreateTime: :class:`tencentcloud.vod.v20180717.models.TimeRange`
         :param _ExpireTime: 匹配过期时间在此时间段内的文件，无法检索到已过期文件。
 <li>包含所指定的头尾时间点。</li>
         :type ExpireTime: :class:`tencentcloud.vod.v20180717.models.TimeRange`
-        :param _Sort: 排序方式。
-<li>Sort.Field 可选 CreateTime 。</li>
-<li>当 Text、 Names 或 Descriptions 不为空时，Sort.Field 字段无效， 搜索结果将以匹配度排序。</li>
-        :type Sort: :class:`tencentcloud.vod.v20180717.models.SortBy`
-        :param _Offset: <div id="p_offset">分页返回的起始偏移量，默认值：0。将返回第 Offset 到第 Offset+Limit-1 条。
-<li>取值范围：Offset + Limit 不超过5000。（参见：<a href="#maxResultsDesc">接口返回结果数限制</a>）</li></div>
-        :type Offset: int
-        :param _Limit: <div id="p_limit">分页返回的记录条数，默认值：10。将返回第 Offset 到第 Offset+Limit-1 条。
-<li>取值范围：Offset + Limit 不超过5000。（参见：<a href="#maxResultsDesc">接口返回结果数限制</a>）</li></div>
-        :type Limit: int
-        :param _Filters: 指定所有媒体文件需要返回的信息，可同时指定多个信息，N 从 0 开始递增。如果未填写该字段，默认返回所有信息。选项有：
-<li>basicInfo（视频基础信息）。</li>
-<li>metaData（视频元信息）。</li>
-<li>transcodeInfo（视频转码结果信息）。</li>
-<li>animatedGraphicsInfo（视频转动图结果信息）。</li>
-<li>imageSpriteInfo（视频雪碧图信息）。</li>
-<li>snapshotByTimeOffsetInfo（视频指定时间点截图信息）。</li>
-<li>sampleSnapshotInfo（采样截图信息）。</li>
-<li>keyFrameDescInfo（打点信息）。</li>
-<li>adaptiveDynamicStreamingInfo（转自适应码流信息）。</li>
-<li>miniProgramReviewInfo（小程序审核信息）。</li>
-        :type Filters: list of str
         :param _StorageRegions: 媒体文件存储地区，如 ap-chongqing，参见[地域列表](https://cloud.tencent.com/document/product/266/9760#.E5.B7.B2.E6.94.AF.E6.8C.81.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8)。
 <li>单个存储地区长度限制：20个字符。</li>
 <li>数组长度限制：20。</li>
         :type StorageRegions: list of str
         :param _StorageClasses: 存储类型数组。可选值有：
 <li> STANDARD：标准存储。</li>
 <li> STANDARD_IA：低频存储。</li>
@@ -49776,14 +49757,36 @@
         :param _TrtcSdkAppIds: TRTC 应用 ID 集合。匹配集合中的任意元素。
 <li>数组长度限制：10。</li>
         :type TrtcSdkAppIds: list of int non-negative
         :param _TrtcRoomIds: TRTC 房间 ID 集合。匹配集合中的任意元素。
 <li>单个房间 ID 长度限制：64个字符；</li>
 <li>数组长度限制：10。</li>
         :type TrtcRoomIds: list of str
+        :param _Filters: 指定所有媒体文件需要返回的信息，可同时指定多个信息，N 从 0 开始递增。如果未填写该字段，默认返回所有信息。选项有：
+<li>basicInfo（视频基础信息）。</li>
+<li>metaData（视频元信息）。</li>
+<li>transcodeInfo（视频转码结果信息）。</li>
+<li>animatedGraphicsInfo（视频转动图结果信息）。</li>
+<li>imageSpriteInfo（视频雪碧图信息）。</li>
+<li>snapshotByTimeOffsetInfo（视频指定时间点截图信息）。</li>
+<li>sampleSnapshotInfo（采样截图信息）。</li>
+<li>keyFrameDescInfo（打点信息）。</li>
+<li>adaptiveDynamicStreamingInfo（转自适应码流信息）。</li>
+<li>miniProgramReviewInfo（小程序审核信息）。</li>
+        :type Filters: list of str
+        :param _Sort: 排序方式。
+<li>Sort.Field 可选 CreateTime 。</li>
+<li>当 Text、 Names 或 Descriptions 不为空时，Sort.Field 字段无效， 搜索结果将以匹配度排序。</li>
+        :type Sort: :class:`tencentcloud.vod.v20180717.models.SortBy`
+        :param _Offset: <div id="p_offset">分页返回的起始偏移量，默认值：0。将返回第 Offset 到第 Offset+Limit-1 条。
+<li>取值范围：Offset + Limit 不超过5000。（参见：<a href="#maxResultsDesc">接口返回结果数限制</a>）</li></div>
+        :type Offset: int
+        :param _Limit: <div id="p_limit">分页返回的记录条数，默认值：10。将返回第 Offset 到第 Offset+Limit-1 条。
+<li>取值范围：Offset + Limit 不超过5000。（参见：<a href="#maxResultsDesc">接口返回结果数限制</a>）</li></div>
+        :type Limit: int
         :param _Text: （不推荐：应使用 Names、NamePrefixes 或 Descriptions 替代）
 搜索文本，模糊匹配媒体文件名称或描述信息，匹配项越多，匹配度越高，排序越优先。长度限制：64个字符。
         :type Text: str
         :param _SourceType: （不推荐：应使用 SourceTypes 替代）
 媒体文件来源，来源取值参见 [SourceType](https://cloud.tencent.com/document/product/266/31773#MediaSourceData)。
         :type SourceType: str
         :param _StreamId: （不推荐：应使用 StreamIds 替代）
@@ -49814,25 +49817,25 @@
         self._ClassIds = None
         self._Tags = None
         self._Categories = None
         self._SourceTypes = None
         self._StreamIds = None
         self._CreateTime = None
         self._ExpireTime = None
-        self._Sort = None
-        self._Offset = None
-        self._Limit = None
-        self._Filters = None
         self._StorageRegions = None
         self._StorageClasses = None
         self._MediaTypes = None
         self._Status = None
         self._ReviewResults = None
         self._TrtcSdkAppIds = None
         self._TrtcRoomIds = None
+        self._Filters = None
+        self._Sort = None
+        self._Offset = None
+        self._Limit = None
         self._Text = None
         self._SourceType = None
         self._StreamId = None
         self._StartTime = None
         self._EndTime = None
         self._Vids = None
         self._Vid = None
@@ -49930,46 +49933,14 @@
         return self._ExpireTime
 
     @ExpireTime.setter
     def ExpireTime(self, ExpireTime):
         self._ExpireTime = ExpireTime
 
     @property
-    def Sort(self):
-        return self._Sort
-
-    @Sort.setter
-    def Sort(self, Sort):
-        self._Sort = Sort
-
-    @property
-    def Offset(self):
-        return self._Offset
-
-    @Offset.setter
-    def Offset(self, Offset):
-        self._Offset = Offset
-
-    @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
-    def Filters(self):
-        return self._Filters
-
-    @Filters.setter
-    def Filters(self, Filters):
-        self._Filters = Filters
-
-    @property
     def StorageRegions(self):
         return self._StorageRegions
 
     @StorageRegions.setter
     def StorageRegions(self, StorageRegions):
         self._StorageRegions = StorageRegions
 
@@ -50018,14 +49989,46 @@
         return self._TrtcRoomIds
 
     @TrtcRoomIds.setter
     def TrtcRoomIds(self, TrtcRoomIds):
         self._TrtcRoomIds = TrtcRoomIds
 
     @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def Sort(self):
+        return self._Sort
+
+    @Sort.setter
+    def Sort(self, Sort):
+        self._Sort = Sort
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
     def Text(self):
         return self._Text
 
     @Text.setter
     def Text(self, Text):
         self._Text = Text
 
@@ -50091,27 +50094,27 @@
         self._StreamIds = params.get("StreamIds")
         if params.get("CreateTime") is not None:
             self._CreateTime = TimeRange()
             self._CreateTime._deserialize(params.get("CreateTime"))
         if params.get("ExpireTime") is not None:
             self._ExpireTime = TimeRange()
             self._ExpireTime._deserialize(params.get("ExpireTime"))
-        if params.get("Sort") is not None:
-            self._Sort = SortBy()
-            self._Sort._deserialize(params.get("Sort"))
-        self._Offset = params.get("Offset")
-        self._Limit = params.get("Limit")
-        self._Filters = params.get("Filters")
         self._StorageRegions = params.get("StorageRegions")
         self._StorageClasses = params.get("StorageClasses")
         self._MediaTypes = params.get("MediaTypes")
         self._Status = params.get("Status")
         self._ReviewResults = params.get("ReviewResults")
         self._TrtcSdkAppIds = params.get("TrtcSdkAppIds")
         self._TrtcRoomIds = params.get("TrtcRoomIds")
+        self._Filters = params.get("Filters")
+        if params.get("Sort") is not None:
+            self._Sort = SortBy()
+            self._Sort._deserialize(params.get("Sort"))
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
         self._Text = params.get("Text")
         self._SourceType = params.get("SourceType")
         self._StreamId = params.get("StreamId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Vids = params.get("Vids")
         self._Vid = params.get("Vid")
```

### Comparing `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.934/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.933'
+__version__ = '3.0.934'
```

### Comparing `tencentcloud-sdk-python-vod-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.934/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.933/README.rst` & `tencentcloud-sdk-python-vod-3.0.934/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.934/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

