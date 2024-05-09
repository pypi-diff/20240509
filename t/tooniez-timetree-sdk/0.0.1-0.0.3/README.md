# Comparing `tmp/tooniez_timetree_sdk-0.0.1.tar.gz` & `tmp/tooniez-timetree-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooniez_timetree_sdk-0.0.1.tar", last modified: Wed May  8 11:23:06 2024, max compression
+gzip compressed data, was "tooniez-timetree-sdk-0.0.3.tar", last modified: Thu May  9 06:43:32 2024, max compression
```

## Comparing `tooniez_timetree_sdk-0.0.1.tar` & `tooniez-timetree-sdk-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 luucrew    (501) staff       (20)        0 2024-05-08 11:23:06.243377 tooniez_timetree_sdk-0.0.1/
--rw-r--r--   0 luucrew    (501) staff       (20)     4636 2024-05-08 11:23:06.243182 tooniez_timetree_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 luucrew    (501) staff       (20)     4202 2024-05-07 10:51:55.000000 tooniez_timetree_sdk-0.0.1/README.md
--rw-r--r--   0 luucrew    (501) staff       (20)       38 2024-05-08 11:23:06.243422 tooniez_timetree_sdk-0.0.1/setup.cfg
--rw-r--r--   0 luucrew    (501) staff       (20)      820 2024-05-08 11:21:04.000000 tooniez_timetree_sdk-0.0.1/setup.py
-drwxr-xr-x   0 luucrew    (501) staff       (20)        0 2024-05-08 11:23:06.239616 tooniez_timetree_sdk-0.0.1/timetree_sdk/
--rw-r--r--   0 luucrew    (501) staff       (20)       38 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/__init__.py
--rw-r--r--   0 luucrew    (501) staff       (20)     6438 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/api.py
-drwxr-xr-x   0 luucrew    (501) staff       (20)        0 2024-05-08 11:23:06.241474 tooniez_timetree_sdk-0.0.1/timetree_sdk/models/
--rw-r--r--   0 luucrew    (501) staff       (20)      469 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/models/__init__.py
--rw-r--r--   0 luucrew    (501) staff       (20)     1087 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/models/base.py
--rw-r--r--   0 luucrew    (501) staff       (20)     2943 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/models/events.py
--rw-r--r--   0 luucrew    (501) staff       (20)     8542 2023-07-24 21:47:09.000000 tooniez_timetree_sdk-0.0.1/timetree_sdk/models/responses.py
-drwxr-xr-x   0 luucrew    (501) staff       (20)        0 2024-05-08 11:23:06.242923 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/
--rw-r--r--   0 luucrew    (501) staff       (20)     4636 2024-05-08 11:23:06.000000 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/PKG-INFO
--rw-r--r--   0 luucrew    (501) staff       (20)      405 2024-05-08 11:23:06.000000 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 luucrew    (501) staff       (20)        1 2024-05-08 11:23:06.000000 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 luucrew    (501) staff       (20)        9 2024-05-08 11:23:06.000000 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/requires.txt
--rw-r--r--   0 luucrew    (501) staff       (20)       34 2024-05-08 11:23:06.000000 tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/timetree_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-05-09 06:43:27.000000 tooniez-timetree-sdk-0.0.3/timetree_sdk/models/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:43:32.586269 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 06:43:32.000000 tooniez-timetree-sdk-0.0.3/tooniez_timetree_sdk.egg-info/top_level.txt
```

### Comparing `tooniez_timetree_sdk-0.0.1/PKG-INFO` & `tooniez-timetree-sdk-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: tooniez-timetree-sdk
-Version: 0.0.1
-Summary: TimeTree SDK
-Home-page: https://github.com/tooniez/timetree-sdk
-Author: tooniez
-Author-email: tooni22@proton.me
-License: MIT
-Keywords: timetree api sdk
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-
 # TimeTree SDK for Python
 
 [TimeTree API](https://developers.timetreeapp.com/en/docs/api) SDK for Python.
 
 # Installing
 
 ```
-$ pip install timetree-sdk
+$ pip install tooniez-timetree-sdk
 ```
 
 # Usage
 
 ```python
 from timetree_sdk import TimeTreeApi
```

### Comparing `tooniez_timetree_sdk-0.0.1/setup.py` & `tooniez-timetree-sdk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tooniez-timetree-sdk',
     packages=['timetree_sdk', 'timetree_sdk/models/'],
-    version='0.0.1',
+    version='0.0.3',
     license='MIT',
     install_requires=['requests'],
     author='tooniez',
     author_email='tooni22@proton.me',
     url='https://github.com/tooniez/timetree-sdk',
     description='TimeTree SDK',
     long_description=long_description,
```

### Comparing `tooniez_timetree_sdk-0.0.1/timetree_sdk/api.py` & `tooniez-timetree-sdk-0.0.3/timetree_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tooniez_timetree_sdk-0.0.1/timetree_sdk/models/base.py` & `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `tooniez_timetree_sdk-0.0.1/timetree_sdk/models/events.py` & `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/events.py`

 * *Files identical despite different names*

### Comparing `tooniez_timetree_sdk-0.0.1/timetree_sdk/models/responses.py` & `tooniez-timetree-sdk-0.0.3/timetree_sdk/models/responses.py`

 * *Files identical despite different names*

### Comparing `tooniez_timetree_sdk-0.0.1/tooniez_timetree_sdk.egg-info/PKG-INFO` & `tooniez-timetree-sdk-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,202 +1,202 @@
 Metadata-Version: 2.1
 Name: tooniez-timetree-sdk
-Version: 0.0.1
+Version: 0.0.3
 Summary: TimeTree SDK
 Home-page: https://github.com/tooniez/timetree-sdk
 Author: tooniez
 Author-email: tooni22@proton.me
 License: MIT
-Keywords: timetree api sdk
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-
-# TimeTree SDK for Python
-
-[TimeTree API](https://developers.timetreeapp.com/en/docs/api) SDK for Python.
-
-# Installing
-
-```
-$ pip install timetree-sdk
-```
-
-# Usage
-
-```python
-from timetree_sdk import TimeTreeApi
-
-api = TimeTreeApi('API_ACCESS_TOKEN')
-calendar = api.get_calendar('CALENDAR_ID')
-print(calendar.data.attributes.name) # calendar name
-```
-
-# API
-
-## Oauth
-
-### get oauth authorize url
-
-```python
-oauth_authorize_url = TimeTreeApi.get_oauth_authorize_url('CLIENT_ID', 'REDIRECT_URI', 'RESPONSE_TYPE', 'STATE')
-```
-
-## User
-
-### get current user
-
-```python
-user = api.get_current_user()
-print(user.data.attributes.name) # user name
-```
-
-## Calendar
-
-### get calendars
-
-```python
-calendars = api.get_calendars()
-print(calendars.data[0].attributes.name) # first calendar name
-```
-
-### get calendar
-
-```python
-calendar = api.get_calendar('CALENDAR_ID')
-print(calendar.data.attributes.name) # calendar name
-```
-
-### get calendar labels
-
-```python
-labels = api.get_calendar_labels('CALENDAR_ID')
-print(labels.data[0].attributes.name) # first calendar's label name
-```
-
-### get calendar members
-
-```python
-members = api.get_calendar_members('CALENDAR_ID')
-print(members.data[0].attributes.name) # first calendar's member name
-```
-
-## Event
-
-### get event
-
-```python
-event = api.get_event('CALENDAR_ID', 'EVENT_ID')
-print(event.data.attributes.title) # event title
-```
-
-### get upcoming events
-
-```python
-events = api.get_upcoming_events('CALENDAR_ID', 'Asia/Tokyo', 7)
-print(events.data[0].attributes.title) # most recent event title in 7 days
-```
-
-### create event
-
-```python
-event = Event(
-    data=EventData(
-        attributes=EventAttributes(
-            title='Title',
-            category='schedule',
-            all_day=False,
-            start_at='2020-04-04T11:00:00.000Z',
-            end_at='2020-04-04T13:00:00.000Z',
-            description='Description',
-            location='Location',
-            start_timezone='Japan',
-            end_timezone='Japan'
-        ),
-        relationships=EventRelationships(
-            label=EventRelationshipsLabel(
-                data=EventRelationshipsLabelData(
-                    id='LABEL_ID',
-                    type='label'
+Description: # TimeTree SDK for Python
+        
+        [TimeTree API](https://developers.timetreeapp.com/en/docs/api) SDK for Python.
+        
+        # Installing
+        
+        ```
+        $ pip install tooniez-timetree-sdk
+        ```
+        
+        # Usage
+        
+        ```python
+        from timetree_sdk import TimeTreeApi
+        
+        api = TimeTreeApi('API_ACCESS_TOKEN')
+        calendar = api.get_calendar('CALENDAR_ID')
+        print(calendar.data.attributes.name) # calendar name
+        ```
+        
+        # API
+        
+        ## Oauth
+        
+        ### get oauth authorize url
+        
+        ```python
+        oauth_authorize_url = TimeTreeApi.get_oauth_authorize_url('CLIENT_ID', 'REDIRECT_URI', 'RESPONSE_TYPE', 'STATE')
+        ```
+        
+        ## User
+        
+        ### get current user
+        
+        ```python
+        user = api.get_current_user()
+        print(user.data.attributes.name) # user name
+        ```
+        
+        ## Calendar
+        
+        ### get calendars
+        
+        ```python
+        calendars = api.get_calendars()
+        print(calendars.data[0].attributes.name) # first calendar name
+        ```
+        
+        ### get calendar
+        
+        ```python
+        calendar = api.get_calendar('CALENDAR_ID')
+        print(calendar.data.attributes.name) # calendar name
+        ```
+        
+        ### get calendar labels
+        
+        ```python
+        labels = api.get_calendar_labels('CALENDAR_ID')
+        print(labels.data[0].attributes.name) # first calendar's label name
+        ```
+        
+        ### get calendar members
+        
+        ```python
+        members = api.get_calendar_members('CALENDAR_ID')
+        print(members.data[0].attributes.name) # first calendar's member name
+        ```
+        
+        ## Event
+        
+        ### get event
+        
+        ```python
+        event = api.get_event('CALENDAR_ID', 'EVENT_ID')
+        print(event.data.attributes.title) # event title
+        ```
+        
+        ### get upcoming events
+        
+        ```python
+        events = api.get_upcoming_events('CALENDAR_ID', 'Asia/Tokyo', 7)
+        print(events.data[0].attributes.title) # most recent event title in 7 days
+        ```
+        
+        ### create event
+        
+        ```python
+        event = Event(
+            data=EventData(
+                attributes=EventAttributes(
+                    title='Title',
+                    category='schedule',
+                    all_day=False,
+                    start_at='2020-04-04T11:00:00.000Z',
+                    end_at='2020-04-04T13:00:00.000Z',
+                    description='Description',
+                    location='Location',
+                    start_timezone='Japan',
+                    end_timezone='Japan'
+                ),
+                relationships=EventRelationships(
+                    label=EventRelationshipsLabel(
+                        data=EventRelationshipsLabelData(
+                            id='LABEL_ID',
+                            type='label'
+                        )
+                    ),
+                    attendees=EventRelationshipsAttendees(
+                        data=[EventRelationshipsAttendeesData(
+                            id='USER_ID',
+                            type='user'
+                        )]
+                    )
                 )
-            ),
-            attendees=EventRelationshipsAttendees(
-                data=[EventRelationshipsAttendeesData(
-                    id='USER_ID',
-                    type='user'
-                )]
             )
         )
-    )
-)
-response = api.create_event('CALENDAR_ID', event)
-print(response.data.attributes.title) # Title
-```
-
-### update event
-
-```python
-event = Event(
-    data=EventData(
-        attributes=EventAttributes(
-            title='Updated Title',
-            category='schedule',
-            all_day=False,
-            start_at='2020-04-04T11:30:00.000Z',
-            end_at='2020-04-04T13:30:00.000Z',
-            description='Description',
-            location='Location',
-            start_timezone='Japan',
-            end_timezone='Japan'
-        ),
-        relationships=EventRelationships(
-            label=EventRelationshipsLabel(
-                data=EventRelationshipsLabelData(
-                    id='LABEL_ID',
-                    type='label'
+        response = api.create_event('CALENDAR_ID', event)
+        print(response.data.attributes.title) # Title
+        ```
+        
+        ### update event
+        
+        ```python
+        event = Event(
+            data=EventData(
+                attributes=EventAttributes(
+                    title='Updated Title',
+                    category='schedule',
+                    all_day=False,
+                    start_at='2020-04-04T11:30:00.000Z',
+                    end_at='2020-04-04T13:30:00.000Z',
+                    description='Description',
+                    location='Location',
+                    start_timezone='Japan',
+                    end_timezone='Japan'
+                ),
+                relationships=EventRelationships(
+                    label=EventRelationshipsLabel(
+                        data=EventRelationshipsLabelData(
+                            id='LABEL_ID',
+                            type='label'
+                        )
+                    ),
+                    attendees=EventRelationshipsAttendees(
+                        data=[EventRelationshipsAttendeesData(
+                            id='USER_ID',
+                            type='user'
+                        )]
+                    )
                 )
-            ),
-            attendees=EventRelationshipsAttendees(
-                data=[EventRelationshipsAttendeesData(
-                    id='USER_ID',
-                    type='user'
-                )]
             )
         )
-    )
-)
-response = api.create_event('CALENDAR_ID', 'EVENT_ID', event)
-print(response.data.attributes.title) # Updated Title
-```
-
-### delete event
-
-```python
-status_code = api.delete_event('CALENDAR_ID', 'EVENT_ID')
-print(status_code) # 204 on success
-```
-
-## Event Comment
-
-### create comment to event
-
-```python
-comment = EventComment(
-    data=EventCommentData(
-        attributes=EventCommentAttributes(
-            content='Hello, world'
+        response = api.create_event('CALENDAR_ID', 'EVENT_ID', event)
+        print(response.data.attributes.title) # Updated Title
+        ```
+        
+        ### delete event
+        
+        ```python
+        status_code = api.delete_event('CALENDAR_ID', 'EVENT_ID')
+        print(status_code) # 204 on success
+        ```
+        
+        ## Event Comment
+        
+        ### create comment to event
+        
+        ```python
+        comment = EventComment(
+            data=EventCommentData(
+                attributes=EventCommentAttributes(
+                    content='Hello, world'
+                )
+            )
         )
-    )
-)
-event_comment = api.create_event_comment('CALENDAR_ID', 'EVENT_ID', comment)
-print(event_comment.data.attributes.content) # Hello, world
-```
-
-# Documentation
-
-Official API documentation
-
-English: https://developers.timetreeapp.com/en/docs/api
-
-Japanese: https://developers.timetreeapp.com/ja/docs/api
+        event_comment = api.create_event_comment('CALENDAR_ID', 'EVENT_ID', comment)
+        print(event_comment.data.attributes.content) # Hello, world
+        ```
+        
+        # Documentation
+        
+        Official API documentation
+        
+        English: https://developers.timetreeapp.com/en/docs/api
+        
+        Japanese: https://developers.timetreeapp.com/ja/docs/api
+        
+Keywords: timetree api sdk
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
```

