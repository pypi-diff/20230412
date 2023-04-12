# Comparing `tmp/cybereason-0.1.2.tar.gz` & `tmp/cybereason-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybereason-0.1.2.tar", last modified: Thu Mar 16 15:42:24 2023, max compression
+gzip compressed data, was "cybereason-0.1.3.tar", last modified: Wed Apr 12 17:41:57 2023, max compression
```

## Comparing `cybereason-0.1.2.tar` & `cybereason-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:24.189026 cybereason-0.1.2/
--rw-rw-rw-   0        0        0     1481 2023-03-16 14:32:48.000000 cybereason-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2986 2023-03-16 15:42:24.191036 cybereason-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1977 2023-03-16 15:42:24.194044 cybereason-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-03-16 14:32:48.000000 cybereason-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:23.443645 cybereason-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:23.982022 cybereason-0.1.2/src/cybereason/
--rw-rw-rw-   0        0        0      198 2023-03-16 14:58:23.000000 cybereason-0.1.2/src/cybereason/__init__.py
--rw-rw-rw-   0        0        0     3023 2023-03-16 15:38:34.000000 cybereason-0.1.2/src/cybereason/_patch.py
--rw-rw-rw-   0        0        0     1243 2023-03-16 15:01:25.000000 cybereason-0.1.2/src/cybereason/_typing.py
--rw-rw-rw-   0        0        0    15229 2023-03-16 15:31:09.000000 cybereason-0.1.2/src/cybereason/client.py
--rw-rw-rw-   0        0        0     2616 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/custom_rules.py
--rw-rw-rw-   0        0        0     3775 2023-03-16 14:53:41.000000 cybereason-0.1.2/src/cybereason/exceptions.py
--rw-rw-rw-   0        0        0     3483 2023-03-16 15:38:09.000000 cybereason-0.1.2/src/cybereason/incident_reponse.py
--rw-rw-rw-   0        0        0     5083 2023-03-16 15:31:32.000000 cybereason-0.1.2/src/cybereason/malops.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:24.125503 cybereason-0.1.2/src/cybereason/parse/
--rw-rw-rw-   0        0        0      147 2023-03-16 15:37:41.000000 cybereason-0.1.2/src/cybereason/parse/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/parse/cef.py
--rw-rw-rw-   0        0        0     2830 2023-03-16 15:33:56.000000 cybereason-0.1.2/src/cybereason/parse/server.py
--rw-rw-rw-   0        0        0        0 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/py.typed
--rw-rw-rw-   0        0        0    16746 2023-03-16 15:32:12.000000 cybereason-0.1.2/src/cybereason/sensors.py
--rw-rw-rw-   0        0        0     4477 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/system.py
--rw-rw-rw-   0        0        0     6370 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/threat_intel.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:24.179025 cybereason-0.1.2/src/cybereason/utils/
--rw-rw-rw-   0        0        0     2967 2023-03-16 15:34:48.000000 cybereason-0.1.2/src/cybereason/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-03-16 14:32:48.000000 cybereason-0.1.2/src/cybereason/utils/guid.py
-drwxrwxrwx   0        0        0        0 2023-03-16 15:42:24.078498 cybereason-0.1.2/src/cybereason.egg-info/
--rw-rw-rw-   0        0        0     2986 2023-03-16 15:42:21.000000 cybereason-0.1.2/src/cybereason.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-03-16 15:42:22.000000 cybereason-0.1.2/src/cybereason.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 15:42:21.000000 cybereason-0.1.2/src/cybereason.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-16 15:42:21.000000 cybereason-0.1.2/src/cybereason.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      181 2023-03-16 15:42:21.000000 cybereason-0.1.2/src/cybereason.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-16 15:42:21.000000 cybereason-0.1.2/src/cybereason.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.845063 cybereason-0.1.3/
+-rw-rw-rw-   0        0        0     1481 2023-04-12 17:30:28.000000 cybereason-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2986 2023-04-12 17:41:57.845063 cybereason-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-04-12 17:41:57.849074 cybereason-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-04-12 17:30:28.000000 cybereason-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.743979 cybereason-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.805167 cybereason-0.1.3/src/cybereason/
+-rw-rw-rw-   0        0        0      198 2023-04-12 17:32:03.000000 cybereason-0.1.3/src/cybereason/__init__.py
+-rw-rw-rw-   0        0        0     3023 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/_patch.py
+-rw-rw-rw-   0        0        0     1243 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/_typing.py
+-rw-rw-rw-   0        0        0    15392 2023-04-12 17:35:50.000000 cybereason-0.1.3/src/cybereason/client.py
+-rw-rw-rw-   0        0        0     2640 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/custom_rules.py
+-rw-rw-rw-   0        0        0     3775 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/exceptions.py
+-rw-rw-rw-   0        0        0     3531 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/incident_reponse.py
+-rw-rw-rw-   0        0        0     5212 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/malops.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.833578 cybereason-0.1.3/src/cybereason/parse/
+-rw-rw-rw-   0        0        0      147 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/cef.py
+-rw-rw-rw-   0        0        0     2846 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/server.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/py.typed
+-rw-rw-rw-   0        0        0    16783 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/sensors.py
+-rw-rw-rw-   0        0        0     4477 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/system.py
+-rw-rw-rw-   0        0        0     6444 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/threat_intel.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.841210 cybereason-0.1.3/src/cybereason/utils/
+-rw-rw-rw-   0        0        0     2967 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/utils/guid.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.822298 cybereason-0.1.3/src/cybereason.egg-info/
+-rw-rw-rw-   0        0        0     2986 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      229 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/top_level.txt
```

### Comparing `cybereason-0.1.2/LICENSE` & `cybereason-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/PKG-INFO` & `cybereason-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -87,8 +87,8 @@
             json.dump(logs, f, indent=4)
 
 asyncio.run(user_audit())
 ```
 
 ---
 
-Copyright &copy; 2021-2022 [Forensic & Security](https://forensic-security.com/)
+Copyright &copy; 2021-2023 [Forensic & Security](https://forensic-security.com/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.1.2 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.1.3 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
@@ -29,8 +29,8 @@
 ["name"]}.json' with open(filename, 'w') as f: json.dump(policy, f, indent=4)
 asyncio.run(dump_policies_config()) ``` ### Download and parse into JSON all
 user audit logs (action log) ```python from cybereason import Cybereason import
 asyncio import json async def user_audit(): async with Cybereason(, , ) as
 client: # rotated=False to get only the latest logs logs = [log async for log
 in client.get_user_audit_logs(rotated=True)] with open('user_audit.json', 'w')
 as f: json.dump(logs, f, indent=4) asyncio.run(user_audit()) ``` --- Copyright
-© 2021-2022 [Forensic & Security](https://forensic-security.com/)
+© 2021-2023 [Forensic & Security](https://forensic-security.com/)
```

### Comparing `cybereason-0.1.2/setup.cfg` & `cybereason-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -91,34 +91,40 @@
 000005a0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
 000005b0: 7265 7175 6972 655d 0d0a 7a69 7020 3d20  require]..zip = 
 000005c0: 0d0a 0970 797a 6970 7065 720d 0a73 6f63  ...pyzipper..soc
 000005d0: 6b73 203d 200d 0a09 6874 7470 782d 736f  ks = ...httpx-so
 000005e0: 636b 735b 6173 796e 6369 6f5d 0d0a 6465  cks[asyncio]..de
 000005f0: 7620 3d20 0d0a 096d 7970 790d 0a09 666c  v = ...mypy...fl
 00000600: 616b 6538 0d0a 0970 7974 6573 740d 0a09  ake8...pytest...
-00000610: 7079 7961 6d6c 0d0a 096a 736f 6e73 6368  pyyaml...jsonsch
-00000620: 656d 610d 0a09 7079 7465 7374 2d61 7379  ema...pytest-asy
-00000630: 6e63 696f 0d0a 0970 7974 6573 742d 6461  ncio...pytest-da
-00000640: 7461 6669 6c65 730d 0a64 6f63 7320 3d20  tafiles..docs = 
-00000650: 0d0a 0973 7068 696e 780d 0a09 7370 6869  ...sphinx...sphi
-00000660: 6e78 2d72 7464 2d74 6865 6d65 0d0a 0d0a  nx-rtd-theme....
-00000670: 5b66 6c61 6b65 385d 0d0a 6967 6e6f 7265  [flake8]..ignore
-00000680: 203d 2045 3232 312c 2045 3234 312c 2045   = E221, E241, E
-00000690: 3430 322c 2045 3733 310d 0a65 7863 6c75  402, E731..exclu
-000006a0: 6465 203d 200d 0a09 2e67 6974 2c0d 0a09  de = ....git,...
-000006b0: 5f5f 7079 6361 6368 655f 5f2c 0d0a 092e  __pycache__,....
-000006c0: 6d79 7079 5f63 6163 6865 2c0d 0a09 2e70  mypy_cache,....p
-000006d0: 7974 6573 745f 6361 6368 652c 0d0a 095f  ytest_cache,..._
-000006e0: 7479 7069 6e67 2e70 790d 0a69 6e6c 696e  typing.py..inlin
-000006f0: 652d 7175 6f74 6573 203d 2073 696e 676c  e-quotes = singl
-00000700: 650d 0a6d 6178 2d63 6f6d 706c 6578 6974  e..max-complexit
-00000710: 7920 3d20 3133 0d0a 6d61 782d 6c69 6e65  y = 13..max-line
-00000720: 2d6c 656e 6774 6820 3d20 3939 0d0a 6d75  -length = 99..mu
-00000730: 6c74 696c 696e 652d 7175 6f74 6573 203d  ltiline-quotes =
-00000740: 2073 696e 676c 650d 0a64 6f63 7374 7269   single..docstri
-00000750: 6e67 2d71 756f 7465 7320 3d20 7369 6e67  ng-quotes = sing
-00000760: 6c65 0d0a 0d0a 5b6d 7970 795d 0d0a 6967  le....[mypy]..ig
-00000770: 6e6f 7265 5f6d 6973 7369 6e67 5f69 6d70  nore_missing_imp
-00000780: 6f72 7473 203d 2054 7275 650d 0a0d 0a5b  orts = True....[
-00000790: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000007a0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000007b0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000610: 7079 7961 6d6c 0d0a 0970 7974 6573 742d  pyyaml...pytest-
+00000620: 6173 796e 6369 6f0d 0a09 7079 7465 7374  asyncio...pytest
+00000630: 2d64 6174 6166 696c 6573 0d0a 096a 736f  -datafiles...jso
+00000640: 6e73 6368 656d 610d 0a09 6671 646e 0d0a  nschema...fqdn..
+00000650: 0972 6663 3333 3339 2d76 616c 6964 6174  .rfc3339-validat
+00000660: 6f72 0d0a 0969 736f 6475 7261 7469 6f6e  or...isoduration
+00000670: 0d0a 0969 646e 610d 0a09 7266 6333 3938  ...idna...rfc398
+00000680: 370d 0a64 6f63 7320 3d20 0d0a 0973 7068  7..docs = ...sph
+00000690: 696e 780d 0a09 7370 6869 6e78 2d72 7464  inx...sphinx-rtd
+000006a0: 2d74 6865 6d65 0d0a 0d0a 5b66 6c61 6b65  -theme....[flake
+000006b0: 385d 0d0a 6967 6e6f 7265 203d 2045 3131  8]..ignore = E11
+000006c0: 352c 2045 3232 312c 2045 3234 312c 2045  5, E221, E241, E
+000006d0: 3430 322c 2045 3733 310d 0a65 7863 6c75  402, E731..exclu
+000006e0: 6465 203d 200d 0a09 2e67 6974 2c0d 0a09  de = ....git,...
+000006f0: 5f5f 7079 6361 6368 655f 5f2c 0d0a 092e  __pycache__,....
+00000700: 6d79 7079 5f63 6163 6865 2c0d 0a09 2e70  mypy_cache,....p
+00000710: 7974 6573 745f 6361 6368 652c 0d0a 092e  ytest_cache,....
+00000720: 7665 6e76 2c0d 0a09 6275 696c 642c 0d0a  venv,...build,..
+00000730: 0974 6573 742e 2a2c 0d0a 095f 7479 7069  .test.*,..._typi
+00000740: 6e67 2e70 790d 0a69 6e6c 696e 652d 7175  ng.py..inline-qu
+00000750: 6f74 6573 203d 2073 696e 676c 650d 0a6d  otes = single..m
+00000760: 6178 2d63 6f6d 706c 6578 6974 7920 3d20  ax-complexity = 
+00000770: 3133 0d0a 6d61 782d 6c69 6e65 2d6c 656e  13..max-line-len
+00000780: 6774 6820 3d20 3939 0d0a 6d75 6c74 696c  gth = 99..multil
+00000790: 696e 652d 7175 6f74 6573 203d 2073 696e  ine-quotes = sin
+000007a0: 676c 650d 0a64 6f63 7374 7269 6e67 2d71  gle..docstring-q
+000007b0: 756f 7465 7320 3d20 7369 6e67 6c65 0d0a  uotes = single..
+000007c0: 0d0a 5b6d 7970 795d 0d0a 6967 6e6f 7265  ..[mypy]..ignore
+000007d0: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
+000007e0: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
+000007f0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000800: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000810: 300d 0a0d 0a                             0....
```

### Comparing `cybereason-0.1.2/src/cybereason/_patch.py` & `cybereason-0.1.3/src/cybereason/_patch.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/_typing.py` & `cybereason-0.1.3/src/cybereason/_typing.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/client.py` & `cybereason-0.1.3/src/cybereason/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from io import BytesIO
 import logging
 
 # monkey-patch to allow multiple {'file-encoding': 'chunked'} headers
 import httpx
 from ._patch import normalize_and_validate
-httpx._transports.default.httpcore._async.http11.h11._headers.normalize_and_validate = normalize_and_validate
+httpx._transports.default.httpcore._async.http11.h11._headers.normalize_and_validate = normalize_and_validate  # noqa: E501
 from httpx import AsyncClient, HTTPStatusError, ConnectError
 
 from .exceptions import (
     AccessDenied, AuthenticationError, ResourceNotFoundError,
     UnauthorizedRequest, CybereasonException, ServerError, ClientError,
 )
 from .utils import get_filename, to_list
@@ -117,14 +117,17 @@
             resp = await self.session.post('login.html', data=auth, **options)  # type: ignore
         except ConnectError as e:
             raise ConnectionError(e) from None
 
         if 'error' in str(resp.url):
             await self.session.aclose()
             raise AuthenticationError('Invalid credentials')
+        elif 'reset' in str(resp.url):
+            await self.session.aclose()
+            raise AuthenticationError('Expired password')
 
         if 'Two factor authentication' in resp.text:
             if not self.totp_code:
                 await self.session.aclose()
                 raise AuthenticationError('TOTP code (2FA) is required')
 
             totp = {'totpCode': self.totp_code, 'submit': 'Login'}
@@ -154,14 +157,15 @@
     async def aclose(self) -> None:
         if 'session' in self.__dict__:
             await self.logout()
             await self.session.aclose()
         if 'session_sage' in self.__dict__:
             await self.session_sage.aclose()
 
+    @staticmethod
     async def gather_limit(num, *tasks):
         '''Limits concurrency.
 
         Args:
             num: max of simultaneous tasks.
         '''
         import asyncio
@@ -424,15 +428,15 @@
 
         _, archive = await self.raw_download('monitor/global/userAuditLog')
         async for content in extract_logfiles(archive, 'userAuditSyslog', rotated):
             # yield latest logs first
             for line in content.splitlines()[::-1]:
                 yield cefparse(line.decode())
 
-    # TODO: https://nest.cybereason.com/documentation/api-documentation/all-versions/how-build-queries
+    # https://nest.cybereason.com/documentation/api-documentation/all-versions/how-build-queries
     async def query(self, data: 'Dict[str, Any]') -> 'Dict[str, Any]':
         # default since version 20.1.381
         data.setdefault('perGroupLimit', 100)
         if data['perGroupLimit'] > 1000:
             data['perGroupLimit'] = 1000
 
         # log.debug('Running query %s', data)
```

### Comparing `cybereason-0.1.2/src/cybereason/custom_rules.py` & `cybereason-0.1.3/src/cybereason/custom_rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,61 +8,61 @@
 
 
 class CustomRulesMixin(CybereasonProtocol):
     # FIXME: breaks on 22.1
     async def get_active_custom_rules(self) -> 'List[Dict[str, Any]]':
         '''Retrieve a list of all active custom detection rules.
         '''
-        resp = await self.get('customRules/decisionFeature/live')
+        resp = await self.get('v2/customRules/decisionFeature/live')
         # TODO: resp['limitExceed']: bool ?
         return resp['rules']
 
     async def get_disabled_custom_rules(self) -> 'List[Dict[str, Any]]':
         '''Returns a list of all custom rules currently disabled in your
         environment.
         '''
-        return await self.get('customRules/decisionFeature/deleted')
+        return await self.get('v2/customRules/decisionFeature/deleted')
 
     async def get_root_causes(self) -> 'List[str]':
         '''Returns a list of all Elements you can use for a root cause
         for a Malop generated from this custom rule.
         '''
-        return await self.get('customRules/rootCauses')
+        return await self.get('v2/customRules/rootCauses')
 
     @authz('L3 Analyst')
     async def get_malop_detection_types(self) -> 'List[Dict[str, str]]':
         '''Returns a list of all available detection types you can use
         for custom detection rules.
         '''
-        return await self.get('customRules/getMalopDetectionTypes')
+        return await self.get('v2/customRules/getMalopDetectionTypes')
 
     @authz('L3 Analyst')
     async def get_malop_activity_types(self) -> 'List[Dict[str, str]]':
         '''Returns a list of all available Malop activity types you can
         use for custom detection rules.
         '''
-        return await self.get('customRules/getMalopActivityTypes')
+        return await self.get('v2/customRules/getMalopActivityTypes')
 
     # TODO
     async def create_custom_rule(self, data):
         '''Creates a custom detection rule.
 
         .. warning::
             Custom detection rules should be created only after adequate
             research regarding precision and coverage has been completed.
             Creating a custom detection rule that is not specific enough
             can have detrimental impact on retention and overall
             performance of the environment.
         '''
-        return await self.post('customRules/decisionFeature/create', data)
+        return await self.post('v2/customRules/decisionFeature/create', data)
 
     # TODO
     async def update_custom_rule(self, data):
         '''Updates an existing custom detection rule.
         '''
-        return await self.post('customRules/decisionFeature/update', data)
+        return await self.post('v2/customRules/decisionFeature/update', data)
 
     async def get_custom_rule_history(self, rule_id: int) -> 'List[Dict[str, Any]]':
-        resp = await self.get(f'customRules/history/{rule_id}')
+        resp = await self.get(f'v2/customRules/history/{rule_id}')
         if not resp['history']:
             raise ResourceNotFoundError(rule_id)
         return resp['history']
```

### Comparing `cybereason-0.1.2/src/cybereason/exceptions.py` & `cybereason-0.1.3/src/cybereason/exceptions.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/incident_reponse.py` & `cybereason-0.1.3/src/cybereason/incident_reponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,22 +52,22 @@
         }
 
         if platform:
             try:
                 _platform = dict(x86='ARCH_X86', x64='ARCH_AMD64')[platform]
             except KeyError:
                 raise ValueError("Platform must be 'x86' or 'x64'") from None
-            data['packageOSInfoList']['platform'] = _platform
+            data['packageOSInfoList']['platform'] = _platform  # type: ignore
 
         if run_command or output_dir:
             data['packageRunConfiguration'] = {}
             if run_command:
-                data['packageRunConfiguration']['runCommand'] = run_command
+                data['packageRunConfiguration']['runCommand'] = run_command  # type: ignore
             if output_dir:
-                data['packageRunConfiguration']['outputDir'] = output_dir
+                data['packageRunConfiguration']['outputDir'] = output_dir  # type: ignore
 
         try:
             package_info = 'file', open(filepath, 'rb'), 'application/octet-stream'
         except FileNotFoundError:
             raise ResourceNotFoundError(filepath) from None
         files = {'packageInfo': package_info}
```

### Comparing `cybereason-0.1.2/src/cybereason/malops.py` & `cybereason-0.1.3/src/cybereason/malops.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,26 @@
     Label = Dict[str, Union[str, int]]
 
 log = logging.getLogger(__name__)
 
 
 class MalopsMixin(CybereasonProtocol):
     async def get_malops(
-        self, start: 'Union[datetime, date]', end: 'Union[datetime, date]'
+        self,
+        start: 'Union[datetime, date]',
+        end:   'Union[datetime, date, None]' = None,
     ) -> 'List[Dict[str, Any]]':
         '''Retrieve all malops of all types between the given dates.
         '''
         if isinstance(start, date):
             start = datetime.combine(start, datetime.min.time())
-        if isinstance(end, date):
+
+        if end is None:
+            end = datetime.combine(date.today(), datetime.max.time())
+        elif isinstance(end, date):
             end = datetime.combine(end, datetime.max.time())
 
         if start.tzinfo is None:
             start = start.replace(tzinfo=timezone.utc)
         if end.tzinfo is None:
             end = end.replace(tzinfo=timezone.utc)
```

### Comparing `cybereason-0.1.2/src/cybereason/parse/cef.py` & `cybereason-0.1.3/src/cybereason/parse/cef.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/parse/server.py` & `cybereason-0.1.3/src/cybereason/parse/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         '''Returns the rotated logs in order.
         '''
         rotation = self.logs[logname].get('rotation')
         archives = sorted(list(self.folder.glob(f'{logname}[-.]*.log.gz')), reverse=True)
 
         if rotation == 'seq':
             ptrn = re.compile(r'(\d+)').search
-            sort = lambda x: int(ptrn(x.stem).group(0))
+            sort = lambda x: int(ptrn(x.stem).group(0))  # type: ignore
             archives = sorted(archives, key=sort, reverse=True)
 
         return archives
 
     @staticmethod
     def log_datetime(dt):
         fmt = '%Y-%m-%d %H:%M:%S,%f'
```

### Comparing `cybereason-0.1.2/src/cybereason/sensors.py` & `cybereason-0.1.3/src/cybereason/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Any, TYPE_CHECKING
+from typing import Optional, Union, Any, TYPE_CHECKING, cast
 from pathlib import Path
 from os import PathLike
 import logging
 import asyncio
 
 from .utils import to_list, unset, get_filename
 from .exceptions import (
     AccessDenied, ServerError, ClientError,
     ResourceExistsError, ResourceNotFoundError,
     authz, min_version,
 )
 from ._typing import CybereasonProtocol
 
 if TYPE_CHECKING:
-    from typing import AsyncIterator, Dict, List, Union
+    from typing import AsyncIterator, Dict, List
     from ._typing import SensorId
     from .utils import Unset
 
 
 log = logging.getLogger(__name__)
 
 
@@ -302,35 +302,35 @@
         device_type:    'Union[Unset, None, str]' = unset,
         critical_asset: 'Union[Unset, None, bool]' = unset,
         custom_tags:    'Union[Unset, None, str]' = unset,
     ) -> 'Dict[str, Dict[str, Union[str, bool]]]':
         '''Creates, modifies or delete tags for a specific sensor or
         group of sensors. To delete a tag set the value to ``None``.
         '''
-        tags: 'Dict[str, Union[str, bool]]' = dict()
+        ops: 'Dict[str, Dict[str, Union[str, bool]]]' = dict()
 
         for name, value, typ in (
             ('department',     department,     str),
             ('location',       location,       str),
             ('device type',    device_type,    str),
             ('critical asset', critical_asset, bool),
             ('custom tags',    custom_tags,    str),
         ):
             if value is not unset:
                 if value is None:
-                    tags[name] = {'operation': 'REMOVE'}
+                    ops[name] = {'operation': 'REMOVE'}
                 elif isinstance(value, typ):
                     if typ == str and len(value) > 100:  # type: ignore
-                        err = f'The maximum length for the {name!r} tag is 100 characters'
-                        raise ValueError(err)
-                    tags[name] = {'operation': 'SET', 'value': value}
+                        msg = f'The maximum length for the {name!r} tag is 100 characters'
+                        raise ValueError(msg)
+                    ops[name] = {'operation': 'SET', 'value': cast(Union[str, bool], value)}
                 else:
                     raise TypeError(f'{name!r} tag must be a {typ.__name__!r}')
 
-        data = {'entities': {pylum_id: {'tags': tags, 'entityType': 'MACHINE'}}}
+        data = {'entities': {pylum_id: {'tags': ops, 'entityType': 'MACHINE'}}}
         resp = await self.post('tagging/process_tags', data)
         resp = resp['entities'][pylum_id]['results']
 
         err = dict()
         for tag, result in resp.items():
             if not result['success']:
                 # ignore unsuccessful deletions of missing tags
```

### Comparing `cybereason-0.1.2/src/cybereason/system.py` & `cybereason-0.1.3/src/cybereason/system.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/threat_intel.py` & `cybereason-0.1.3/src/cybereason/threat_intel.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         '''Returns a list of all domain reputations used by the threat
         intelligence service.
         '''
         from warnings import warn
         warn("'get_domain_reputations' is deprecated", DeprecationWarning)
         return await self.post_sage('download_v1/domain_reputation', {})
 
+    # XXX: broken: commas not escaped, `None` and `` in boolean fields...
     async def get_reputations(
         self,
         reputation: 'Optional[str]' = None,
     ) -> 'AsyncIterator[Dict[str, Any]]':
         '''Returns a list of custom reputations for files, IP addresses,
         and domain names.
```

### Comparing `cybereason-0.1.2/src/cybereason/utils/__init__.py` & `cybereason-0.1.3/src/cybereason/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason/utils/guid.py` & `cybereason-0.1.3/src/cybereason/utils/guid.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.2/src/cybereason.egg-info/PKG-INFO` & `cybereason-0.1.3/src/cybereason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.1.2
+Version: 0.1.3
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -87,8 +87,8 @@
             json.dump(logs, f, indent=4)
 
 asyncio.run(user_audit())
 ```
 
 ---
 
-Copyright &copy; 2021-2022 [Forensic & Security](https://forensic-security.com/)
+Copyright &copy; 2021-2023 [Forensic & Security](https://forensic-security.com/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.1.2 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.1.3 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
@@ -29,8 +29,8 @@
 ["name"]}.json' with open(filename, 'w') as f: json.dump(policy, f, indent=4)
 asyncio.run(dump_policies_config()) ``` ### Download and parse into JSON all
 user audit logs (action log) ```python from cybereason import Cybereason import
 asyncio import json async def user_audit(): async with Cybereason(, , ) as
 client: # rotated=False to get only the latest logs logs = [log async for log
 in client.get_user_audit_logs(rotated=True)] with open('user_audit.json', 'w')
 as f: json.dump(logs, f, indent=4) asyncio.run(user_audit()) ``` --- Copyright
-© 2021-2022 [Forensic & Security](https://forensic-security.com/)
+© 2021-2023 [Forensic & Security](https://forensic-security.com/)
```

### Comparing `cybereason-0.1.2/src/cybereason.egg-info/SOURCES.txt` & `cybereason-0.1.3/src/cybereason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

