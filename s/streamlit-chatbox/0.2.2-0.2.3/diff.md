# Comparing `tmp/streamlit_chatbox-0.2.2-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5003 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    10013 b- defN 23-Jun-28 13:06 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      425 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/RECORD
-5 files, 12889 bytes uncompressed, 4207 bytes compressed:  67.4%
+Zip file size: 5106 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    10021 b- defN 23-Jul-13 08:41 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     2607 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      425 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/RECORD
+5 files, 13163 bytes uncompressed, 4310 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.2.2.dist-info/METADATA
+Filename: streamlit_chatbox-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.2.2.dist-info/WHEEL
+Filename: streamlit_chatbox-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.2.2.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.2.2.dist-info/RECORD
+Filename: streamlit_chatbox-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -177,15 +177,15 @@
                     self.last_response = empty
         return self.last_response
 
     def update_last_box_text(self, msg):
         if self.last_response is not None:
             self.history[-1]['content'] = msg
             self.last_response.markdown(
-                self.format_md(msg, False),
+                self.format_md(msg + '▌', False),
                 unsafe_allow_html=True
             )
 
     def robot_stream(self, msg, init_msg='', words_per_sec=10, max_seconds=10):
         step = max(words_per_sec, len(msg) // max_seconds + 1) // 5 + 1
         self.robot_say(init_msg)
         self.output_messages()
```

## Comparing `streamlit_chatbox-0.2.2.dist-info/METADATA` & `streamlit_chatbox-0.2.3.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,91 @@
-Metadata-Version: 2.1
-Name: streamlit-chatbox
-Version: 0.2.2
-Summary: A chat box used in streamlit
-Home-page: https://github.com/liunux4odoo/streamlit-chatbox
-Author: liunux
-Author-email: liunux@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: streamlit
-
-# Attention!
-
-Since version 1.24.0 streamlit provides official elements to [build conversational apps](https://docs.streamlit.io/knowledge-base/tutorials/build-conversational-apps).
-
-The new elements are more flexible, extensible and better supported, I would suggest to use them. 
-
-
-# Chatbox component for streamlit
-
-A Streamlit component to show chat messages.
-
-## Features
-
-- user can custom the bg_color and icon of message senders.
-- support streaming output.
-- support image/video/audio messages
-
-
-This make it easy to chat with LLMs in streamlit.
-
-
-## Install
-
-just `pip install streamlit-chatbox`
-
-## Usage examples
-
-```python
-import streamlit as st
-from streamlit_chatbox import st_chatbox, MsgType
-import time
-
-
-st.write('start to chat')
-streaming = st.checkbox('streaming', False)
-chat_box = st_chatbox(
-	greetings=['welcome to chat', '\n```streamlit``` is a great tool!'])
-# use help(st_chatbox) to see costom params
-
-q = st.text_input('input', placeholder='input your question here')
-if q:
-    chat_box.user_say(q)
-    text = f'my answer to:\n\n{q}\n\n```this is some code```'
-    if streaming:
-        chat_box.robot_stream(text)
-    else:
-        chat_box.robot_say(text)
-
-    chat_box.robot_say('https://tse4-mm.cn.bing.net/th/id/OIP-C.cy76ifbr2oQPMEs2H82D-QHaEv?w=284&h=181&c=7&r=0&o=5&dpr=1.5&pid=1.7', MsgType.IMAGE)
-
-    chat_box.robot_say('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4', MsgType.VIDEO, format='viedo/mp4')
-
-    chat_box.robot_say('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4', MsgType.AUDIO, format='audio/mp4')
-
-chat_box.output_messages()
-```
-
-![demo](https://github.com/liunux4odoo/streamlit-chatbox/blob/master/demo.gif)
-
-
-## Todos
-
-- input messages:
-	- [x] TEXT
-	- [ ] IMAGE
-		- [ ] file upload
-		- [ ] paste from clipboard(streamlit_bokeh_events)
-	- [ ] VIDEO
-		- [ ] file upload
-	- [ ] AUDIO
-		- [ ] file upload
-		- [ ] audio-recorder-streamlit
-
-- output messages:
-	- [x] TEXT
-	- [x] IMAGE
-	- [x] VIDEO
-	- [x] AUDIO
-
-
+Metadata-Version: 2.1
+Name: streamlit-chatbox
+Version: 0.2.3
+Summary: A chat box used in streamlit
+Home-page: https://github.com/liunux4odoo/streamlit-chatbox
+Author: liunux
+Author-email: liunux@qq.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: streamlit
+
+# Attention!
+
+Since version 1.24.0 streamlit provides official elements to [build conversational apps](https://docs.streamlit.io/knowledge-base/tutorials/build-conversational-apps).
+
+The new elements are more flexible, extensible and better supported, I would suggest to use them. 
+
+However, streamlit>=1.23 requires protobuf>=4 when some package requires protobuf<=3. In this condition you can use this package with streamlit<=1.22 as alternative. They are all simple to render text messages.
+
+
+# Chatbox component for streamlit
+
+A Streamlit component to show chat messages.
+
+## Features
+
+- user can custom the bg_color and icon of message senders.
+- support streaming output.
+- support image/video/audio messages
+
+
+This make it easy to chat with LLMs in streamlit.
+
+
+## Install
+
+just `pip install streamlit-chatbox`
+
+## Usage examples
+
+```python
+import streamlit as st
+from streamlit_chatbox import st_chatbox, MsgType
+import time
+
+
+st.write('start to chat')
+streaming = st.checkbox('streaming', False)
+chat_box = st_chatbox(
+	greetings=['welcome to chat', '\n```streamlit``` is a great tool!'])
+# use help(st_chatbox) to see costom params
+
+q = st.text_input('input', placeholder='input your question here')
+if q:
+    chat_box.user_say(q)
+    text = f'my answer to:\n\n{q}\n\n```this is some code```'
+    if streaming:
+        chat_box.robot_stream(text)
+    else:
+        chat_box.robot_say(text)
+
+    chat_box.robot_say('https://tse4-mm.cn.bing.net/th/id/OIP-C.cy76ifbr2oQPMEs2H82D-QHaEv?w=284&h=181&c=7&r=0&o=5&dpr=1.5&pid=1.7', MsgType.IMAGE)
+
+    chat_box.robot_say('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4', MsgType.VIDEO, format='viedo/mp4')
+
+    chat_box.robot_say('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4', MsgType.AUDIO, format='audio/mp4')
+
+chat_box.output_messages()
+```
+
+![demo](https://github.com/liunux4odoo/streamlit-chatbox/blob/master/demo.gif)
+
+
+## Todos
+
+- input messages:
+	- [x] TEXT
+	- [ ] IMAGE
+		- [ ] file upload
+		- [ ] paste from clipboard(streamlit_bokeh_events)
+	- [ ] VIDEO
+		- [ ] file upload
+	- [ ] AUDIO
+		- [ ] file upload
+		- [ ] audio-recorder-streamlit
+
+- output messages:
+	- [x] TEXT
+	- [x] IMAGE
+	- [x] VIDEO
+	- [x] AUDIO
```

