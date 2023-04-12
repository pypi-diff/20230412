# Comparing `tmp/airlabs-0.0.1.tar.gz` & `tmp/airlabs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlabs-0.0.1.tar", last modified: Tue Apr 11 23:52:18 2023, max compression
+gzip compressed data, was "airlabs-0.0.2.tar", last modified: Wed Apr 12 00:11:00 2023, max compression
```

## Comparing `airlabs-0.0.1.tar` & `airlabs-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 23:52:18.450427 airlabs-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-11 20:29:40.000000 airlabs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       57 2023-04-11 20:29:40.000000 airlabs-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1973 2023-04-11 23:52:18.450427 airlabs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-04-11 22:55:06.000000 airlabs-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 23:52:18.451425 airlabs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-04-11 20:29:40.000000 airlabs-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:52:18.439350 airlabs-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 23:52:18.446438 airlabs-0.0.1/src/airlabs/
--rw-rw-rw-   0        0        0       27 2023-04-11 20:29:40.000000 airlabs-0.0.1/src/airlabs/__init__.py
--rw-rw-rw-   0        0        0     9455 2023-04-11 23:44:56.000000 airlabs-0.0.1/src/airlabs/endpoints.py
--rw-rw-rw-   0        0        0      460 2023-04-11 23:30:26.000000 airlabs-0.0.1/src/airlabs/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:52:18.449430 airlabs-0.0.1/src/airlabs.egg-info/
--rw-rw-rw-   0        0        0     1973 2023-04-11 23:52:18.000000 airlabs-0.0.1/src/airlabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-11 23:52:18.000000 airlabs-0.0.1/src/airlabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 23:52:18.000000 airlabs-0.0.1/src/airlabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 23:52:18.000000 airlabs-0.0.1/src/airlabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       38 2023-04-11 20:29:40.000000 airlabs-0.0.1/versions.md
+drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.086203 airlabs-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-11 20:29:40.000000 airlabs-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-04-11 20:29:40.000000 airlabs-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1946 2023-04-12 00:11:00.085176 airlabs-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1461 2023-04-11 23:56:33.000000 airlabs-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 00:11:00.086203 airlabs-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-04-12 00:10:38.000000 airlabs-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.075202 airlabs-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.082213 airlabs-0.0.2/src/airlabs/
+-rw-rw-rw-   0        0        0       27 2023-04-11 20:29:40.000000 airlabs-0.0.2/src/airlabs/__init__.py
+-rw-rw-rw-   0        0        0     9455 2023-04-11 23:44:56.000000 airlabs-0.0.2/src/airlabs/endpoints.py
+-rw-rw-rw-   0        0        0      460 2023-04-11 23:30:26.000000 airlabs-0.0.2/src/airlabs/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.084209 airlabs-0.0.2/src/airlabs.egg-info/
+-rw-rw-rw-   0        0        0     1946 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2023-04-12 00:10:33.000000 airlabs-0.0.2/versions.md
```

### Comparing `airlabs-0.0.1/LICENSE` & `airlabs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.1/PKG-INFO` & `airlabs-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,59 @@
-Metadata-Version: 2.1
-Name: airlabs
-Version: 0.0.1
-Summary: Python wrapper for AirLabs
-Home-page: https://github.com/calebyhan/AirLabs
-Author: Caleb Han
-Author-email: calebhantech@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-**Project Portfolio: https://github.com/calebyhan/CalebHan**
-
-# airlabs-ch
-
-Python wrapper for [AirLabs](https://airlabs.co/).
-
-
-## Installation
-----------------------
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install currency-ch.
-
-```bash
-pip install airlabs-ch
-```
-
-
-## Usage
-----------------------
-
-```python
-import airlabs
-
-# converts amount of money from one currency to another
-currency.convert("usd", "eur", 1)
-
-# returns rate from one currency to another
-currency.rate("usd", "eur")
-```
-
-
-## Documentation
-----------------------
-
-``currency.convert(input_currency, output_currency, amount, roundTo)``
-
-Converts input_currency of amount (default 1) to output_currency with rounded to roundTo decimal places (default 2).
-
-``currency.rate(input_currency, output_currency, roundTo)``
-
-Returns rate of converting input_currency to output_currency rounded to roundTo decimal places (default 2).
-
-``currency.add(values, output_currency, roundTo)``
-
-Adds up currencies in 2-D array values (in format [amount, input_currency]), and displays in form of output_currency rounded to roundTo decimal places (default 2).
-
-## Contributing
-----------------------
-
-Pull requests are welcome. For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-
-
-## License
-----------------------
-
-[MIT](https://choosealicense.com/licenses/mit/)
+**Project Portfolio: https://github.com/calebyhan/CalebHan**
+
+# airlabs
+
+Python wrapper for [AirLabs](https://airlabs.co/).
+
+
+## Installation
+----------------------
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install airlabs.
+
+```bash
+pip install airlabs
+```
+
+
+## Usage
+----------------------
+
+```python
+import airlabs
+
+# Gets airline information about American Airlines
+airlabs.airlines(iata_code="AA")
+
+# Gets information about real-time flights
+airlabs.flights()
+```
+
+
+## Documentation
+----------------------
+
+``currency.convert(input_currency, output_currency, amount, roundTo)``
+
+Converts input_currency of amount (default 1) to output_currency with rounded to roundTo decimal places (default 2).
+
+``currency.rate(input_currency, output_currency, roundTo)``
+
+Returns rate of converting input_currency to output_currency rounded to roundTo decimal places (default 2).
+
+``currency.add(values, output_currency, roundTo)``
+
+Adds up currencies in 2-D array values (in format [amount, input_currency]), and displays in form of output_currency rounded to roundTo decimal places (default 2).
+
+## Contributing
+----------------------
+
+Pull requests are welcome. For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+
+## License
+----------------------
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `airlabs-0.0.1/setup.py` & `airlabs-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="airlabs",
-    version="0.0.1",
+    version="0.0.2",
     description="Python wrapper for AirLabs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/calebyhan/AirLabs",
     author="Caleb Han",
     author_email="calebhantech@gmail.com",
     license="MIT",
```

### Comparing `airlabs-0.0.1/src/airlabs/endpoints.py` & `airlabs-0.0.2/src/airlabs/endpoints.py`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.1/src/airlabs.egg-info/PKG-INFO` & `airlabs-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: airlabs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for AirLabs
 Home-page: https://github.com/calebyhan/AirLabs
 Author: Caleb Han
 Author-email: calebhantech@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **Project Portfolio: https://github.com/calebyhan/CalebHan**
 
-# airlabs-ch
+# airlabs
 
 Python wrapper for [AirLabs](https://airlabs.co/).
 
 
 ## Installation
 ----------------------
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install currency-ch.
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install airlabs.
 
 ```bash
-pip install airlabs-ch
+pip install airlabs
 ```
 
 
 ## Usage
 ----------------------
 
 ```python
 import airlabs
 
-# converts amount of money from one currency to another
-currency.convert("usd", "eur", 1)
+# Gets airline information about American Airlines
+airlabs.airlines(iata_code="AA")
 
-# returns rate from one currency to another
-currency.rate("usd", "eur")
+# Gets information about real-time flights
+airlabs.flights()
 ```
 
 
 ## Documentation
 ----------------------
 
 ``currency.convert(input_currency, output_currency, amount, roundTo)``
```

