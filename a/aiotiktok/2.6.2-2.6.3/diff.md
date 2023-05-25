# Comparing `tmp/aiotiktok-2.6.2.tar.gz` & `tmp/aiotiktok-2.6.3.tar.gz`

## Comparing `aiotiktok-2.6.2.tar` & `aiotiktok-2.6.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/__init__.py
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/client.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/constants.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/exceptions.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/extractors.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/types.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/LICENSE
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/README.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/client.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/constants.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/extractors.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/aiotiktok/types.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/LICENSE
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/README.rst
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 aiotiktok-2.6.3/PKG-INFO
```

### Comparing `aiotiktok-2.6.2/aiotiktok/client.py` & `aiotiktok-2.6.3/aiotiktok/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class Client:
     def __init__(self, signature_url: str = "http://127.0.0.1:8002/signature") -> None:
         self.signature_url = signature_url
         self.api_headers = {
             "user-agent": "com.ss.android.ugc.trill/2613 (Linux; U; Android 10; en_US; Pixel 4; "
-                          "Build/QQ3A.200805.001; Cronet/58.0.2991.0)"
+            "Build/QQ3A.200805.001; Cronet/58.0.2991.0)"
         }
         self.base_url = "https://www.tiktok.com/"
         self.api_url = (
             "https://api16-normal-c-useast1a.tiktokv.com/aweme/v1/feed/?aweme_id={}"
         )
         self.headers = {
             "Accept-Encoding": "gzip, deflate",
@@ -32,37 +32,39 @@
         }
 
     async def _request(
         self,
         url: str,
         method: str = "GET",
         params: dict | None = None,
-        data: dict | str | None = None,
+        data: dict | None = None,
         headers: dict | None = None,
         allow_redirects: bool = True,
     ) -> dict:
         async with AsyncClient() as session:
             response = await session.request(
                 method=method,
                 url=url,
                 params=params,
                 data=data,
                 headers=headers,
                 follow_redirects=allow_redirects,
             )
             response_headers = response.headers
             try:
-                response = response.json()
+                response_data = response.json()
             except json.decoder.JSONDecodeError:
-                response = response.read()
-        return dict(response=response, headers=response_headers)
+                response_data = response.read()
+        return dict(response=response_data, headers=response_headers)
 
     async def get_video_id(self, url: str) -> str:
         if "@" not in url:
-            headers = (await self._request(url, allow_redirects=False)).get("headers")
+            headers = (await self._request(url, allow_redirects=False)).get(
+                "headers", {}
+            )
             url = headers.get("Location").split("?")[0]
         if url == self.base_url or "video" not in url:
             raise URLUnavailable("URLUnavailable, check the link")
         video_id = re.findall("/video/(\d+)", url)[0]
         return video_id
 
     async def video_data(
@@ -70,72 +72,76 @@
     ) -> VideoData:
         """
         Get TikTok data
         :param video_id: id of video:
         :param url: url to video
         :return: :class:`aiotiktok.types.VideoData`
         """
-        if video_id is None:
+        if video_id is None and url:
             video_id = await self.get_video_id(url)
         api_link = self.api_url.format(video_id)
         data = (
             (await self._request(api_link, headers=self.api_headers))
             .get("response", {})
             .get("aweme_list", {})[0]
         )
         if data and data.get("aweme_id") == str(video_id):
             return extract_video_data(data)
         raise VideoUnavailable("VideoUnavailable")
 
-    async def user_feed(self, username: str, count: int = None) -> list[VideoData]:
+    async def user_feed(
+        self, username: str, count: int | None = None
+    ) -> list[VideoData]:
         """
         Get user feed, only 30 videos.
         :param username:
         :param count:
         :return: list[:class:`aiotiktok.types.VideoData`]
         """
         url = urljoin(self.base_url, f"@{username}")
         response = await self._request(url, headers=self.headers)
-        data = extract_data_from_html(response.get("response").decode())
+        data = extract_data_from_html(response.get("response", b"").decode())
         item_module = data.get("ItemModule")
         videos = []
         for video in list(item_module.values())[:count]:
             videos.append(await self.video_data(video_id=video.get("id")))
         return videos
 
     async def user_info(self, username: str) -> Author:
         """
         Get UserInfo
         :param username:
         :return :class:`aiotiktok.types.Author`:
         """
         url = urljoin(self.base_url, f"@{username}")
         response = await self._request(url, headers=self.headers)
-        data = extract_data_from_html(response.get("response").decode())
+        data = extract_data_from_html(response.get("response", b"").decode())
         return extract_user_data(data)
 
     async def sign_url(self, url: str) -> dict:
         request = await self._request(
             url=self.signature_url, method="POST", data={"url": url}
         )
         return request.get("response", {})
 
-    async def _get_user_feed_private(self, username: str, count: int | None = None) -> list[dict]:
+    async def _get_user_feed_private(
+        self, username: str, count: int | None = None
+    ) -> list[dict]:
         sec_uid = (await self.user_info(username)).sec_uid
         params = default_user_videos_params
         params.update({"secUid": sec_uid})
         unsigned_url = f"{static_unsigned_user_videos}{urlencode(params)}"
         signature_data = await self.sign_url(unsigned_url)
         headers = {
             "x-tt-params": signature_data.get("x-tt-params"),
             "user-agent": signature_data.get("navigator", {}).get("user_agent"),
         }
         api_response = (
             await self._request(url=static_user_videos_url, headers=headers)
-        ).get("response")
+        ).get("response", {})
         user_videos = [video for video in api_response.get("itemList", [])]
         has_more = api_response.get("hasMore")
         while has_more and len(user_videos) < count if count else None:
             cursor = api_response.get("cursor")
             params.update({"cursor": cursor})
             unsigned_url = f"{static_unsigned_user_videos}{urlencode(params)}"
             signature_data = await self.sign_url(unsigned_url)
@@ -143,15 +149,17 @@
             api_response = (
                 await self._request(url=static_user_videos_url, headers=headers)
             ).get("response")
             user_videos.extend(api_response.get("itemList"))
             has_more = api_response.get("hasMore")
         return user_videos
 
-    async def user_feed_sig(self, username: str, count: int | None = None) -> list[VideoData]:
+    async def user_feed_sig(
+        self, username: str, count: int | None = None
+    ) -> list[VideoData]:
         """
         Get user feed with private signature, for use that method you must up your application
         https://github.com/sheldygg/aiotiktok#signature
         :param username:
         :param count:
         :return: list[:class:`aiotiktok.types.VideoData`]
         """
```

### Comparing `aiotiktok-2.6.2/aiotiktok/constants.py` & `aiotiktok-2.6.3/aiotiktok/constants.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.2/aiotiktok/extractors.py` & `aiotiktok-2.6.3/aiotiktok/extractors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,79 @@
 import json
 import re
 
-from .types import Album, Author, Music, Video, VideoData, VideoType, video_type_codes
+from .types import (
+    Album,
+    Author,
+    Music,
+    Statistics,
+    Video,
+    VideoData,
+    VideoType,
+    video_type_codes,
+)
+
+
+def create_url_to_video(username: str, video_id: str):
+    return f"https://www.tiktok.com/@{username}/video/{video_id}"
 
 
 def extract_video_data(data: dict) -> VideoData:
     video_type = video_type_codes.get(data["aweme_type"], VideoType.VIDEO)
     if video_type == VideoType.ALBUM:
-        images_list = []
-        for images in data["image_post_info"]["images"]:
-            images_list.append(images["display_image"]["url_list"][0])
-        media = Album(urls=images_list)
-    else:
+        media = Album(
+            urls=[
+                images["display_image"]["url_list"][0]
+                for images in data["image_post_info"]["images"]
+            ]
+        )
+    elif video_type == VideoType.VIDEO:
         media = Video(url=data["video"]["play_addr"]["url_list"][0])
-    author_data = data.get("author")
+    else:
+        media = None
+    author_data = data.get("author", {})
+    author = Author(
+        id=author_data.get("id"),
+        nickname=author_data.get("nickname"),
+        unique_id=author_data.get("unique_id"),
+        avatar=author_data.get("avatar_larger", {}).get("url_list")[0],
+        sec_uid=author_data.get("sec_uid"),
+    )
+    statistics = data.get("statistics", {})
     return VideoData(
+        url=create_url_to_video(author.unique_id, data.get("aweme_id", "")),
         video_type=video_type,
         media=media,
         cover=data["video"]["cover"]["url_list"][0],
         dynamic_cover=data["video"]["dynamic_cover"]["url_list"][0],
         description=data["desc"],
-        play_count=data["statistics"]["comment_count"],
-        comment_count=data["statistics"]["comment_count"],
-        download_count=data["statistics"]["download_count"],
-        share_count=data["statistics"]["share_count"],
-        create_time=data["create_time"],
-        author=Author(
-            id=author_data.get("id"),
-            nickname=author_data.get("nickname"),
-            unique_id=author_data.get("unique_id"),
-            avatar=author_data.get("avatar_larger", {}).get("url_list")[0],
+        statistics=Statistics(
+            likes=statistics.get("digg_count"),
+            plays=statistics.get("play_count"),
+            comments=statistics.get("comment_count"),
+            downloads=statistics.get("download_count"),
+            shares=statistics.get("share_count"),
+            saves=statistics.get("collect_count"),
         ),
+        create_time=data["create_time"],
+        author=author,
         music=Music(
             title=data["music"]["title"],
             author=data["music"]["author"],
             url=data["music"]["play_url"]["uri"],
             cover=data["music"]["cover_large"]["url_list"][0],
         ),
     )
 
 
 def extract_data_from_html(data: str):
     pattern = r'<script id="SIGI_STATE" type="application\/json">(.*?)<\/script>'
     match = re.search(pattern, data, re.S)
-    return json.loads(match.group(1))
+    if match:
+        return json.loads(match.group(1))
 
 
 def extract_user_data(data: dict):
     user_data = list(data.get("UserModule", {}).get("users", {}).values())[0]
     return Author(
         id=user_data.get("id"),
         unique_id=user_data.get("uniqueId"),
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_lbw9tg1b_/tmpddomc42s_TarContainer/0/4.py", line 58, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_lbw9tg1b_/tmpddomc42s_TarContainer/0/4.py", line 58, column 0: CDATA terminal not found*

```diff
@@ -1,19 +1,24 @@
-import json import re from .types import Album, Author, Music, Video,
-VideoData, VideoType, video_type_codes def extract_video_data(data: dict) -
-> VideoData: video_type = video_type_codes.get(data["aweme_type"],
-VideoType.VIDEO) if video_type == VideoType.ALBUM: images_list = [] for images
-in data["image_post_info"]["images"]: images_list.append(images
-["display_image"]["url_list"][0]) media = Album(urls=images_list) else: media =
-Video(url=data["video"]["play_addr"]["url_list"][0]) author_data = data.get
-("author") return VideoData( video_type=video_type, media=media, cover=data
-["video"]["cover"]["url_list"][0], dynamic_cover=data["video"]["dynamic_cover"]
-["url_list"][0], description=data["desc"], play_count=data["statistics"]
-["comment_count"], comment_count=data["statistics"]["comment_count"],
-download_count=data["statistics"]["download_count"], share_count=data
-["statistics"]["share_count"], create_time=data["create_time"], author=Author
+import json import re from .types import ( Album, Author, Music, Statistics,
+Video, VideoData, VideoType, video_type_codes, ) def create_url_to_video
+(username: str, video_id: str): return f"https://www.tiktok.com/@{username}/
+video/{video_id}" def extract_video_data(data: dict) -> VideoData: video_type =
+video_type_codes.get(data["aweme_type"], VideoType.VIDEO) if video_type ==
+VideoType.ALBUM: media = Album( urls=[ images["display_image"]["url_list"][0]
+for images in data["image_post_info"]["images"] ] ) elif video_type ==
+VideoType.VIDEO: media = Video(url=data["video"]["play_addr"]["url_list"][0])
+else: media = None author_data = data.get("author", {}) author = Author
 ( id=author_data.get("id"), nickname=author_data.get("nickname"),
 unique_id=author_data.get("unique_id"), avatar=author_data.get("avatar_larger",
-{}).get("url_list")[0], ), music=Music( title=data["music"]["title"],
+{}).get("url_list")[0], sec_uid=author_data.get("sec_uid"), ) statistics =
+data.get("statistics", {}) return VideoData( url=create_url_to_video
+(author.unique_id, data.get("aweme_id", "")), video_type=video_type,
+media=media, cover=data["video"]["cover"]["url_list"][0], dynamic_cover=data
+["video"]["dynamic_cover"]["url_list"][0], description=data["desc"],
+statistics=Statistics( likes=statistics.get("digg_count"), plays=statistics.get
+("play_count"), comments=statistics.get("comment_count"),
+downloads=statistics.get("download_count"), shares=statistics.get
+("share_count"), saves=statistics.get("collect_count"), ), create_time=data
+["create_time"], author=author, music=Music( title=data["music"]["title"],
 author=data["music"]["author"], url=data["music"]["play_url"]["uri"],
 cover=data["music"]["cover_large"]["url_list"][0], ), ) def
 extract_data_from_html(data: str): pattern = r'
```

### Comparing `aiotiktok-2.6.2/aiotiktok/types.py` & `aiotiktok-2.6.3/aiotiktok/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,43 +15,50 @@
     55: VideoType.VIDEO,
     58: VideoType.VIDEO,
     61: VideoType.VIDEO,
     150: VideoType.ALBUM,
 }
 
 
-class Video(Struct):
+class Video(Struct, array_like=True):
     url: str
 
 
-class Album(Struct):
+class Album(Struct, array_like=True):
     urls: list[str]
 
 
-class Author(Struct, kw_only=True):
-    id: str
+class Author(Struct, array_like=True):
     unique_id: str
     nickname: str
-    sec_uid: str | None = None
     avatar: str
+    id: str | None = None
+    sec_uid: str | None = None
 
 
-class Music(Struct):
+class Music(Struct, array_like=True):
     title: str
     author: str
     url: str
     cover: str
 
 
-class VideoData(Struct):
+class Statistics(Struct, array_like=True):
+    likes: int
+    plays: int
+    comments: int
+    downloads: int
+    shares: int
+    saves: int
+
+
+class VideoData(Struct, array_like=True):
+    url: str
     video_type: VideoType
-    media: Video | Album
+    media: Video | Album | None
     cover: str
     dynamic_cover: str
     description: str
-    play_count: int
-    comment_count: int
-    download_count: int
-    share_count: int
+    statistics: Statistics
     create_time: datetime
     author: Author
     music: Music
```

### Comparing `aiotiktok-2.6.2/.gitignore` & `aiotiktok-2.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.2/LICENSE` & `aiotiktok-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.2/README.rst` & `aiotiktok-2.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.2/pyproject.toml` & `aiotiktok-2.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,8 +32,11 @@
 path = "aiotiktok/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/aiotiktok",
 ]
 [tool.isort]
-profile = "black"
+profile = "black"
+
+[tool.ruff]
+line-length = 99
```

### Comparing `aiotiktok-2.6.2/PKG-INFO` & `aiotiktok-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotiktok
-Version: 2.6.2
+Version: 2.6.3
 Summary: Tool for parse tiktok data
 Project-URL: Homepage, https://github.com/sheldygg/aiotiktok
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

