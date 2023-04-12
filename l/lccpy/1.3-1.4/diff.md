# Comparing `tmp/lccpy-1.3.tar.gz` & `tmp/lccpy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.3.tar", last modified: Mon Apr 10 14:10:50 2023, max compression
+gzip compressed data, was "lccpy-1.4.tar", last modified: Wed Apr 12 15:21:34 2023, max compression
```

## Comparing `lccpy-1.3.tar` & `lccpy-1.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.3/LICENSE
--rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.3/lccpy/__init__.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.3/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.3/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20516 2023-04-10 03:17:09.725430 lccpy-1.3/lccpy/asymongo/_asymongo.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.3/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.3/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    20195 2023-04-10 03:17:33.907847 lccpy-1.3/lccpy/asymysql/_asymysql.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.3/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.3/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.3/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.3/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20932 2023-04-10 03:19:30.328296 lccpy-1.3/lccpy/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.3/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.3/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    19848 2023-04-10 03:19:42.932854 lccpy-1.3/lccpy/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.3/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.3/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.3/lccpy/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.3/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1512 2023-04-08 15:57:17.331903 lccpy-1.3/lccpy/increment/_increment.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.3/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.3/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.3/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.3/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    11905 2023-04-09 16:11:55.211629 lccpy-1.3/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      571 2023-04-10 09:23:39.492835 lccpy-1.3/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 lccpy-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4/LICENSE
+-rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4/lccpy/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4/lccpy/_mtype.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
+-rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4/lccpy/asymongo/_asymongo.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    20193 2023-04-11 02:42:51.177983 lccpy-1.4/lccpy/asymysql/_asymysql.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4/lccpy/coolmongo/_coolmongo.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    21648 2023-04-12 14:25:22.814767 lccpy-1.4/lccpy/coolmysql/_coolmysql.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4/lccpy/encrypt256/_encrypt256.py
+-rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4/lccpy/increment/_increment.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4/lccpy/vtype/_cooltime.py
+-rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      571 2023-04-12 15:08:03.806587 lccpy-1.4/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 lccpy-1.4/PKG-INFO
```

### Comparing `lccpy-1.3/LICENSE` & `lccpy-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/asymongo/_asymongo.py` & `lccpy-1.4/lccpy/asymongo/_asymongo.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient  # 代码提示
 
 from ..vtype import uniset, empset, SysEmpty, ToolPool
+from .._mtype import MgIndexError
 
 
 class Factory:
     _variable = True
 
     def __init__(self, where):
         if where is not empset:
@@ -173,16 +174,14 @@
 repairUpsert = False
 # pymongo官方bug
 # cannot infer query fields to set, path 'a' is matched twice, full error: {'index': 0, 'code': 54, 'errmsg': "cannot infer query fields to set, path 'a' is matched twice"}
 
 
 class allColumns: ...
 
-class MgIndexError(IndexError): ...
-
 
 class makeSlice():
     def __init__(self, func, *vs, **kvs):
         self.func = func
         self.vs = vs
         self.kvs = kvs
     def __getitem__(self, key):
```

### Comparing `lccpy-1.3/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/asymysql/_asymysql.py` & `lccpy-1.4/lccpy/asymysql/_asymysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from copy import deepcopy
 from collections import deque
 from aiomysql.cursors import DictCursor
 
 from ..vtype import uniset, empset, SysEmpty
 from ..coolfunc import jsonChinese
+from .._mtype import MgIndexError
 
 
 class ToolPool():
     async def asy_init(self, mktool, minlen:int=0, maxlen=None):
         self.mktool = mktool
         self.pool = deque([await mktool() for i in range(minlen or 0)], maxlen=maxlen)
     
@@ -238,15 +239,14 @@
         self.func = func
         self.vs = vs
         self.kvs = kvs
     
     def __getitem__(self, key):
         return self.func(key, *self.vs, **self.kvs)
 
-class MgIndexError(IndexError): ...
 
 class sheetORM():
     _variable = True
     _pk = ''
 
     def __init__(self, connPool:ToolPool, dbName:str, sheetName:str, where=None, columns='*', _sort=None):
         if not columns: ValueError('columns 不能为空')
```

### Comparing `lccpy-1.3/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/coolmongo/_coolmongo.py` & `lccpy-1.4/lccpy/coolmongo/_coolmongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from pymongo import MongoClient  # 代码提示
 
 from ..vtype import uniset, empset, SysEmpty, ToolPool
+from .._mtype import MgIndexError
 
 
 class Factory:
     _variable = True
 
     def __init__(self, where):
         if where is not empset:
@@ -183,15 +184,14 @@
 repairUpsert = False
 # pymongo官方bug
 # cannot infer query fields to set, path 'a' is matched twice, full error: {'index': 0, 'code': 54, 'errmsg': "cannot infer query fields to set, path 'a' is matched twice"}
 
 
 class allColumns: ...
 
-class MgIndexError(IndexError): ...
 
 class sheetORM():
     _variable = True
 
     def __init__(self, connPool:ToolPool, dbName:str, sheetName:str, where=None, columns=allColumns, _sort=None):
         assert columns
         self.connPool = connPool
```

### Comparing `lccpy-1.3/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/coolmysql/_coolmysql.py` & `lccpy-1.4/lccpy/coolmysql/_coolmysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from copy import deepcopy
 from collections import deque
 from pymysql import connect  # 代码提示
 from pymysql.cursors import DictCursor
 
 from ..vtype import uniset, empset, SysEmpty
 from ..coolfunc import jsonChinese
+from .._mtype import MgIndexError
 
 
 class ToolPool():
     def __init__(self, mktool, minlen:int=0, maxlen=None):
         self.mktool = mktool
         self.pool = deque([mktool() for i in range(minlen or 0)], maxlen=maxlen)
     
@@ -237,27 +238,25 @@
         self.func = func
         self.vs = vs
         self.kvs = kvs
     
     def __getitem__(self, key):
         return self.func(key, *self.vs, **self.kvs)
 
-class MgIndexError(IndexError): ...
-
 class sheetORM():
     _variable = True
     _pk = ''
 
     def __init__(self, connPool:ToolPool, dbName:str, sheetName:str, where=None, columns='*', _sort=None):
-        if not columns: ValueError('columns 不能为空')
+        assert columns  # 不能为空
+        self.columns = columns  # str型 或 tuple型
         self.connPool = connPool
         self.dbName = dbName
         self.sheetName = sheetName
         self.where = where or Factory(uniset)
-        self.columns = columns  # str型 或 tuple型
         self._sort = deepcopy(_sort or {})
             # {A:True, B:False, C:1, D:0}
             # bool(value) == True --> 升序
             # bool(value) == False --> 降序
         self._variable = False
 
     def __setattr__(self, name, value):
@@ -283,14 +282,63 @@
             return ' order by ' + ', '.join([k if v else f"{k} desc" for k,v in self._sort.items()])
         return ''
 
     def _ParseColumns(self):
         if type(self.columns) is str:
             return self.columns
         return ', '.join(self.columns)
+    
+    def apply(self, handler):
+        return makeSlice(self._applyBase, handler=handler)
+    
+    def _applyBase(self, key, handler):
+        pk = self.getPK()
+        # 添加主键字段
+        cols = raw_columns = self.columns
+        if isinstance(cols, str): cols = [cols]
+        for x in cols:
+            if x.strip() in ('*', pk):
+                break
+        else:
+            self.columns = tuple(list(cols) + [pk])
+        # 从数据库提取数据
+        lines = self[key]
+        object.__setattr__(self, 'columns', raw_columns)  # 恢复用户设定的columns
+        if type(lines) is dict:
+            lines = [lines]
+            r_type = 'dict'
+        else:
+            r_type = 'list'
+        # 处理数据
+        records = {}
+        for line in lines:
+            line2 = line.copy()
+            handler(line2)
+            key = line[pk]
+            for k, v in line2.items():
+                if v != line.get(k, SysEmpty):
+                    records.setdefault(k, {})[key] = v
+        if r_type == 'dict':
+            lines = lines[0]
+        # 更新到数据库
+        if records:
+            blocks = []
+            for field, kvs in records.items():
+                s = [f"{field} = ", '    case']
+                for k, v in kvs.items():
+                    s.append(f"        when {pk} = {jsonChinese(k)} then {jsonChinese(v)}")
+                s.append(f"else {field}")
+                s.append('end')
+                blocks.append('\n'.join(s))
+            blocks = ' ,\n'.join(blocks)
+            sql = f"update {self.sheetName} set \n{blocks}"
+            r, cursor = self.execute(sql=sql)
+            return dict(datas=lines, cursor=cursor, result=r)
+        else:
+            return dict(datas=lines, cursor=None, result=None)
 
     def order(self, **rule): return self._copy(_sort={**rule})
 
     def __add__(self, data):
         if type(data) is dict:
             cols = data.keys()
             sql = f"insert into {self.sheetName}({', '.join(cols)}) values ({', '.join(('%s',)*len(cols))})"
```

### Comparing `lccpy-1.3/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/encrypt256/_encrypt256.py` & `lccpy-1.4/lccpy/encrypt256/_encrypt256.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/increment/_increment.py` & `lccpy-1.4/lccpy/increment/_increment.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     return Characters[0]
 
 getTid = lambda : EncodeNum(int(time.time() * 1000))  # 一般毫秒后面的数值没有分辨率
 pid = EncodeNum(os.getpid())
 
 class incrementer():
     def __init__(self, macid=None, macidSize=4):
-        self._threads = []
-        self._ContPool = deque()
+        self._threads = []  # 线程安全
+        self._ContPool = deque()  # 线程安全
         self.macid = macid or ''.join(choices(Characters, k=macidSize or 1))
         self._TMP = f"{getTid()}_{self.macid}_{pid}"
 
     def _getid(self):
         try:
             cont = self._ContPool.popleft()
         except:
```

### Comparing `lccpy-1.3/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/vtype/_cooltime.py` & `lccpy-1.4/lccpy/vtype/_cooltime.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.3/lccpy/vtype/_vtype.py` & `lccpy-1.4/lccpy/vtype/_vtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,41 +20,38 @@
     '''
         解决 1 == True 的历史遗留问题
     '''
     name: str
     _hash_value: int
     _bool_vlaue: bool
     def __new__(cls, value, name='', _sysValue=False):
-        self = object.__new__(cls)
         if _sysValue:
+            self = object.__new__(cls)
             self.name = name
             self._bool_vlaue = bool(value)
-            self._hash_value = hash(lambda: ...)  # 生成一个随机但固定的值
             return self
         else:
             return vtrue if value else vfalse
 
-    def __eq__(self, o): return self is o
-    def __hash__(self): return self._hash_value
     def __bool__(self): return self._bool_vlaue
+    def __eq__(self, o): return self is o
     def __str__(self): return self.name
 
 vtrue = vbool(True, 'vtrue', _sysValue=True)
 vfalse = vbool(False, 'vfalse', _sysValue=True)
 
 uniset = vbool(True, 'uniset', _sysValue=True)  # 全集
 empset = vbool(False, 'empset', _sysValue=True)  # 空集
 
 SysEmpty = vbool(False, 'SysEmpty', _sysValue=True)
     # 供开发者调用的表示空的标识, 如:
         # 作为默认参数以识别调用者是否传参
         # 在函数内部作为某种状态标识
     # 此参数只允许函数开发者引用, 禁止函数调用者引用.
 
-
 ########################################## bidict ##########################################
 
 class bidict:
     ''' 双向字典 '''
     def __init__(self):
         self.core = {}
```

### Comparing `lccpy-1.3/pyproject.toml` & `lccpy-1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.3"
+version = "1.4"
 description = "The dependent package of project <Make Python simpler> ."
 dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `lccpy-1.3/PKG-INFO` & `lccpy-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.3
+Version: 1.4
 Summary: The dependent package of project <Make Python simpler> .
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
```

