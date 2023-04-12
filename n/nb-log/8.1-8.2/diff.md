# Comparing `tmp/nb_log-8.1.tar.gz` & `tmp/nb_log-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-8.1.tar", last modified: Mon Apr  3 03:41:35 2023, max compression
+gzip compressed data, was "dist\nb_log-8.2.tar", last modified: Wed Apr 12 09:54:01 2023, max compression
```

## Comparing `nb_log-8.1.tar` & `nb_log-8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 03:41:35.000000 nb_log-8.1/
--rw-rw-rw-   0        0        0    27863 2023-04-03 03:41:35.000000 nb_log-8.1/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 03:41:35.000000 nb_log-8.1/nb_log/
--rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.1/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50515 2022-12-23 03:23:06.000000 nb_log-8.1/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.1/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30311 2023-04-03 03:39:42.000000 nb_log-8.1/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7183 2022-09-17 06:12:29.000000 nb_log-8.1/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     8782 2023-03-23 09:52:31.000000 nb_log-8.1/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7530 2022-09-17 06:13:18.000000 nb_log-8.1/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-04-03 03:41:35.000000 nb_log-8.1/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27863 2023-04-03 03:41:34.000000 nb_log-8.1/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-03 03:41:35.000000 nb_log-8.1/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 03:41:34.000000 nb_log-8.1/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-04-03 03:41:34.000000 nb_log-8.1/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-03 03:41:34.000000 nb_log-8.1/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 03:41:35.000000 nb_log-8.1/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-04-03 03:41:28.000000 nb_log-8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/
+-rw-rw-rw-   0        0        0    27863 2023-04-12 09:54:01.000000 nb_log-8.2/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2022-12-05 09:46:23.000000 nb_log-8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/nb_log/
+-rw-rw-rw-   0        0        0     2329 2022-09-17 07:28:19.000000 nb_log-8.2/nb_log/__init__.py
+-rw-rw-rw-   0        0        0    50515 2022-12-23 03:23:06.000000 nb_log-8.2/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-8.2/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    30380 2023-04-12 09:53:33.000000 nb_log-8.2/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     7183 2022-09-17 06:12:29.000000 nb_log-8.2/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0     8847 2023-04-03 09:15:14.000000 nb_log-8.2/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     7530 2022-09-17 06:13:18.000000 nb_log-8.2/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:54:01.000000 nb_log-8.2/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27863 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 09:54:00.000000 nb_log-8.2/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:54:01.000000 nb_log-8.2/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-04-12 09:53:51.000000 nb_log-8.2/setup.py
```

### Comparing `nb_log-8.1/PKG-INFO` & `nb_log-8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.1
+Version: 8.2
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.1/README.md` & `nb_log-8.2/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log/__init__.py` & `nb_log-8.2/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log/handlers.py` & `nb_log-8.2/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log/handlers0000.py` & `nb_log-8.2/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log/log_manager.py` & `nb_log-8.2/nb_log/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
     """
     Set the logging level of this logger.  level must be an int or a str.
     """
     level2 = LogManager.preset_name__level_map.get(self.name, level)
     if level2 != level:
         very_nb_print(f'日志命名空间 {self.name} 已经锁定了为了 {level2} 级别 ,后续不可以更改为 {level} 级别')
     self.level = _checkLevel(level2)
-    self.manager._clear_cache()
+    if sys.version_info.minor >=7:  # python3.6 没有 _clear_cache 方法
+        self.manager._clear_cache()
+
 
 
 logging.Logger.callHandlers = revision_call_handlers  # 打猴子补丁。
 logging.Logger.addHandler = revision_add_handler  # 打猴子补丁。
 logging.Logger.setLevel = revision_setLevel  # 打猴子补丁。
 
 
@@ -202,16 +204,16 @@
     logger_list = []
     preset_name__level_map = dict()
 
     def __init__(self, logger_name: typing.Union[str, None] = 'nb_log_default_namespace'):
         """
         :param logger_name: 日志名称，当为None时候创建root命名空间的日志，一般情况下千万不要传None，除非你确定需要这么做和是在做什么.这个命名空间是双刃剑
         """
-        if logger_name in (None, '', 'root') and multiprocessing.process.current_process().name == 'MainProcess':
-            very_nb_print('logger_name 设置为None和root和空字符串都是一个意义，在操作根日志命名空间，任何其他日志的行为将会发生变化，'
+        if logger_name in (None, '', ) and multiprocessing.process.current_process().name == 'MainProcess':
+            very_nb_print('logger_name 设置为None和空字符串都是一个意义，在操作根日志命名空间，任何其他日志的行为将会发生变化，'
                           '一定要弄清楚原生logging包的日志name的意思。这个命名空间是双刃剑')
         self._logger_name = logger_name
         self.logger = logging.getLogger(logger_name)
 
     def preset_log_level(self, log_level_int=20):
         """
         提前设置锁定日志级别，当之后再设置该命名空间日志的级别的时候，按照提前预设的级别，无视之后设定的级别。
```

### Comparing `nb_log-8.1/nb_log/monkey_print.py` & `nb_log-8.2/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log/nb_log_config_default.py` & `nb_log-8.2/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,37 @@
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
-LOG_FILE_BACKUP_COUNT = 14  # 对同一个日志文件，默认最多备份几个文件，超过就删除了。
+LOG_FILE_BACKUP_COUNT = 10  # 对同一个日志文件，默认最多备份几个文件，超过就删除了。
 
 LOG_PATH = '/pythonlogs'  # 默认的日志文件夹,如果不写明磁盘名，则是项目代码所在磁盘的根目录下的/pythonlogs
 # LOG_PATH = Path(__file__).absolute().parent / Path("pythonlogs")   #这么配置就会自动在你项目的根目录下创建pythonlogs文件夹了并写入。
 if os.name == 'posix':  # linux非root用户和mac用户无法操作 /pythonlogs 文件夹，没有权限，默认修改为   home/[username]  下面了。例如你的linux用户名是  xiaomin，那么默认会创建并在 /home/xiaomin/pythonlogs文件夹下写入日志文件。
     home_path = os.environ.get("HOME", '/')  # 这个是获取linux系统的当前用户的主目录，不需要亲自设置
     LOG_PATH = Path(home_path) / Path('pythonlogs')  # linux mac 权限很严格，非root权限不能在/pythonlogs写入，修改一下默认值。
+# print('LOG_PATH:',LOG_PATH)
 
 LOG_FILE_HANDLER_TYPE = 1  # 1 2 3 4 5
 """
 LOG_FILE_HANDLER_TYPE 这个值可以设置为 1 2 3 4 5 四种值，
 1为使用多进程安全按日志文件大小切割的文件日志,这是本人实现的批量写入日志，减少操作文件锁次数，测试10进程快速写入文件，win上性能比第5种提高了100倍，linux提升5倍
 2为多进程安全按天自动切割的文件日志，同一个文件，每天生成一个新的日志文件。日志文件名字后缀自动加上日期。
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
 
 LOG_LEVEL_FILTER = logging.DEBUG  # 默认日志级别，低于此级别的日志不记录了。例如设置为INFO，那么logger.debug的不会记录，只会记录logger.info以上级别的。
                                   # 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
-                                  # https://nb-log-doc.readthedocs.io/zh_CN/latest 文档里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
+                                  # https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
 
 RUN_ENV = 'test'
 
 FORMATTER_DICT = {
     1: logging.Formatter(
         '日志时间【%(asctime)s】 - 日志名称【%(name)s】 - 文件【%(filename)s】 - 第【%(lineno)d】行 - 日志等级【%(levelname)s】 - 日志信息【%(message)s】',
         "%Y-%m-%d %H:%M:%S"),
@@ -114,15 +115,15 @@
     5: logging.Formatter(
         '%(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s',
         "%Y-%m-%d %H:%M:%S"),  # 我认为的最好的模板,推荐
     6: logging.Formatter('%(name)s - %(asctime)-15s - %(filename)s - %(lineno)d - %(levelname)s: %(message)s',
                          "%Y-%m-%d %H:%M:%S"),
     7: logging.Formatter('%(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 一个只显示简短文件名和所处行数的日志模板
 
-    8: JsonFormatterJumpAble('%(asctime)s - %(name)s - %(levelname)s - %(message)s - "%(filename)s %(lineno)d -" ', "%Y-%m-%d %H:%M:%S", json_ensure_ascii=False),  # 这个是json日志，方便分析.
+    8: JsonFormatterJumpAble('%(asctime)s - %(name)s - %(levelname)s - %(message)s - "%(filename)s %(lineno)d -" ', "%Y-%m-%d %H:%M:%S", json_ensure_ascii=False),  # 这个是json日志，方便elk采集分析.
 
     9: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s',
         "%Y-%m-%d %H:%M:%S"),  # 对5改进，带进程和线程显示的日志模板。
     10: logging.Formatter(
         '[p%(process)d_t%(thread)d] %(asctime)s - %(name)s - "%(filename)s:%(lineno)d" - %(levelname)s - %(message)s', "%Y-%m-%d %H:%M:%S"),  # 对7改进，带进程和线程显示的日志模板。
     11: logging.Formatter(
```

### Comparing `nb_log-8.1/nb_log/set_nb_log_config.py` & `nb_log-8.2/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.1/nb_log.egg-info/PKG-INFO` & `nb_log-8.2/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.1
+Version: 8.2
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.1/setup.py` & `nb_log-8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.1",
+    version="8.2",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -61,14 +61,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.1.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-8.2.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

