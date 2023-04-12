# Comparing `tmp/gnuhealth-all-modules-4.2.0.tar.gz` & `tmp/gnuhealth-all-modules-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnuhealth-all-modules-4.2.0.tar", last modified: Tue Feb 14 14:23:25 2023, max compression
+gzip compressed data, was "gnuhealth-all-modules-4.2.1.tar", last modified: Wed Apr 12 13:55:58 2023, max compression
```

## Comparing `gnuhealth-all-modules-4.2.0.tar` & `gnuhealth-all-modules-4.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/
--rw-rw-r--   0 wiese     (1001) wiese     (1001)    34431 2022-06-01 11:28:43.000000 gnuhealth-all-modules-4.2.0/LICENSE.txt
--rw-rw-r--   0 wiese     (1001) wiese     (1001)       55 2022-11-17 16:53:27.000000 gnuhealth-all-modules-4.2.0/MANIFEST.in
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     2441 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/PKG-INFO
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     1435 2023-02-14 14:18:27.000000 gnuhealth-all-modules-4.2.0/README.rst
-drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/
-drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/
--rw-rw-r--   0 wiese     (1001) wiese     (1001)      311 2022-11-16 22:05:13.000000 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/gnuhealth.service
--rw-rw-r--   0 wiese     (1001) wiese     (1001)      459 2022-11-16 22:02:33.000000 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/gnuhealth_log.conf
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     1177 2022-11-16 23:26:27.000000 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/reverse_proxy.conf
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     8071 2022-11-16 22:03:49.000000 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/trytond.conf
--rw-rw-r--   0 wiese     (1001) wiese     (1001)      625 2022-11-16 22:12:16.000000 gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/uwsgi_trytond.ini
-drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     2441 2023-02-14 14:23:25.000000 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/PKG-INFO
--rw-rw-r--   0 wiese     (1001) wiese     (1001)      510 2023-02-14 14:23:25.000000 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/SOURCES.txt
--rw-rw-r--   0 wiese     (1001) wiese     (1001)        1 2023-02-14 14:23:25.000000 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/dependency_links.txt
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     1862 2023-02-14 14:23:25.000000 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/requires.txt
--rw-rw-r--   0 wiese     (1001) wiese     (1001)       22 2023-02-14 14:23:25.000000 gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/top_level.txt
--rw-rw-r--   0 wiese     (1001) wiese     (1001)       85 2022-06-01 11:38:07.000000 gnuhealth-all-modules-4.2.0/pyproject.toml
--rw-rw-r--   0 wiese     (1001) wiese     (1001)       38 2023-02-14 14:23:25.204021 gnuhealth-all-modules-4.2.0/setup.cfg
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     2096 2023-02-14 14:21:32.000000 gnuhealth-all-modules-4.2.0/setup.py
--rw-rw-r--   0 wiese     (1001) wiese     (1001)     1798 2023-02-14 14:21:44.000000 gnuhealth-all-modules-4.2.0/tryton.cfg
+drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-04-12 13:55:58.290732 gnuhealth-all-modules-4.2.1/
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)    34431 2022-06-01 11:28:43.000000 gnuhealth-all-modules-4.2.1/LICENSE.txt
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)       55 2022-11-17 16:53:27.000000 gnuhealth-all-modules-4.2.1/MANIFEST.in
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     2443 2023-04-12 13:55:58.290732 gnuhealth-all-modules-4.2.1/PKG-INFO
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     1437 2023-02-14 15:14:31.000000 gnuhealth-all-modules-4.2.1/README.rst
+drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-04-12 13:55:58.286732 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/
+drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-04-12 13:55:58.290732 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)      311 2022-11-16 22:05:13.000000 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/gnuhealth.service
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)      459 2022-11-16 22:02:33.000000 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/gnuhealth_log.conf
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     1177 2022-11-16 23:26:27.000000 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/reverse_proxy.conf
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     8071 2022-11-16 22:03:49.000000 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/trytond.conf
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)      625 2022-11-16 22:12:16.000000 gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/uwsgi_trytond.ini
+drwxrwxr-x   0 wiese     (1001) wiese     (1001)        0 2023-04-12 13:55:58.290732 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     2443 2023-04-12 13:55:58.000000 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/PKG-INFO
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)      510 2023-04-12 13:55:58.000000 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)        1 2023-04-12 13:55:58.000000 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     1862 2023-04-12 13:55:58.000000 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/requires.txt
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)       22 2023-04-12 13:55:58.000000 gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/top_level.txt
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)       85 2022-06-01 11:38:07.000000 gnuhealth-all-modules-4.2.1/pyproject.toml
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)       38 2023-04-12 13:55:58.290732 gnuhealth-all-modules-4.2.1/setup.cfg
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     2096 2023-04-12 13:51:17.000000 gnuhealth-all-modules-4.2.1/setup.py
+-rw-rw-r--   0 wiese     (1001) wiese     (1001)     1798 2023-04-12 13:52:50.000000 gnuhealth-all-modules-4.2.1/tryton.cfg
```

### Comparing `gnuhealth-all-modules-4.2.0/LICENSE.txt` & `gnuhealth-all-modules-4.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gnuhealth-all-modules-4.2.0/PKG-INFO` & `gnuhealth-all-modules-4.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnuhealth-all-modules
-Version: 4.2.0
+Version: 4.2.1
 Summary: GNU Health HMIS: Hospital Management Information System
 Home-page: https://www.gnuhealth.org
 Author: GNU Solidario
 Author-email: health@gnusolidario.org
 License: GPLv3+
 Project-URL: Homepage, https://www.gnuhealth.org/
 Project-URL: Source Code, https://gitlab.com/geraldwiese/gnu-health-all-modules-pypi
@@ -43,15 +43,17 @@
 
 You can find configuration templates in gnuhealth-all-modules/etc. They will be shipped during installation as well.
 After installation the folder can be located by running 'pip3 show gnuhealth-all-modules'.
 
 Check 'HOWTO' for informations on packaging, using testpypi, signatures and hashes.
 
 This content is available both on PyPI and on GitLab in case you want to double check the integrity:
+
 https://pypi.org/project/gnuhealth-all-modules/
+
 https://gitlab.com/geraldwiese/gnu-health-all-modules-pypi
 
 Further reading:
 
 GNU Health core package
 https://pypi.org/project/gnuhealth/
```

### Comparing `gnuhealth-all-modules-4.2.0/README.rst` & `gnuhealth-all-modules-4.2.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
 You can find configuration templates in gnuhealth-all-modules/etc. They will be shipped during installation as well.
 After installation the folder can be located by running 'pip3 show gnuhealth-all-modules'.
 
 Check 'HOWTO' for informations on packaging, using testpypi, signatures and hashes.
 
 This content is available both on PyPI and on GitLab in case you want to double check the integrity:
+
 https://pypi.org/project/gnuhealth-all-modules/
+
 https://gitlab.com/geraldwiese/gnu-health-all-modules-pypi
 
 Further reading:
 
 GNU Health core package
 https://pypi.org/project/gnuhealth/
```

### Comparing `gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/reverse_proxy.conf` & `gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/reverse_proxy.conf`

 * *Files identical despite different names*

### Comparing `gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/trytond.conf` & `gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/trytond.conf`

 * *Files identical despite different names*

### Comparing `gnuhealth-all-modules-4.2.0/gnuhealth-all-modules/etc/uwsgi_trytond.ini` & `gnuhealth-all-modules-4.2.1/gnuhealth-all-modules/etc/uwsgi_trytond.ini`

 * *Files identical despite different names*

### Comparing `gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/PKG-INFO` & `gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnuhealth-all-modules
-Version: 4.2.0
+Version: 4.2.1
 Summary: GNU Health HMIS: Hospital Management Information System
 Home-page: https://www.gnuhealth.org
 Author: GNU Solidario
 Author-email: health@gnusolidario.org
 License: GPLv3+
 Project-URL: Homepage, https://www.gnuhealth.org/
 Project-URL: Source Code, https://gitlab.com/geraldwiese/gnu-health-all-modules-pypi
@@ -43,15 +43,17 @@
 
 You can find configuration templates in gnuhealth-all-modules/etc. They will be shipped during installation as well.
 After installation the folder can be located by running 'pip3 show gnuhealth-all-modules'.
 
 Check 'HOWTO' for informations on packaging, using testpypi, signatures and hashes.
 
 This content is available both on PyPI and on GitLab in case you want to double check the integrity:
+
 https://pypi.org/project/gnuhealth-all-modules/
+
 https://gitlab.com/geraldwiese/gnu-health-all-modules-pypi
 
 Further reading:
 
 GNU Health core package
 https://pypi.org/project/gnuhealth/
```

### Comparing `gnuhealth-all-modules-4.2.0/gnuhealth_all_modules.egg-info/requires.txt` & `gnuhealth-all-modules-4.2.1/gnuhealth_all_modules.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,62 +9,62 @@
 trytond-product<6.1,>=6.0
 trytond-purchase<6.1,>=6.0
 trytond-purchase-request<6.1,>=6.0
 trytond-stock<6.1,>=6.0
 trytond-stock-lot<6.1,>=6.0
 trytond-stock-supply<6.1,>=6.0
 proteus<6.1,>=6.0
-gnuhealth-archives==4.2.0
-gnuhealth-caldav==4.2.0
-gnuhealth-calendar==4.2.0
-gnuhealth-contact-tracing==4.2.0
-gnuhealth-crypto==4.2.0
-gnuhealth-crypto-lab==4.2.0
-gnuhealth-dentistry==4.2.0
-gnuhealth-disability==4.2.0
-gnuhealth-ems==4.2.0
-gnuhealth-federation==4.2.0
-gnuhealth-genetics==4.2.0
-gnuhealth-genetics-uniprot==4.2.0
-gnuhealth-gyneco==4.2.0
-gnuhealth-history==4.2.0
-gnuhealth-icd10==4.2.0
-gnuhealth-icd10pcs==4.2.0
-gnuhealth-icd11==4.2.0
-gnuhealth-icd9procs==4.2.0
-gnuhealth-icpm==4.2.0
-gnuhealth-icu==4.2.0
-gnuhealth-imaging==4.2.0
-gnuhealth-inpatient==4.2.0
-gnuhealth-inpatient-calendar==4.2.0
-gnuhealth-insurance==4.2.0
-gnuhealth-iss==4.2.0
-gnuhealth-lab==4.2.0
-gnuhealth-lifestyle==4.2.0
-gnuhealth-mdg6==4.2.0
-gnuhealth-ntd==4.2.0
-gnuhealth-ntd-chagas==4.2.0
-gnuhealth-ntd-dengue==4.2.0
-gnuhealth-nursing==4.2.0
-gnuhealth-ophthalmology==4.2.0
-gnuhealth-orthanc==4.2.0
-gnuhealth-pediatrics==4.2.0
-gnuhealth-pediatrics-growth-charts==4.2.0
-gnuhealth-pediatrics-growth-charts-who==4.2.0
-gnuhealth-profile==4.2.0
-gnuhealth-qrcodes==4.2.0
-gnuhealth-reporting==4.2.0
-gnuhealth-services==4.2.0
-gnuhealth-services-imaging==4.2.0
-gnuhealth-services-lab==4.2.0
-gnuhealth-socioeconomics==4.2.0
-gnuhealth-stock==4.2.0
-gnuhealth-surgery==4.2.0
-gnuhealth-webdav3-server==4.2.0
-gnuhealth-who-essential-medicines==4.2.0
+gnuhealth-archives==4.2.1
+gnuhealth-caldav==4.2.1
+gnuhealth-calendar==4.2.1
+gnuhealth-contact-tracing==4.2.1
+gnuhealth-crypto==4.2.1
+gnuhealth-crypto-lab==4.2.1
+gnuhealth-dentistry==4.2.1
+gnuhealth-disability==4.2.1
+gnuhealth-ems==4.2.1
+gnuhealth-federation==4.2.1
+gnuhealth-genetics==4.2.1
+gnuhealth-genetics-uniprot==4.2.1
+gnuhealth-gyneco==4.2.1
+gnuhealth-history==4.2.1
+gnuhealth-icd10==4.2.1
+gnuhealth-icd10pcs==4.2.1
+gnuhealth-icd11==4.2.1
+gnuhealth-icd9procs==4.2.1
+gnuhealth-icpm==4.2.1
+gnuhealth-icu==4.2.1
+gnuhealth-imaging==4.2.1
+gnuhealth-inpatient==4.2.1
+gnuhealth-inpatient-calendar==4.2.1
+gnuhealth-insurance==4.2.1
+gnuhealth-iss==4.2.1
+gnuhealth-lab==4.2.1
+gnuhealth-lifestyle==4.2.1
+gnuhealth-mdg6==4.2.1
+gnuhealth-ntd==4.2.1
+gnuhealth-ntd-chagas==4.2.1
+gnuhealth-ntd-dengue==4.2.1
+gnuhealth-nursing==4.2.1
+gnuhealth-ophthalmology==4.2.1
+gnuhealth-orthanc==4.2.1
+gnuhealth-pediatrics==4.2.1
+gnuhealth-pediatrics-growth-charts==4.2.1
+gnuhealth-pediatrics-growth-charts-who==4.2.1
+gnuhealth-profile==4.2.1
+gnuhealth-qrcodes==4.2.1
+gnuhealth-reporting==4.2.1
+gnuhealth-services==4.2.1
+gnuhealth-services-imaging==4.2.1
+gnuhealth-services-lab==4.2.1
+gnuhealth-socioeconomics==4.2.1
+gnuhealth-stock==4.2.1
+gnuhealth-surgery==4.2.1
+gnuhealth-webdav3-server==4.2.1
+gnuhealth-who-essential-medicines==4.2.1
 psycopg2
 psycopg2cffi
 matplotlib
 qrcode
 barcode
 vobject
 bcrypt
```

### Comparing `gnuhealth-all-modules-4.2.0/setup.py` & `gnuhealth-all-modules-4.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     requires.append('%s>=%s,<%s' % (dep, deps_dict.get('trytond_version'), deps_dict.get('trytond_smaller')))
 for dep in deps_dict.get('depends_gnuhealth', []):
     requires.append('%s==%s' % (dep, deps_dict.get('gnuhealth_version')))
 for dep in deps_dict.get('depends_pip', []):
     requires.append(dep)
 setup(
     name='gnuhealth-all-modules',
-    version='4.2.0',
+    version='4.2.1',
     description='GNU Health HMIS: Hospital Management Information System',
     long_description=read('README.rst'),
     author='GNU Solidario',
     author_email='health@gnusolidario.org',
     url='https://www.gnuhealth.org',
     project_urls = {
       'Homepage': 'https://www.gnuhealth.org/',
```

### Comparing `gnuhealth-all-modules-4.2.0/tryton.cfg` & `gnuhealth-all-modules-4.2.1/tryton.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tryton]
-gnuhealth_version=4.2.0
+gnuhealth_version=4.2.1
 trytond_version=6.0
 trytond_smaller=6.1
 depends_trytond:
     trytond-account
     trytond-account-invoice
     trytond-account-invoice-stock
     trytond-account-product
```

