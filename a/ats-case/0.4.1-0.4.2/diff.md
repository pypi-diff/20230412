# Comparing `tmp/ats_case-0.4.1.tar.gz` & `tmp/ats_case-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.1.tar", last modified: Tue Apr 11 03:21:31 2023, max compression
+gzip compressed data, was "ats_case-0.4.2.tar", last modified: Wed Apr 12 01:19:10 2023, max compression
```

## Comparing `ats_case-0.4.1.tar` & `ats_case-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.625325 ats_case-0.4.1/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-11 03:21:31.618344 ats_case-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.092851 ats_case-0.4.1/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.1/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.304100 ats_case-0.4.1/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.1/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17233 2023-04-11 03:13:22.000000 ats_case-0.4.1/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.1/ats_case/case/context.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 01:42:05.000000 ats_case-0.4.1/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5435 2023-04-10 06:53:43.000000 ats_case-0.4.1/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.491562 ats_case-0.4.1/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.1/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.1/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.1/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.561223 ats_case-0.4.1/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.1/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.1/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2584 2023-04-10 01:54:51.000000 ats_case-0.4.1/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.600079 ats_case-0.4.1/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.1/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-04-11 02:59:20.000000 ats_case-0.4.1/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-11 03:21:31.185604 ats_case-0.4.1/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 03:21:30.000000 ats_case-0.4.1/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 03:21:31.625325 ats_case-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-04-11 03:14:31.000000 ats_case-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.180730 ats_case-0.4.2/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-12 01:19:10.169760 ats_case-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.204342 ats_case-0.4.2/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.2/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.929402 ats_case-0.4.2/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.2/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17147 2023-04-12 01:02:29.000000 ats_case-0.4.2/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.2/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     5143 2023-04-12 01:07:14.000000 ats_case-0.4.2/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.2/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.045093 ats_case-0.4.2/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.2/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.2/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.2/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.092965 ats_case-0.4.2/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.2/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.2/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.2/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.143829 ats_case-0.4.2/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.2/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.2/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.389847 ats_case-0.4.2/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 01:19:10.180730 ats_case-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-04-12 01:19:03.000000 ats_case-0.4.2/setup.py
```

### Comparing `ats_case-0.4.1/PKG-INFO` & `ats_case-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.1
+Version: 0.4.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.1/README.md` & `ats_case-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.1/ats_case/case/command.py` & `ats_case-0.4.2/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,17 +217,15 @@
         logger.info('~ @PRO-ENCODE<- protocol:{} frame:{}'.format(self._protocol, parse.get('frame')))
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context):
         if self._frame is None or len(self._frame) <= 0:
-            cre = ClientReturnError(self._frame)
-            client().operation("app:error").message(str(cre))
-            raise cre
+            raise ClientReturnError(self._frame)
 
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         self._handle_framing(context, data)
```

### Comparing `ats_case-0.4.1/ats_case/case/context.py` & `ats_case-0.4.2/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.1/ats_case/case/executor.py` & `ats_case-0.4.2/ats_case/case/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from importlib import import_module
 
 from ats_base.log.logger import logger
 
 from ats_case.case import translator, command
 from ats_case.case.context import Context
 from ats_case.common.enum import *
+from ats_case.common.error import *
 
 
 def execute(context: Context):
-    if context.mode == WorkMode.FORMAL:
-        FormalExecutor(context).exec()
-    else:
-        DebugExecutor(context).exec()
+    try:
+        if context.mode == WorkMode.FORMAL:
+            FormalExecutor(context).exec()
+        else:
+            DebugExecutor(context).exec()
+    except APIError as ae:
+        logger.info(str(ae))
+        raise AssertionError(str(ae))
+    except ClientReturnError as ce:
+        logger.info(str(ce))
+        command.client().operation("app:error").message(str(ce))
+        raise AssertionError(str(ce))
+    except Exception as e:
+        logger.error(str(e))
+        command.client().operation("app:error").message(str(e))
+        raise AssertionError(str(e))
 
 
 class Executor(object):
     def __init__(self, context: Context):
         self._context = context
         self._model = None
 
@@ -33,15 +46,15 @@
     def step_exec(self):
         try:
             logger.info('~ @TCC-STEP-> steps[#{}] execute'.format(self._context.runtime.step))
 
             if self.is_exec():
                 getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
         except Exception as e:
-            logger.error(str(e))
+            raise Exception(str(e))
 
     def loop_meet(self):
         try:
             loops = self._context.case.control.get('loops')
 
             if loops is None or type(loops) is not list or len(loops) <= 0:
                 return False
@@ -58,15 +71,15 @@
             if step_start <= self._context.runtime.step <= step_end:
                 self._context.runtime.loop_start_step = step_start
                 self._context.runtime.loop_end_step = step_end
                 self._context.runtime.loop_count = int(count)
                 self._context.runtime.loop_index = 0
                 return True
         except Exception as e:
-            logger.error(str(e))
+            raise Exception(str(e))
 
         return False
 
     def loop_exec(self):
         logger.info('~ @TCC-LOOP-> loops[#{}] start. -range {}:{}  -count {}'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
             self._context.runtime.loop_end_step, self._context.runtime.loop_count))
```

### Comparing `ats_case-0.4.1/ats_case/case/translator.py` & `ats_case-0.4.2/ats_case/case/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 # if self._contain_keyword(step):
                 #     tab_count += 1
                 f.write(self._gen_line(2))
 
             return steps
 
     def _script(self):
-        user_dir = func.makeDir(os.getenv('PWD'), 'script', 'debug', self._context.tester.username)
+        user_dir = func.makeDir(func.project_dir(), 'script', 'debug', self._context.tester.username)
         script_file = os.path.join(user_dir, 'steps.py')
 
         if not os.path.exists(user_dir):
             Path(user_dir).mkdir(parents=True, exist_ok=True)
 
         return script_file
```

### Comparing `ats_case-0.4.1/ats_case/common/error.py` & `ats_case-0.4.2/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.1/ats_case/manage/core.py` & `ats_case-0.4.2/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.1/ats_case/manage/start.py` & `ats_case-0.4.2/ats_case/manage/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def _save(self):
         pass
 
     def _build(self, work_mode: WorkMode, code: str = None):
         if code is None:
             code = 'case'
 
-        user_dir = func.makeDir(os.getenv('PWD'), 'testcase', work_mode.value.lower(), self._username)
+        user_dir = func.makeDir(func.project_dir(), 'testcase', work_mode.value.lower(), self._username)
         template_file = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'template', 'testcase_v1.tmp')
         script_file = os.path.join(user_dir, 'test_{}.py'.format(code))
 
         with open(template_file, 'r', encoding='UTF-8') as file:
             content = file.read()
             content = content.replace('{script}', code.upper())
         with open(script_file, 'w', encoding='UTF-8') as file:
```

### Comparing `ats_case-0.4.1/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.2/ats_case/template/testcase_v1.tmp`

 * *Files 10% similar despite different names*

```diff
@@ -42,16 +42,9 @@
     def test_main(self, CaseContext):
         """
         测试用例主体步骤
         :return:
         """
         logger.info('~ @TCC-MSG-> SCRIPT START -mode "{}" -client "{}"'.
                     format(CaseContext.mode, CaseContext.tester.api))
-        try:
-            executor.execute(CaseContext)
-        except APIError as ae:
-            logger.info(str(ae))
-            raise AssertionError(str(ae))
-        except ClientReturnError as ce:
-            logger.info(str(ce))
-            raise AssertionError(str(ce))
+        executor.execute(CaseContext)
```

### Comparing `ats_case-0.4.1/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.2/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.1
+Version: 0.4.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.1/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.2/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.1/setup.py` & `ats_case-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.1",
+    version="0.4.2",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

