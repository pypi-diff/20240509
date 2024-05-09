# Comparing `tmp/fuo_netease-1.0.2.tar.gz` & `tmp/fuo_netease-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_netease-1.0.2.tar", last modified: Fri May  3 13:29:33 2024, max compression
+gzip compressed data, was "fuo_netease-1.0.3.tar", last modified: Thu May  9 16:49:22 2024, max compression
```

## Comparing `fuo_netease-1.0.2.tar` & `fuo_netease-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/assets/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/cloud_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/login_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (127)    19219 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/fuo_netease/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/fuo_netease/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/fuo_netease/cloud_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/cloud_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/cloud_helpers/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/cloud_helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/login_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19729 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/fuo_netease/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/fuo_netease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 16:49:22.000000 fuo_netease-1.0.3/fuo_netease.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 16:49:22.738326 fuo_netease-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 16:49:20.000000 fuo_netease-1.0.3/setup.py
```

### Comparing `fuo_netease-1.0.2/PKG-INFO` & `fuo_netease-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_netease
-Version: 1.0.2
+Version: 1.0.3
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-1.0.2/README.md` & `fuo_netease-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 ## 安装
 
 ```sh
 pip3 install fuo-netease
 ```
 
 ## changelog
+### 1.0.3 (2024-05-10)
+- 忽略试听片段（将这类歌曲视作没有资源的歌曲）
+
 ### 1.0.2 (2024-05-03)
 - 修复歌手歌曲列表
 
 ### 1.0.1 (2024-03-04)
 - 支持识别 vip 歌曲
 - 修复纯音乐歌曲的歌词
```

### Comparing `fuo_netease-1.0.2/fuo_netease/__init__.py` & `fuo_netease-1.0.3/fuo_netease/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/api.py` & `fuo_netease-1.0.3/fuo_netease/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,14 +626,21 @@
 
     def djradio_list(self, radio_id, limit=50, offset=0, asc=False):
         data = dict(radioId=radio_id, limit=limit, offset=offset, asc=asc)
         url = uri_e + '/v1/dj/program/byradio'
         payload = self.eapi_encrypt(b'/api/v1/dj/program/byradio', data)
         return self.request('POST', url, {'params': payload})
 
+    def list_toplist(self):
+        url = uri + '/toplist'
+        data = self.request('GET', url)
+        if data['code'] == 200:
+            return data['list']
+        raise CodeShouldBe200(data)
+
     def _create_aes_key(self, size):
         return (''.join([hex(b)[2:] for b in os.urandom(size)]))[0:16]
 
     def _aes_encrypt(self, text, key):
         pad = 16 - len(text) % 16
         text = text + pad * chr(pad)
         encryptor = AES.new(bytes(key, 'utf-8'), 2, b'0102030405060708')
```

### Comparing `fuo_netease-1.0.2/fuo_netease/assets/icon.svg` & `fuo_netease-1.0.3/fuo_netease/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/cloud_helpers/__init__.py` & `fuo_netease-1.0.3/fuo_netease/cloud_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/cloud_helpers/cloud_api.py` & `fuo_netease-1.0.3/fuo_netease/cloud_helpers/cloud_api.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/cloud_helpers/security.py` & `fuo_netease-1.0.3/fuo_netease/cloud_helpers/security.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/downloader.py` & `fuo_netease-1.0.3/fuo_netease/downloader.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/login_controller.py` & `fuo_netease-1.0.3/fuo_netease/login_controller.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/models.py` & `fuo_netease-1.0.3/fuo_netease/models.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/page_fav.py` & `fuo_netease-1.0.3/fuo_netease/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease/provider.py` & `fuo_netease-1.0.3/fuo_netease/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         if songs_data is None:
             logger.error('data should not be None')
             return None
         return [_deserialize(song_data, V2SongSchema)
                 for song_data in songs_data]
 
     def rec_list_daily_playlists(self):
+        # If no user login, the API return code=301.
         if not self.has_current_user():
             return []
 
         playlists_data = self.api.get_recommend_playlists()
         rec_playlists = []
         for playlist_data in playlists_data:
             # FIXME: GUI模式下无法显示歌单描述
@@ -119,14 +120,20 @@
         return rec_playlists
 
     def rec_list_daily_songs(self):
         songs_data = self.api.get_recommend_songs()
         return [_deserialize(song_data, V2SongSchemaForV3)
                 for song_data in songs_data]
 
+    def toplist_list(self):
+        return [_deserialize(each, V2PlaylistSchema) for each in self.api.list_toplist()]
+
+    def toplist_get(self, identifier):
+        return self.playlist_get(identifier)
+
     def song_get(self, identifier):
         data = self.api.song_detail(int(identifier))
         return _deserialize(data, V2SongSchema)
 
     def song_list_similar(self, song):
         songs = self.api.get_similar_song(song.identifier)
         return [_deserialize(song, V2SongSchema) for song in songs]
@@ -243,40 +250,42 @@
             # Trick: try to find the highest quality url
             # When the song is only for vip/paid user and current user is non-vip,
             # the highest bitrate is 0, which means this song is unavailable
             # for current user.
             songs_url_data = self.api.weapi_songs_url([song_id], 999000)
             assert songs_url_data, 'length should not be 0'
             song_url_data = songs_url_data[0]
-            highest_bitrate = song_url_data['br']
-            # When the bitrate is large than 320000, the quality is treated as
-            # lossless. We set the threshold to 400000 here.
-            # Note(cosven): From manual testing, the bitrate of lossless media
-            # can be 740kbps, 883kbps, 1411kbps, 1777kbps.
-            if song_url_data['url'] and 'privatecloud' in song_url_data['url']:
-                # 对于云盘歌曲, netease会抛弃官方音乐地址, 只会返回自己上传的音乐链接
-                # bitrate不由用户提供 由官方估算， 且不再是标准的320, 192, 128
-                q_media_mapping[Quality.Audio.shq] = (highest_bitrate,
-                                                      song_url_data['url'],
-                                                      song_url_data['type'])
+            if song_url_data['freeTrialInfo'] is not None:
+                logger.debug(f'song:{song_id} only has media segment for trial')
             else:
-                if highest_bitrate > 400000:
+                highest_bitrate = song_url_data['br']
+                # When the bitrate is large than 320000, the quality is treated as
+                # lossless. We set the threshold to 400000 here.
+                # Note(cosven): From manual testing, the bitrate of lossless media
+                # can be 740kbps, 883kbps, 1411kbps, 1777kbps.
+                if song_url_data['url'] and 'privatecloud' in song_url_data['url']:
+                    # 对于云盘歌曲, netease会抛弃官方音乐地址, 只会返回自己上传的音乐链接
+                    # bitrate不由用户提供 由官方估算， 且不再是标准的320, 192, 128
                     q_media_mapping[Quality.Audio.shq] = (highest_bitrate,
                                                           song_url_data['url'],
                                                           song_url_data['type'])
-
-                for key, quality in key_quality_mapping.items():
-                    # Ensure the quality info exists.
-                    if key in song_data and song_data[key] is not None:
-                        # This resource is invalid for current user since the expected
-                        # bitrate is large than the highest_bitrate
-                        if (song_data[key]['br'] - highest_bitrate) > 10000:
-                            continue
-                        q_media_mapping[quality] = (song_data[key]['br'], None, None)
-
+                else:
+                    if highest_bitrate > 400000:
+                        q_media_mapping[Quality.Audio.shq] = (highest_bitrate,
+                                                              song_url_data['url'],
+                                                              song_url_data['type'])
+
+                    for key, quality in key_quality_mapping.items():
+                        # Ensure the quality info exists.
+                        if key in song_data and song_data[key] is not None:
+                            # This resource is invalid for current user since the
+                            # expected bitrate is large than the highest_bitrate
+                            if (song_data[key]['br'] - highest_bitrate) > 10000:
+                                continue
+                            q_media_mapping[quality] = (song_data[key]['br'], None, None)
         ttl = 60 * 20
         song.cache_set('q_media_mapping', q_media_mapping, ttl)
         return q_media_mapping
 
     def song_get_web_url(self, song):
         return f'https://music.163.com/#/song?id={song.identifier}'
```

### Comparing `fuo_netease-1.0.2/fuo_netease/provider_ui.py` & `fuo_netease-1.0.3/fuo_netease/provider_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         self._user = user
         LoginController.save(user)
         left_panel = self._app.ui.left_panel
         left_panel.playlists_con.show()
         left_panel.playlists_con.create_btn.show()
         left_panel.my_music_con.show()
 
-        mymusic_fm_item = self._app.mymusic_uimgr.create_item('📻 私人 FM')
+        mymusic_fm_item = self._app.mymusic_uimgr.create_item('私人 FM')
         mymusic_fm_item.clicked.connect(self._activate_fm)
-        mymusic_cloud_item = self._app.mymusic_uimgr.create_item('☁ 云盘歌曲')
+        mymusic_cloud_item = self._app.mymusic_uimgr.create_item('云盘歌曲')
         mymusic_cloud_item.clicked.connect(
             lambda: self._app.browser.goto(page='/providers/netease/fav'),
             weak=False)
 
         self._app.mymusic_uimgr.clear()
         self._app.mymusic_uimgr.add_item(mymusic_fm_item)
         self._app.mymusic_uimgr.add_item(mymusic_cloud_item)
```

### Comparing `fuo_netease-1.0.2/fuo_netease/schemas.py` & `fuo_netease-1.0.3/fuo_netease/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from datetime import datetime
 
 from marshmallow import Schema, post_load, fields, EXCLUDE
 
 from feeluown.library import (
     SongModel, BriefAlbumModel, BriefArtistModel, ModelState, BriefSongModel,
     VideoModel, AlbumModel, ArtistModel, PlaylistModel, BriefUserModel,
-    SimpleSearchResult, MediaFlags,
+    SimpleSearchResult, MediaFlags, AlbumType
 )
 from feeluown.media import Quality, MediaType, Media
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSchema(Schema):
@@ -51,14 +51,26 @@
         for field, value in cache_data.items():
             model.cache_set(field, value)
     else:
         model = model_cls(**data)
     return model
 
 
+def get_media_flags(fee: int):
+    # 0: 免费或无版权
+    # 1: VIP 歌曲
+    # 4: 购买专辑
+    # 8: 非会员可免费播放低音质，会员可播放高音质及下载
+    if fee == 1:
+        return MediaFlags.vip
+    elif fee == 4:
+        return MediaFlags.pay
+    return None
+
+
 class V2MvSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     title = fields.Str(required=True, data_key='name')
     cover = fields.Str(required=True)
     brs = fields.Dict(required=True)
     artists = fields.List(fields.Nested('V2BriefArtistSchema'))
     duration = fields.Int(required=True)
@@ -130,40 +142,41 @@
 
     @post_load
     def create_v2_model(self, data, **kwargs):
         # https://github.com/feeluown/FeelUOwn/issues/499
         if data['title'] is None:
             data['title'] = Unknown
 
-        # 0: 免费或无版权
-        # 1: VIP 歌曲
-        # 4: 购买专辑
-        # 8: 非会员可免费播放低音质，会员可播放高音质及下载
         fee = data.pop('fee')
-        if fee == 1:
-            data['media_flags'] = MediaFlags.vip
-        elif fee == 4:
-            data['media_flags'] = MediaFlags.pay
+        flags = get_media_flags(fee)
+        if flags is not None:
+            data['media_flags'] = flags
         return create_model(SongModel, data, ['mv_id', 'comment_thread_id'])
 
 
 class V2SongSchemaForV3(Schema):
     identifier = fields.Int(required=True, data_key='id')
     title = fields.Str(required=True, data_key='name')
     duration = fields.Float(required=True, data_key='dt')
     album = fields.Nested('V2BriefAlbumSchema', data_key='al', allow_none=True)
     artists = fields.List(fields.Nested('V2BriefArtistSchema'),
                           data_key='ar',
                           allow_none=True)
 
     mv_id = fields.Int(required=True, data_key='mv')
+    fee = fields.Int(required=True)
 
     @post_load
     def create_v2_model(self, data, **kwargs):
         data['artists'] = data['artists'] or []
+
+        fee = data.pop('fee')
+        flags = get_media_flags(fee)
+        if flags is not None:
+            data['media_flags'] = flags
         return create_model(SongModel, data, ['mv_id'])
 
 
 class V2AlbumSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     name = fields.Str(required=True)
     cover = fields.Str(data_key='picUrl', allow_none=True)
@@ -172,22 +185,37 @@
     songs = fields.List(fields.Nested('V2SongSchema'), allow_none=True)
     song_count = fields.Int(data_key='size')
 
     # Description is fetched seperatelly by `album_desc` API.
     description = fields.Str(missing='')
     released = fields.Int(data_key='publishTime', missing=0)
 
+    # Single/专辑/"EP/Single"/合集/专辑/精选集
+    type = fields.Str(required=True, data_key='type')
+
     @post_load
     def create_v2_model(self, data, **kwargs):
         released = data['released']
         if released:
             released_date = datetime.fromtimestamp(released / 1000)
             released_str = released_date.strftime('%Y-%m-%d')
             data['released'] = released_str
         data['songs'] = data['songs'] or []
+        type_str = data.pop('type')
+        if type_str == 'Single':
+            type_ = AlbumType.single
+        elif type_str == 'EP/Single':
+            type_ = AlbumType.ep
+        elif type_str == '合集':
+            type_ = AlbumType.compilation
+        elif type_str == '精选集':
+            type_ = AlbumType.retrospective
+        else:
+            type_ = AlbumType.standard
+        data['type_'] = type_
         return AlbumModel(**data)
 
 
 class V2ArtistSchema(Schema):
     identifier = fields.Int(required=True, data_key='id')
     name = fields.Str()
     pic_url = fields.Str(data_key='picUrl', allow_none=True)
```

### Comparing `fuo_netease-1.0.2/fuo_netease/ui.py` & `fuo_netease-1.0.3/fuo_netease/ui.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/fuo_netease.egg-info/PKG-INFO` & `fuo_netease-1.0.3/fuo_netease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-netease
-Version: 1.0.2
+Version: 1.0.3
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-1.0.2/fuo_netease.egg-info/SOURCES.txt` & `fuo_netease-1.0.3/fuo_netease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.2/setup.py` & `fuo_netease-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='fuo_netease',
-    version='1.0.2',
+    version='1.0.3',
     description='feeluown netease plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=find_packages(exclude=('tests*',)),
     package_data={
         '': ['assets/*.svg',
              ]
```

