# Comparing `tmp/cgpt-1.1.25.tar.gz` & `tmp/cgpt-1.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpt-1.1.25.tar", last modified: Wed Mar 29 16:46:04 2023, max compression
+gzip compressed data, was "cgpt-1.1.26.tar", last modified: Wed Apr 12 19:02:35 2023, max compression
```

## Comparing `cgpt-1.1.25.tar` & `cgpt-1.1.26.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.1.25/LICENSE
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.1.25/MANIFEST.in
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-03-29 16:46:04.444018 cgpt-1.1.25/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1597 2023-03-29 16:43:12.000000 cgpt-1.1.25/README.md
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/app/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.1.25/app/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2455 2023-03-28 13:21:18.000000 cgpt-1.1.25/app/base.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/app/client/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-22 11:27:42.000000 cgpt-1.1.25/app/client/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1310 2023-03-28 13:22:25.000000 cgpt-1.1.25/app/client/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      510 2023-03-28 07:27:41.000000 cgpt-1.1.25/app/file_service.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      436 2023-03-26 11:39:43.000000 cgpt-1.1.25/app/main.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1370 2023-03-28 13:25:41.000000 cgpt-1.1.25/app/plugin.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/app/server/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-22 11:27:23.000000 cgpt-1.1.25/app/server/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1194 2023-03-29 16:36:34.000000 cgpt-1.1.25/app/server/main.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/app/utils/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-22 12:01:26.000000 cgpt-1.1.25/app/utils/__init__.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2152 2023-03-29 16:23:41.000000 cgpt-1.1.25/app/utils/constant.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      137 2023-03-28 13:22:44.000000 cgpt-1.1.25/app/utils/verify_env.py
-drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:46:04.444018 cgpt-1.1.25/cgpt.egg-info/
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/PKG-INFO
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      442 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       34 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/entry_points.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       51 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/requires.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-03-29 16:46:04.000000 cgpt-1.1.25/cgpt.egg-info/top_level.txt
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1068 2023-03-28 11:42:09.000000 cgpt-1.1.25/cgpt.py
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-03-29 16:46:04.444018 cgpt-1.1.25/setup.cfg
--rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1144 2023-03-28 11:28:01.000000 cgpt-1.1.25/setup.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1065 2023-03-17 13:19:22.000000 cgpt-1.1.26/LICENSE
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       15 2023-03-17 13:19:22.000000 cgpt-1.1.26/MANIFEST.in
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-04-12 19:02:35.472151 cgpt-1.1.26/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1684 2023-03-30 12:25:43.000000 cgpt-1.1.26/README.md
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.468151 cgpt-1.1.26/app/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-17 13:58:28.000000 cgpt-1.1.26/app/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2455 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/base.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/client/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/client/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1300 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/client/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      499 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/file_service.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      406 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/main.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1319 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/plugin.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/server/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/server/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1186 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/server/main.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/app/utils/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-03-29 16:59:50.000000 cgpt-1.1.26/app/utils/__init__.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     2137 2023-04-12 12:18:25.000000 cgpt-1.1.26/app/utils/constant.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      137 2023-04-12 12:16:56.000000 cgpt-1.1.26/app/utils/verify_env.py
+drwxrwxr-x   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        0 2023-04-12 19:02:35.472151 cgpt-1.1.26/cgpt.egg-info/
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1603 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      442 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        1 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       34 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       51 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/requires.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)        9 2023-04-12 19:02:35.000000 cgpt-1.1.26/cgpt.egg-info/top_level.txt
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)     1010 2023-04-12 12:16:38.000000 cgpt-1.1.26/cgpt.py
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)       38 2023-04-12 19:02:35.472151 cgpt-1.1.26/setup.cfg
+-rw-rw-r--   0 hairun-pc-yves  (1000) hairun-pc-yves  (1000)      995 2023-04-12 12:16:38.000000 cgpt-1.1.26/setup.py
```

### Comparing `cgpt-1.1.25/LICENSE` & `cgpt-1.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpt-1.1.25/PKG-INFO` & `cgpt-1.1.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.1.25
+Version: 1.1.26
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `cgpt-1.1.25/README.md` & `cgpt-1.1.26/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-![](https://komarev.com/ghpvc/?username=ainayves&color=blueviolet)
+![python](https://img.shields.io/badge/Python-3.7-blue.svg)
+![commit activity](https://img.shields.io/github/commit-activity/m/ainayves/cgpt?color=blue)
+
 
 ## Use openai chat-gpt inside your CLI
 </br>
 
 https://user-images.githubusercontent.com/66997516/228263166-01828e31-3bc1-46b9-ad37-9d44ca117d7f.mp4
 
 </br>
```

### Comparing `cgpt-1.1.25/app/base.py` & `cgpt-1.1.26/app/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import Union , List, Dict
+from typing import Union, List, Dict
 import click, socket
 from app.file_service import file_prompt
 from app.plugin import davinci
-from app.utils.constant import init_conversation , ASSISTANT
+from app.utils.constant import init_conversation, ASSISTANT
 
-class Base_CGPT():
+
+class Base_CGPT:
 
     """
     Baseclass to create a conversational infinite-loop with CGPT module
     """
 
     def __init__(
-            self, exit_key : str, 
-            modify_api_key : str, 
-            input_text : str , 
-            decoration : str, 
-            encode : str,
-            socket_resp : bool,
-            icon_ans :str,
-            socket_instance : socket = None) -> None:
-
+        self,
+        exit_key: str,
+        modify_api_key: str,
+        input_text: str,
+        decoration: str,
+        encode: str,
+        socket_resp: bool,
+        icon_ans: str,
+        socket_instance: socket = None,
+    ) -> None:
         self.exit_key = exit_key
         self.modify_api_key = modify_api_key
         self.input_text = input_text
         self.decoration = decoration
         self.icon_ans = icon_ans
         self.encode = encode
         self.socket_resp = socket_resp
@@ -31,52 +33,57 @@
 
     def _anonym_func(self, *args):
         return args[0]
 
     def _void_func(self) -> None:
         pass
 
-    def _I_O_func(self , socket_resp : bool , previous_conv : List[Dict], client_input : str = None,  socket = None) -> str:
-
-        if socket_resp :
+    def _I_O_func(
+        self,
+        socket_resp: bool,
+        previous_conv: List[Dict],
+        client_input: str = None,
+        socket=None,
+    ) -> str:
+        if socket_resp:
             if client_input is not None:
                 socket.send(client_input.encode(self.encode.lower()))
-            
+
             elif client_input == self.exit_key:
                 return
-            
+
             elif client_input == self.modify_api_key:
                 file_prompt()
                 return
 
             data = socket.recv(1024)
             res = str(data.decode(self.encode.lower()))
         else:
             res = davinci(client_input, previous_conv)
 
         return res
 
     def infinite_loop(self) -> None:
-
-        while True :
-
+        while True:
             self._void_func()
             client = input(self.input_text)
             if client == self.exit_key:
                 break
-            
+
             elif client == self.modify_api_key:
                 file_prompt()
                 break
 
-            resp = self._I_O_func(self.socket_resp, previous_conv=init_conversation, client_input=client, socket=self.socket_instance)
-            init_conversation.append(
-                {"role": ASSISTANT, "content": resp}
+            resp = self._I_O_func(
+                self.socket_resp,
+                previous_conv=init_conversation,
+                client_input=client,
+                socket=self.socket_instance,
             )
+            init_conversation.append({"role": ASSISTANT, "content": resp})
             if resp is None:
                 break
-            
+
             click.echo(self.decoration, color=True)
             click.echo(f"<< {self.icon_ans} >> {resp}")
             click.echo("\n")
             click.echo(self.decoration, color=True)
-
```

### Comparing `cgpt-1.1.25/app/client/main.py` & `cgpt-1.1.26/app/client/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 # -*- coding: utf-8 -*-
 
 import ipaddress
-import socket, click 
+import socket, click
 from app.utils.constant import (
     UTF,
     IA,
     SAY_SOMETHING,
     ENTER_SERVER_IP,
     CONNECTION_ERROR,
     CONNECTION_IMPOSSIBLE,
     DASHED,
     PORT,
-    ADDRESS_NOT_VALID
-)   
+    ADDRESS_NOT_VALID,
+)
 
 from app.utils.verify_env import _check_env_file
 from app.base import Base_CGPT
 
+
 def main():
-    
     adresse_ip = click.prompt(ENTER_SERVER_IP)
 
     try:
-
         ipaddress.IPv4Address(adresse_ip)
-        s = socket.socket(socket.AF_INET,socket.SOCK_STREAM)
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
-
             s.connect((adresse_ip, int(PORT)))
             Base_CGPT._void_func = _check_env_file
 
             cgpt = Base_CGPT(
                 exit_key="q",
                 modify_api_key="m",
                 input_text=SAY_SOMETHING,
                 decoration=DASHED,
                 encode=UTF,
                 icon_ans=IA,
                 socket_resp=True,
-                socket_instance=s
+                socket_instance=s,
             )
 
             cgpt.infinite_loop()
 
-        except OSError as e: 
-
+        except OSError as e:
             if e.errno == 113:
                 click.echo(CONNECTION_IMPOSSIBLE)
             else:
                 click.echo(CONNECTION_ERROR, e)
 
         finally:
-
             s.close()
 
-    except ipaddress.AddressValueError: 
-
+    except ipaddress.AddressValueError:
         click.echo(ADDRESS_NOT_VALID)
 
-if __name__ == '__main__':
-    main()
+
+if __name__ == "__main__":
+    main()
```

### Comparing `cgpt-1.1.25/app/plugin.py` & `cgpt-1.1.26/app/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 # -*- coding: utf-8 -*-
 
 import os, click
-from typing import Union , List, Dict
+from typing import Union, List, Dict
 import openai
 from app.file_service import file_prompt
 from dotenv import load_dotenv
+
 load_dotenv()
 from app.utils.constant import (
     AI_COLON,
     CHOICES,
     STR_OPENAI_API_KEY,
     DAVINCI_MODEL,
     INCORRECT_API_KEY,
     MESSAGE,
     CONTENT,
     OPENAI_REQUEST_TIMEOUT,
     NOT_CONNECTED,
     TOO_MUCH_REQUEST,
-    USER
+    USER,
 )
 
 openai.api_key = os.getenv(STR_OPENAI_API_KEY)
 
-def davinci(what : str, previous_conv :  List[Dict]) -> Union[str, None]:
+
+def davinci(what: str, previous_conv: List[Dict]) -> Union[str, None]:
     try:
-        
         previous_conv.append({"role": USER, "content": what})
         response = openai.ChatCompletion.create(
-        model=DAVINCI_MODEL,
-        messages=previous_conv
+            model=DAVINCI_MODEL, messages=previous_conv
         )
-        
-        res = response[CHOICES][0][MESSAGE][CONTENT].replace(AI_COLON,"")
 
-    except openai.error.AuthenticationError:
+        res = response[CHOICES][0][MESSAGE][CONTENT].replace(AI_COLON, "")
 
+    except openai.error.AuthenticationError:
         modify_apikey = input(INCORRECT_API_KEY)
 
-        if modify_apikey == "m" :
-
+        if modify_apikey == "m":
             file_prompt()
             res = None
-            
-        else:
 
+        else:
             res = None
-            
-    except openai.error.Timeout:
 
+    except openai.error.Timeout:
         click.echo(OPENAI_REQUEST_TIMEOUT)
         res = None
 
     except openai.error.APIConnectionError:
-
         click.echo(NOT_CONNECTED)
         res = None
 
     except openai.error.RateLimitError:
-
         click.echo(TOO_MUCH_REQUEST)
         res = None
 
-    return res
+    return res
```

### Comparing `cgpt-1.1.25/app/server/main.py` & `cgpt-1.1.26/app/server/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # -*- coding: utf-8 -*-
 
 import socket, click
 from _thread import *
 import threading
+
 print_lock = threading.Lock()
 from app.plugin import davinci
-from app.utils.constant import PORT , SERVER_LIVE , UTF , LIVE , DECONNECTED_HOST , init_conversation
+from app.utils.constant import (
+    PORT,
+    SERVER_LIVE,
+    UTF,
+    LIVE,
+    DECONNECTED_HOST,
+    init_conversation,
+)
+
 
 def threaded(c):
-    
     init_conversation_client = init_conversation
     while True:
-        
         try:
             client_data = c.recv(1024).decode()
 
-        
             api_response = davinci(client_data, init_conversation_client)
-            if api_response is not None : 
+            if api_response is not None:
                 c.send(api_response.encode(encoding=UTF))
-            else : 
+            else:
                 continue
-        
+
         except BrokenPipeError:
             continue
 
         except ConnectionResetError:
             click.echo(DECONNECTED_HOST)
 
+
 def main():
     adresse_ip = socket.gethostbyname(socket.gethostname())
     server_socket = socket.create_server((adresse_ip, int(PORT)), reuse_port=False)
     server_socket.listen()
-    click.echo(f"{SERVER_LIVE} {adresse_ip} ..{LIVE}")  
+    click.echo(f"{SERVER_LIVE} {adresse_ip} ..{LIVE}")
     while True:
         client, _ = server_socket.accept()
         threading.Thread(target=threaded, args=(client,), daemon=True).start()
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `cgpt-1.1.25/app/utils/constant.py` & `cgpt-1.1.26/app/utils/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import platform
 
-VERSION= "1.1.25"
+VERSION = "1.1.26"
 
 os_name = platform.system()
 
 if os_name == "Linux" or os_name == "Darwin":
     IA = "🤖"
     HAPPY = "😃"
     RELEIVED = "😌"
@@ -15,17 +15,15 @@
     IA = "IA"
     HAPPY = ""
     RELEIVED = ""
     SAD = ""
     NO_ENTRY = ""
     LIVE = ""
 
-init_conversation = [
-            {"role": "system", "content": "You are a helpful assistant."}
-        ]
+init_conversation = [{"role": "system", "content": "You are a helpful assistant."}]
 
 TEMPERATURE = 0.9
 MAX_TOKENS = 200
 TOP_P = 1.0
 FREQUENCY_P = 0.0
 PRESENCE_P = 0.6
 PORT = 2048
@@ -45,24 +43,25 @@
 SERVER_PATH = "/app/server/main.py"
 CLIENT_PATH = "/app/client/main.py"
 CGPT_NETWORK = "--> Voulez-vous utiliser cgpt en réseaux ?"
 YOU_SERVER = f"---> Êtes vous le serveur {HAPPY} ?"
 OPEN_TERMINAL = f"----> Veuillez ouvrir un autre terminal..{RELEIVED}"
 SERVER_LIVE = "Serveur live sur "
 GET_API_KEY = "Ajoutez votre api key (invisible input) >"
-API_KEY_ADDED = "Votre API KEY a bien été ajouté , veuillez relancer la commande `cgpt tellme` "
+API_KEY_ADDED = (
+    "Votre API KEY a bien été ajouté , veuillez relancer la commande `cgpt tellme` "
+)
 API_KEY_NOT_ADDED = "\n Vous n' avez pas ajouter un API KEY \n"
 SAY_SOMETHING = " Dîtes quelque chose (q : quitter , m : modifier api_key ) > "
 ENTER_SERVER_IP = "Entrez l' adresse IP du serveur "
-CONNECTION_LOST = f"Connexion perdue {SAD}" 
+CONNECTION_LOST = f"Connexion perdue {SAD}"
 CONNECTION_IMPOSSIBLE = f"Connexion impossible {SAD}"
 DASHED = "----------------------------------------------------------"
 DAVINCI_MODEL = "gpt-3.5-turbo"
 DAVINCI_PROMPT = "The following is a conversation with an AI. The AI is helpful, creative, clever, and very friendly.\n\nHuman:"
 INCORRECT_API_KEY = "Votre API KEY est incorrect, tapez `m` pour modifer le key , ou `q` pour quitter > "
 OPENAI_REQUEST_TIMEOUT = "IA endormie"
 NOT_CONNECTED = "Vous êtes déconnecté d' internet .."
 TOO_MUCH_REQUEST = "Trop de requête"
 CONNECTION_ERROR = "Erreur de connexion : "
 ADDRESS_NOT_VALID = f"L' adresse IP n' est pas valide {NO_ENTRY}"
 DECONNECTED_HOST = "Un hôte s' est donnecté"
-
```

### Comparing `cgpt-1.1.25/cgpt.egg-info/PKG-INFO` & `cgpt-1.1.26/cgpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgpt
-Version: 1.1.25
+Version: 1.1.26
 Summary: Use openai chat-gpt on your cli
 Home-page: https://github.com/ainayves/cgpt>
 Author: Aina Yves
 Author-email: randrianaina.yves@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `cgpt-1.1.25/cgpt.py` & `cgpt-1.1.26/cgpt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 # -*- coding: utf-8 -*-
 
-import click , os , subprocess
+import click, os, subprocess
 from app.main import prompt
 from app.file_service import file_prompt
 from app.utils.constant import (
-    SERVER_PATH, 
+    SERVER_PATH,
     CLIENT_PATH,
     CGPT_NETWORK,
     YOU_SERVER,
     OPEN_TERMINAL,
-    VERSION
-    )
+    VERSION,
+)
 
 
 @click.group()
 def cli():
     pass
 
+
 @cli.command()
-@click.option('-n', '--name', type=str, help='Name to greet', default='World')
+@click.option("-n", "--name", type=str, help="Name to greet", default="World")
 def hello(name):
-    click.echo(f'Hello {name}')
+    click.echo(f"Hello {name}")
+
 
 @cli.command()
 def version():
     click.echo(VERSION)
 
+
 @cli.command()
 def tellme():
-    
-    cgpt_path = os.path.abspath(os.path.dirname(__file__))   
+    cgpt_path = os.path.abspath(os.path.dirname(__file__))
     use_in_lan = click.confirm(CGPT_NETWORK)
-    
-    if use_in_lan:
 
+    if use_in_lan:
         endpoint = click.confirm(YOU_SERVER)
 
         if endpoint:
             click.echo(OPEN_TERMINAL)
-            subprocess.run(['python', cgpt_path+SERVER_PATH])
-        
-        else:
-            subprocess.run(['python', cgpt_path+CLIENT_PATH])
-
-    else : 
+            subprocess.run(["python", cgpt_path + SERVER_PATH])
 
-        if not os.path.isfile(".env"): 
+        else:
+            subprocess.run(["python", cgpt_path + CLIENT_PATH])
 
+    else:
+        if not os.path.isfile(".env"):
             file_prompt()
         else:
-
             prompt()
-        
-
-
-        
-
-         
-
```

