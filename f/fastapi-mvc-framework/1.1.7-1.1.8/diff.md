# Comparing `tmp/fastapi_mvc_framework-1.1.7.tar.gz` & `tmp/fastapi_mvc_framework-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.7.tar", last modified: Tue Apr 11 14:16:20 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.8.tar", last modified: Wed Apr 12 11:48:39 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.7.tar` & `fastapi_mvc_framework-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.448663 fastapi_mvc_framework-1.1.7/
--rw-rw-rw-   0        0        0     7266 2023-04-11 14:16:20.447666 fastapi_mvc_framework-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.441682 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      994 2023-04-11 14:13:14.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0    10309 2023-04-11 12:22:29.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    13007 2023-04-11 14:01:29.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    11379 2023-04-11 05:34:55.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     5413 2023-04-11 11:47:05.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.446669 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     7266 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 14:16:20.448663 fastapi_mvc_framework-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-04-11 14:16:13.000000 fastapi_mvc_framework-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.408079 fastapi_mvc_framework-1.1.8/
+-rw-rw-rw-   0        0        0     7266 2023-04-12 11:48:39.407080 fastapi_mvc_framework-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.399123 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      994 2023-04-11 14:13:14.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0    10309 2023-04-11 12:22:29.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     4120 2023-04-12 11:44:55.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    13007 2023-04-11 14:01:29.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11897 2023-04-12 11:38:53.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     2764 2023-04-12 10:01:06.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5413 2023-04-11 11:47:05.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.406085 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     7266 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 11:48:39.408079 fastapi_mvc_framework-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-04-12 11:48:13.000000 fastapi_mvc_framework-1.1.8/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.7/PKG-INFO` & `fastapi_mvc_framework-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_mvc_framework
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.8 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.7/README.md` & `fastapi_mvc_framework-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import os
 import yaml
 import logging
 from hashlib import md5
+from typing import Dict
 ROOT_PATH = os.path.realpath(os.curdir)
-__levels_or_log = {
- 'CRITICAL' : 50, 
- 'ERROR' : 40,
- 'WARNING' : 30,
- 'INFO' : 20,
- 'DEBUG' : 10,
- 'NOTSET' : 0,
-}
+# from fastapi.logger import logger
 
 import re
 
 def extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
         return None
 
 class YamlConfig:
-    def __init__(self, filename):
+    def __init__(self, filename:str="",config:Dict={}):
         self.filename = filename
-        self.config = {}
+        self.config = config
         self.load()
-
+    def __getitem__(self,key):
+        return self.get(key)
     def load(self):
         if os.path.isfile(self.filename):
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
         elif os.path.isdir(self.filename):
             self.config = self._merge_yaml_files(self.filename)
+        elif self.config:
+            return True
         else:
             raise ValueError(f"{self.filename} is not a file or directory")
 
     def save(self):
+        if not self.filename:
+            return False
         with open(self.filename, "w") as f:
             yaml.safe_dump(self.config, f)
-
-    def get(self, key, default=None):
-        value:str = self.config.get(key, default)
+        return True
+    def get(self, key:str, default=None): 
+        value = self.config.get(key, default)
         if isinstance(value,str) and value.find("{")>-1:
-            name = extract_name(value)
-            if name:
-                expr = self.config.get(name,"")
-                x = f"{name}"
-                value = value.replace('{'+x+'}',expr)
+            while value.find("{")>-1:
+                name = extract_name(value)
+                if name:
+                    expr = self.config.get(name,"")
+                    x = f"{name}"
+                    value = value.replace('{'+x+'}',expr)
+        elif isinstance(value,dict):
+            return YamlConfig(filename="",config=value)
         return value
-
+    
     def set(self, key, value):
         self.config[key] = value
 
     def delete(self, key):
         del self.config[key]
 
     def _merge_dicts(self, dict1, dict2):
@@ -79,13 +81,35 @@
                 dir_config = self._merge_yaml_files(file_path)
                 merged_config = self._merge_dicts(merged_config, dir_config)
         return merged_config
 
     def _load_yaml_file(self, filename):
         with open(filename, "r") as f:
             return yaml.safe_load(f)
+def __init_log(__logCfg):
+    from fastapi.logger import logger
+    __log_level = __logCfg['level'] or 'DEBUG'
+    __log_file = __logCfg['file'] or None 
+    __isdebug = config.get("debug") or False
+    if __log_file:
+        __log_file = os.path.abspath(__log_file)
+    log_format="%(asctime)s %(name)s:%(levelname)s:%(message)s"
+    datefmt="%Y-%M-%d %H:%M:%S" 
+    if __log_file:
+        if __isdebug:
+            try:
+                os.remove(__log_file)
+            except:
+                pass
+        file_handler = logging.FileHandler(__log_file,mode='a')
+        file_handler.setLevel(logging._nameToLevel[__log_level]) 
+        file_handler.setFormatter(logging.Formatter(fmt= log_format,datefmt=datefmt)) 
+        logger.addHandler(file_handler)
+    logger.setLevel(logging._nameToLevel[__log_level]) 
+    return logger
+    # return logging.getLogger(__logCfg['name'] or 'FastapiMvcFramework')
 
 config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
 
-__log_level = config.get('log')['level'] or 'DEBUG'
-logging.basicConfig(level=__levels_or_log[__log_level])
-_log = logging.getLogger(config.get("log")['name'] or "FastApi Framework")
+_log = __init_log(config.get("log"))
+_log.setLevel(logging.DEBUG)
+
```

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,43 +149,47 @@
                 if accept_header == "application/json":
                     return JSONResponse(content={'status':StateCodes.HTTP_200_OK,'msg':msg})
                 return RedirectResponse(url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
             
             @classmethod
             async def _auth__(cls,request:Request,response:Response,**kwargs):
                 '''called by .controller_util.py->route_method'''
+                auth_type = kwargs['auth_type'] 
+                
                 if not hasattr(application,'authObj'):
                     return True,None
-                auth_type = kwargs['auth_type'] 
+                
                 kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
                 if user: #continue singture 
                     application.authObj.create_access_token(user=user, expires_delta=None,request=request)
                 #
                 if not ret and not user: 
+                    _log.debug(f'Failed Auth[type:{auth_type}] url:'+str(request.url))
                     if accept_header == "application/json":
                         return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
                     _auth_url = getattr(application,f"_{auth_type}_auth_url") if hasattr(application,f"_{auth_type}_auth_url") else None
 
                     if _auth_url: 
                         if 'flash' not in request.session:
                             request.session['flash']=''
                         request.session['flash']  = "you are not authenticated,please login!"  
                         _auth_url = add_redirect_param(_auth_url,str(request.url))
                         return RedirectResponse(_auth_url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
                     else:  
                         return RedirectResponse('/',status_code=StateCodes.HTTP_303_SEE_OTHER),None
                 else:
+                    _log.debug(f'Successed Auth[type:{auth_type}] Url:'+str(request.url)+',User:'+str(user))
                     return ret,user
 
         setattr(puppetController,AUTH_KEY,allargs['auth'])         
         setattr(puppetController,"__name__",targetController.__name__)  
         setattr(puppetController,"__controller_name__",targetController.__name__.lower().replace("controller",""))  
         
         setattr(puppetController,"__version__",version)  
@@ -213,14 +217,16 @@
     ret = func
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
 
 def generate_mvc_app( ):
     global __is_debug
+    if __is_debug:
+        _log.debug("\n\n=================================generating mvc app===========================================")
     if not len(__all_controller__)>0:
         raise "must use @api_route to define a controller class"
     all_routers = []
     all_routers_map = {}
     for ctrl in __all_controller__:
         all_routers.append(register_controllers_to_app(application, ctrl))
     for router in all_routers:
@@ -241,14 +247,16 @@
     
     auth_type = config.get("auth",None)
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             application.authObj = __init_auth(application,auth_type)
     __init_database()
+    if __is_debug:
+        _log.debug("=================================generating mvc app end===========================================")
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug
     host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
     port = "port" in kwargs  and kwargs["port"] or 8000
```

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/database.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,88 @@
 from sqlalchemy import create_engine,Engine
 from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy import text,TextClause
+ 
 from alembic import command
 from alembic.config import Config
 import configparser
 import re,os
+from typing import Union
+from .config import _log
+
 engine:Engine=None 
 class Base(DeclarativeBase):
     pass
-
+class Service():
+    @classmethod
+    def execute(cls,cmd:Union[str,TextClause],**kwargs):
+        if not isinstance(cmd,TextClause):
+            cmd = text(str)
+        with engine.begin() as conn:
+            ret = conn.execute(cmd,**kwargs)
+        return ret
+     
 
 def sanitize_path(path):
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
-
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
-
     return sanitized_path
 
 def __check_migration(engine,uri,alembic_ini): 
     def _update_uri_to_ini(): 
         #auto update alembic.ini sqlalchemy.url section 
         config = configparser.ConfigParser() 
-        # 读取配置文件
+        # read ini config
         config.read(alembic_ini)
         config.set('alembic','sqlalchemy.url',uri)
-        # 保存修改后的配置文件
+        # save modified ini file
         with open(alembic_ini, 'w') as f:
             config.write(f)
+        #makesure the migrations directory exists
         reversions_dir = config.get("alembic",'script_location')
+        reversions_dir = os.path.join(reversions_dir,"versions")
         if not os.path.exists(reversions_dir):
             os.makedirs(reversions_dir,exist_ok=True)
 
     _update_uri_to_ini()
-    # 创建 alembic 配置对象
+    #  
     alembic_cfg = Config(alembic_ini)   
-    # 自动检测变更并生成迁移脚本
+    #  
      
     try:
         command.check(config=alembic_cfg)
     except Exception as e: 
         msg = sanitize_path(str(e.args)) 
         command.revision(alembic_cfg, autogenerate=True, message=msg) 
-        # 执行数据库迁移
+        # upgrade the db
         command.upgrade(alembic_cfg, "head") 
 
 def init_database( uri:str,debug:bool=False,alembic_ini:str=""):
     '''
-    params :uri sqlalchemy 的连接字符串
-    :params debug 是否调试模式
-    :params alembic_ini alembic的配置文件路径,debug=True时则会执行数据迁移
+    params :uri sqlalchemy connection string
+    :params debug mode of debug 
+    :params alembic_ini alembic config file path,when debug=True will auto migrate the changes 
     '''
     engine = create_engine(uri, echo=debug)
+    
     if debug and alembic_ini:
-        __check_migration(engine,uri,alembic_ini)
+        try:
+            #Base.metadata.create_all(engine)
+            __check_migration(engine,uri,alembic_ini)
+        except Exception as e:
+            _log.error(e.args)
+    #test connect
+    try:
+        with engine.connect() as conn:
+            _log.disabled = False
+            _log.debug('database connection successed:' + str(conn))
+
+    except Exception as e:
+        _log.disabled = False
+        _log.error("database connection failed!")  
+         
+        exit(1)  
+
     return engine
```

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc-framework
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.7 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.8 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.7/setup.py` & `fastapi_mvc_framework-1.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     long_description = fh.read()
 with open('requirements.txt', encoding="utf-8-sig") as f:
     requirements = f.readlines()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.7',
+    version='1.1.8',
     license='Apache License 2.0',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

