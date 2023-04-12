# Comparing `tmp/the-money-converter-1.0.0.tar.gz` & `tmp/the-money-converter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-money-converter-1.0.0.tar", last modified: Wed Apr 12 03:24:37 2023, max compression
+gzip compressed data, was "the-money-converter-1.0.1.tar", last modified: Wed Apr 12 04:03:06 2023, max compression
```

## Comparing `the-money-converter-1.0.0.tar` & `the-money-converter-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 03:24:37.800913 the-money-converter-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-12 02:49:17.000000 the-money-converter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2208 2023-04-12 03:24:37.800412 the-money-converter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1966 2023-04-12 01:22:22.000000 the-money-converter-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-12 02:51:06.000000 the-money-converter-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 03:24:37.800913 the-money-converter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      536 2023-04-12 03:03:49.000000 the-money-converter-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:24:37.785412 the-money-converter-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 03:24:37.795912 the-money-converter-1.0.0/src/the_money_converter.egg-info/
--rw-rw-rw-   0        0        0     2208 2023-04-12 03:24:37.000000 the-money-converter-1.0.0/src/the_money_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-12 03:24:37.000000 the-money-converter-1.0.0/src/the_money_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 03:24:37.000000 the-money-converter-1.0.0/src/the_money_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-12 03:24:37.000000 the-money-converter-1.0.0/src/the_money_converter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 03:24:37.798412 the-money-converter-1.0.0/src/themoneyconverter/
--rw-rw-rw-   0        0        0      103 2023-04-12 03:01:02.000000 the-money-converter-1.0.0/src/themoneyconverter/__init__.py
--rw-rw-rw-   0        0        0     2564 2023-04-11 13:08:51.000000 the-money-converter-1.0.0/src/themoneyconverter/the_money_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-12 04:03:06.160735 the-money-converter-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-12 02:49:17.000000 the-money-converter-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2201 2023-04-12 04:03:06.159734 the-money-converter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-04-12 04:01:26.000000 the-money-converter-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-12 02:51:06.000000 the-money-converter-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 04:03:06.160735 the-money-converter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      634 2023-04-12 04:02:47.000000 the-money-converter-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 04:03:06.104232 the-money-converter-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 04:03:06.144232 the-money-converter-1.0.1/src/the_money_converter.egg-info/
+-rw-rw-rw-   0        0        0     2201 2023-04-12 04:03:05.000000 the-money-converter-1.0.1/src/the_money_converter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-04-12 04:03:05.000000 the-money-converter-1.0.1/src/the_money_converter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 04:03:05.000000 the-money-converter-1.0.1/src/the_money_converter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 04:03:05.000000 the-money-converter-1.0.1/src/the_money_converter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 04:03:05.000000 the-money-converter-1.0.1/src/the_money_converter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 04:03:06.158234 the-money-converter-1.0.1/src/themoneyconverter/
+-rw-rw-rw-   0        0        0      105 2023-04-12 03:56:35.000000 the-money-converter-1.0.1/src/themoneyconverter/__init__.py
+-rw-rw-rw-   0        0        0     2564 2023-04-11 13:08:51.000000 the-money-converter-1.0.1/src/themoneyconverter/the_money_converter.py
```

### Comparing `the-money-converter-1.0.0/LICENSE` & `the-money-converter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `the-money-converter-1.0.0/PKG-INFO` & `the-money-converter-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: the-money-converter
-Version: 1.0.0
+Version: 1.0.1
 Summary: 货币汇率转换
+Home-page: https://github.com/KILLER2017/the-money-converter
 Author: GetDream_1996
 Author-email: 543046534@qq.com
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Money Converter
@@ -17,30 +18,28 @@
 ```shell
 pip install themoneyconverter
 ```
 
 使用
 
 ```python
-from the_money_converter import MoneyConverter, Currency
+from themoneyconverter import MoneyConverter, Currency
 
 
 if __name__ == '__main__':
     # 获取1元人民币转换其它货币的汇率
     moneyConverter = MoneyConverter(Currency.CNY.name)
     moneyConverter.refresh()
     rate = moneyConverter.get_rate(Currency.ARS.name)
     print(Currency.ARS.value, rate)
 ```
 
 执行结果示例
 ```python
 Connected to pydev debugger (build 203.7717.81)
-Hi, PyCharm
-结果:5.471575446150859 比例：0.8023283317948717
 阿根廷比索 30.9827
 
 Process finished with exit code 0
 ```
 
 代码说明
 ```python
```

### Comparing `the-money-converter-1.0.0/README.md` & `the-money-converter-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,30 +7,28 @@
 ```shell
 pip install themoneyconverter
 ```
 
 使用
 
 ```python
-from the_money_converter import MoneyConverter, Currency
+from themoneyconverter import MoneyConverter, Currency
 
 
 if __name__ == '__main__':
     # 获取1元人民币转换其它货币的汇率
     moneyConverter = MoneyConverter(Currency.CNY.name)
     moneyConverter.refresh()
     rate = moneyConverter.get_rate(Currency.ARS.name)
     print(Currency.ARS.value, rate)
 ```
 
 执行结果示例
 ```python
 Connected to pydev debugger (build 203.7717.81)
-Hi, PyCharm
-结果:5.471575446150859 比例：0.8023283317948717
 阿根廷比索 30.9827
 
 Process finished with exit code 0
 ```
 
 代码说明
 ```python
```

### Comparing `the-money-converter-1.0.0/setup.py` & `the-money-converter-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="the-money-converter",
-    version="1.0.0",
+    version="1.0.1",
     author="GetDream_1996",
     author_email="543046534@qq.com",
     description="货币汇率转换",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    #url="",
+    url="https://github.com/KILLER2017/the-money-converter",
     #project_urls={},
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.0",
+    install_requires=['requests', 'bs4', 'lxml']
 )
```

### Comparing `the-money-converter-1.0.0/src/the_money_converter.egg-info/PKG-INFO` & `the-money-converter-1.0.1/src/the_money_converter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: the-money-converter
-Version: 1.0.0
+Version: 1.0.1
 Summary: 货币汇率转换
+Home-page: https://github.com/KILLER2017/the-money-converter
 Author: GetDream_1996
 Author-email: 543046534@qq.com
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Money Converter
@@ -17,30 +18,28 @@
 ```shell
 pip install themoneyconverter
 ```
 
 使用
 
 ```python
-from the_money_converter import MoneyConverter, Currency
+from themoneyconverter import MoneyConverter, Currency
 
 
 if __name__ == '__main__':
     # 获取1元人民币转换其它货币的汇率
     moneyConverter = MoneyConverter(Currency.CNY.name)
     moneyConverter.refresh()
     rate = moneyConverter.get_rate(Currency.ARS.name)
     print(Currency.ARS.value, rate)
 ```
 
 执行结果示例
 ```python
 Connected to pydev debugger (build 203.7717.81)
-Hi, PyCharm
-结果:5.471575446150859 比例：0.8023283317948717
 阿根廷比索 30.9827
 
 Process finished with exit code 0
 ```
 
 代码说明
 ```python
```

### Comparing `the-money-converter-1.0.0/src/themoneyconverter/the_money_converter.py` & `the-money-converter-1.0.1/src/themoneyconverter/the_money_converter.py`

 * *Files identical despite different names*

