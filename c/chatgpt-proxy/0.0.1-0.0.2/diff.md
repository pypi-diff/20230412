# Comparing `tmp/chatgpt-proxy-0.0.1.tar.gz` & `tmp/chatgpt-proxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.0.1.tar", last modified: Tue Apr 11 17:40:15 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.0.2.tar", last modified: Wed Apr 12 06:20:19 2023, max compression
```

## Comparing `chatgpt-proxy-0.0.1.tar` & `chatgpt-proxy-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 17:40:15.534210 chatgpt-proxy-0.0.1/
--rw-rw-rw-   0        0        0    35184 2023-04-11 17:04:38.000000 chatgpt-proxy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      226 2023-04-11 17:40:15.532256 chatgpt-proxy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1711 2023-04-11 17:39:48.000000 chatgpt-proxy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 17:40:15.498076 chatgpt-proxy-0.0.1/chatgpt_proxy/
--rw-rw-rw-   0        0        0        0 2023-04-11 16:51:04.000000 chatgpt-proxy-0.0.1/chatgpt_proxy/__init__.py
--rw-rw-rw-   0        0        0      918 2023-04-11 17:31:04.000000 chatgpt-proxy-0.0.1/chatgpt_proxy/__main__.py
--rw-rw-rw-   0        0        0     6607 2023-04-11 17:29:03.000000 chatgpt-proxy-0.0.1/chatgpt_proxy/proxy.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:40:15.529327 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/
--rw-rw-rw-   0        0        0      226 2023-04-11 17:40:15.000000 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-11 17:40:15.000000 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 17:40:15.000000 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-11 17:40:15.000000 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 17:40:15.000000 chatgpt-proxy-0.0.1/chatgpt_proxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      522 2023-04-11 17:28:11.000000 chatgpt-proxy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 17:40:15.534210 chatgpt-proxy-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 06:20:19.114822 chatgpt-proxy-0.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-04-11 17:04:38.000000 chatgpt-proxy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      226 2023-04-12 06:20:19.068691 chatgpt-proxy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-04-12 06:17:09.000000 chatgpt-proxy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 06:20:19.020011 chatgpt-proxy-0.0.2/chatgpt_proxy/
+-rw-rw-rw-   0        0        0       50 2023-04-12 06:11:58.000000 chatgpt-proxy-0.0.2/chatgpt_proxy/__init__.py
+-rw-rw-rw-   0        0        0      995 2023-04-12 06:13:13.000000 chatgpt-proxy-0.0.2/chatgpt_proxy/__main__.py
+-rw-rw-rw-   0        0        0     5877 2023-04-12 06:17:45.000000 chatgpt-proxy-0.0.2/chatgpt_proxy/proxy.py
+drwxrwxrwx   0        0        0        0 2023-04-12 06:20:19.065761 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/
+-rw-rw-rw-   0        0        0      226 2023-04-12 06:20:18.000000 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-12 06:20:18.000000 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 06:20:18.000000 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-12 06:20:18.000000 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 06:20:18.000000 chatgpt-proxy-0.0.2/chatgpt_proxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      522 2023-04-12 06:20:00.000000 chatgpt-proxy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 06:20:19.115360 chatgpt-proxy-0.0.2/setup.cfg
```

### Comparing `chatgpt-proxy-0.0.1/LICENSE` & `chatgpt-proxy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.0.1/README.md` & `chatgpt-proxy-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # ChatGPT-Proxy
 Python version of OpenAI's ChatGPT web API proxy  
-Python alternative to (ChatGPT-Proxy-V4)[https://github.com/acheong08/ChatGPT-Proxy-V4]  
+Python alternative to [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
 Use cookie `_puid` to bypass Cloudflare browser check  
 
 # Requirements
 - ChatGPT plus account
 - Access to chat.openai.com
 
 # Install
 `pip install chatgpt-proxy`
 
 # Usage
 ## Run as a service
 Set these environment variables:
 - `PUID`: Preset cookie `_puid`
 - `ACCESS_TOKEN`: (Optional) For automatic refresh of `_puid`, obtains from [here](https://chat.openai.com/api/auth/session)
+- `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
+    When set to `True`, any requests without an access_token will be given the above access_token.  
+    Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 
 Run: `python -m chatgpt_proxy`
 
 ## Integrate into your FastAPI app
 Check out [\_\_main__.py](./chatgpt_proxy/__main__.py)
@@ -32,18 +35,18 @@
     refresh_puid_task = asyncio.create_task(proxy._refresh_task())
     yield
 
 app = FastAPI(lifespan=lifespan)
 proxy.attach(app, path="/backend-api")
 ```
 
-`WebChatGPTProxy`:
+class `WebChatGPTProxy`:
 - `puid`: Preset cookie `_puid`
 - `access_token`: (Optional), for automatic refresh of `_puid`
-- `trust`: Trust requests from anyclient.
+- `trust`: Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
 
 # Credits
 - ChatGPT-Proxy-V4
 https://github.com/acheong08/ChatGPT-Proxy-V4
```

### Comparing `chatgpt-proxy-0.0.1/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.0.2/chatgpt_proxy/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 )
 
 if __name__ == "__main__":
     PUID = os.environ["PUID"]
     ACCESS_TOKEN = os.environ.get("ACCESS_TOKEN")
     HOST = os.environ.get("HOST", "127.0.0.1")
     PORT = int(os.environ.get("PORT", 7800))
+    TRUST = os.environ.get("PROXY_TRUST_CLIENT", "False").lower() == "true"
 
-    proxy = WebChatGPTProxy(puid=PUID, access_token=ACCESS_TOKEN, trust=False)
+    proxy = WebChatGPTProxy(puid=PUID, access_token=ACCESS_TOKEN, trust=TRUST)
 
     @asynccontextmanager
     async def lifespan(app: FastAPI):
         refresh_puid_task = asyncio.create_task(proxy._refresh_task())
         yield
 
     app = FastAPI(lifespan=lifespan)
```

### Comparing `chatgpt-proxy-0.0.1/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.0.2/chatgpt_proxy/proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 from starlette.requests import Request
 from starlette.responses import StreamingResponse
 
 
 logger = logging.getLogger(__name__)
 
 
-def parse_set_cookie(headers: httpx.Headers) -> SimpleCookie:
-    cookies = SimpleCookie()
-    for key, value in headers.raw:
-        if key.lower() == b'set-cookie':
-            cookies.load(value.decode("utf-8"))
-    return cookies
-
-
 class ReverseProxy:
     ALL_METHODS = [
         "GET",
         "POST",
         "HEAD",
         "PUT",
         "DELETE",
@@ -65,36 +57,25 @@
             method=request.method,
             headers=await self._prepare_headers(request),
             cookies=await self._prepare_cookies(request),
             content=request.stream(),
         )
 
         # Handle Set-Cookie headers
-        cookies = parse_set_cookie(rp_resp.headers)
         headers = rp_resp.headers.copy()
         headers.pop("set-cookie", None)
 
         resp = StreamingResponse(
             rp_resp.aiter_raw(),
             status_code=rp_resp.status_code,
             headers=headers,
         )
 
-        for key, morsel in cookies.items():
-            resp.set_cookie(
-                key,
-                morsel.value,
-                max_age=morsel.get("max-age", None),
-                expires=morsel.get("expires", None),
-                path=morsel.get("path", "/"),
-                domain=morsel.get("domain", None),
-                secure=morsel.get("secure", False),
-                httponly=morsel.get("httponly", False),
-                samesite=morsel.get("samesite", 'lax'),
-            )
+        for key, value in rp_resp.cookies.items():
+            resp.set_cookie(key=key, value=value)
         return resp
 
     async def _send_request(self, path: str, query: bytes, **kwargs) -> httpx.Response:
         url = httpx.URL(path=path, query=query)
         rp_req = self.client.build_request(url=url, **kwargs)
         rp_resp = await self.client.send(rp_req, stream=True)
         return rp_resp
@@ -148,24 +129,24 @@
     async def _refresh_puid(self) -> None:
         """
         Send requests to /models through reverse proxy (current FastAPI app) to get a new puid
         """
         if self._app is None:
             logger.info("Not attached to any FastAPI app, skip refresh")
         async with httpx.AsyncClient(
-            app=self._app, base_url=f"http://app{self._path}"
+            app=self._app, base_url=f"https://chat.openai.com{self._path}"
         ) as client:
             resp = await client.get(
                 "/models", headers={"authorization": f"Bearer {self.access_token}"}
             )
-            cookies = parse_set_cookie(resp.headers)
-            puid = cookies.get("_puid")
+            print(resp.cookies)
+            puid = resp.cookies.get("_puid")
             if puid:
-                logger.info(f"puid: {puid.value}")
-                self.puid = puid.value
+                logger.info(f"puid: {puid}")
+                self.puid = puid
             else:
                 logger.info("puid not found")
 
     async def _refresh_task(self) -> None:
         if self.access_token is None:
             logger.info("access_token not found, skip refresh")
             return
@@ -178,9 +159,7 @@
                 continue
             await asyncio.sleep(60 * 60 * 6)
 
     def attach(self, app: FastAPI, path: str) -> None:
         super().attach(app=app, path=path)
         self._app = app
         self._path = path
-
-
```

### Comparing `chatgpt-proxy-0.0.1/pyproject.toml` & `chatgpt-proxy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatgpt-proxy"
 authors = [
     {name= "18870"}
 ]
-requires-python = ">=3.9"
-version = "0.0.1"
+requires-python = ">=3.8"
+version = "0.0.2"
 dependencies = [
     "httpx",
     "fastapi",
     "uvicorn"
 ]
 description = "Reverse proxy for OpenAI chatgpt website API"
 classifiers = [
```

