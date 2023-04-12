# Comparing `tmp/i2a_chat_api_client-1.2.3.tar.gz` & `tmp/i2a_chat_api_client-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2a_chat_api_client-1.2.3.tar", last modified: Fri Mar 24 13:45:54 2023, max compression
+gzip compressed data, was "i2a_chat_api_client-1.2.5.tar", last modified: Wed Apr 12 09:29:01 2023, max compression
```

## Comparing `i2a_chat_api_client-1.2.3.tar` & `i2a_chat_api_client-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-03-24 13:45:54.217540 i2a_chat_api_client-1.2.3/
--rw-rw-r--   0 adn       (1000) adn       (1000)     1061 2023-03-23 14:43:48.000000 i2a_chat_api_client-1.2.3/LICENSE.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-03-24 13:45:54.217540 i2a_chat_api_client-1.2.3/PKG-INFO
--rw-rw-r--   0 adn       (1000) adn       (1000)      203 2023-03-23 14:43:48.000000 i2a_chat_api_client-1.2.3/README.md
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-03-24 13:45:54.217540 i2a_chat_api_client-1.2.3/i2a_chat_api_client/
--rw-rw-r--   0 adn       (1000) adn       (1000)       49 2023-03-23 14:43:48.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client/__init__.py
--rw-rw-r--   0 adn       (1000) adn       (1000)    11710 2023-03-24 13:45:36.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client/client.py
--rw-rw-r--   0 adn       (1000) adn       (1000)      480 2023-03-23 14:43:48.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client/exceptions.py
-drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-03-24 13:45:54.217540 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/
--rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-03-24 13:45:54.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 adn       (1000) adn       (1000)      340 2023-03-24 13:45:54.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)        1 2023-03-24 13:45:54.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       17 2023-03-24 13:45:54.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/requires.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       20 2023-03-24 13:45:54.000000 i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/top_level.txt
--rw-rw-r--   0 adn       (1000) adn       (1000)       38 2023-03-24 13:45:54.217540 i2a_chat_api_client-1.2.3/setup.cfg
--rw-rw-r--   0 adn       (1000) adn       (1000)      786 2023-03-24 13:45:36.000000 i2a_chat_api_client-1.2.3/setup.py
+drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 09:29:01.197617 i2a_chat_api_client-1.2.5/
+-rw-rw-r--   0 adn       (1000) adn       (1000)     1061 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.2.5/LICENSE.txt
+-rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-04-12 09:29:01.197617 i2a_chat_api_client-1.2.5/PKG-INFO
+-rw-rw-r--   0 adn       (1000) adn       (1000)      203 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.2.5/README.md
+drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 09:29:01.197617 i2a_chat_api_client-1.2.5/i2a_chat_api_client/
+-rw-rw-r--   0 adn       (1000) adn       (1000)       49 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client/__init__.py
+-rw-rw-r--   0 adn       (1000) adn       (1000)    11923 2023-04-12 09:22:10.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client/client.py
+-rw-rw-r--   0 adn       (1000) adn       (1000)      480 2023-04-12 09:16:02.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client/exceptions.py
+drwxrwxr-x   0 adn       (1000) adn       (1000)        0 2023-04-12 09:29:01.197617 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/
+-rw-rw-r--   0 adn       (1000) adn       (1000)      579 2023-04-12 09:29:01.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 adn       (1000) adn       (1000)      340 2023-04-12 09:29:01.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 adn       (1000) adn       (1000)        1 2023-04-12 09:29:01.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 adn       (1000) adn       (1000)       17 2023-04-12 09:29:01.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/requires.txt
+-rw-rw-r--   0 adn       (1000) adn       (1000)       20 2023-04-12 09:29:01.000000 i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 adn       (1000) adn       (1000)       38 2023-04-12 09:29:01.197617 i2a_chat_api_client-1.2.5/setup.cfg
+-rw-rw-r--   0 adn       (1000) adn       (1000)      786 2023-04-12 09:28:42.000000 i2a_chat_api_client-1.2.5/setup.py
```

### Comparing `i2a_chat_api_client-1.2.3/LICENSE.txt` & `i2a_chat_api_client-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2a_chat_api_client-1.2.3/PKG-INFO` & `i2a_chat_api_client-1.2.5/i2a_chat_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: i2a_chat_api_client
-Version: 1.2.3
+Name: i2a-chat-api-client
+Version: 1.2.5
 Summary: Sdk for i2a chat api
 Download-URL: https://pypi.org/project/i2a_chat_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Chat Api Client,I2A Chat Api,I2A Chat,Python 3,I2A Chat Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_chat_api_client-1.2.3/i2a_chat_api_client/client.py` & `i2a_chat_api_client-1.2.5/i2a_chat_api_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,33 +258,37 @@
         elif response.status_code == 404:
             raise I2AChatApiClientNotFoundError(data=response.json())
         elif response.status_code == 400:
             raise I2AChatApiClientValidationError(data=response.json())
         else:
             raise Exception(f'Send system message failed. {self._status_code_message(response)}')
 
-    def set_message_is_active(
+    def get_chat_room_messages(
         self,
-        message_timestamp_identifier: int,
-        is_active: bool
+        chat_room_identifier: str,
+        message_timestamp_from: int = None,
+        limit: int = None
     ):
         """
-            Set flag is_active on chat message
-            :param message_timestamp_identifier: int
-            :param is_active: bool
-            :return: response - 200
-        """
-        url = self._get_full_url(f'chat-message/{message_timestamp_identifier}/set-active/')
-        data = {
-            'is_active': is_active
-        }
-        response = requests.post(url, data, headers=self._required_headers())
+        Queuing system message to be saved and send on websocket in provided chat room
+        :param chat_room_identifier: str, None
+        :param message_timestamp_from: str, None
+        :param limit: int
+        :return: response - [messages]
+       """
+        url = self._get_full_url(f'/chat-room/{chat_room_identifier}/messages/')
+        params = {}
+        if message_timestamp_from:
+            params['timestamp_from'] = message_timestamp_from
+        if limit:
+            params['limit'] = limit
+        response = requests.get(url, headers=self._required_headers(), params=params)
         if response.status_code == 200:
             return response
         elif response.status_code == 401:
             raise I2AChatApiClientUnauthorizedException(data=response.json())
         elif response.status_code == 404:
             raise I2AChatApiClientNotFoundError(data=response.json())
         elif response.status_code == 400:
             raise I2AChatApiClientValidationError(data=response.json())
         else:
-            raise Exception(f'Set message is active flag failed. {self._status_code_message(response)}')
+            raise Exception(f'Send system message failed. {self._status_code_message(response)}')
```

### Comparing `i2a_chat_api_client-1.2.3/i2a_chat_api_client.egg-info/PKG-INFO` & `i2a_chat_api_client-1.2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: i2a-chat-api-client
-Version: 1.2.3
+Name: i2a_chat_api_client
+Version: 1.2.5
 Summary: Sdk for i2a chat api
 Download-URL: https://pypi.org/project/i2a_chat_api_client/
 Author: i2a Solutions Inc.
 Author-email: msyta@i2asolutions.com
 License: MIT
 Keywords: I2A Chat Api Client,I2A Chat Api,I2A Chat,Python 3,I2A Chat Api SDK
 Description-Content-Type: text/markdown
```

### Comparing `i2a_chat_api_client-1.2.3/setup.py` & `i2a_chat_api_client-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='i2a_chat_api_client',
-    version='1.2.3',
+    version='1.2.5',
     description='Sdk for i2a chat api',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='i2a Solutions Inc.',
     author_email='msyta@i2asolutions.com',
```

