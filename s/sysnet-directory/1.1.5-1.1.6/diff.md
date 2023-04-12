# Comparing `tmp/sysnet-directory-1.1.5.tar.gz` & `tmp/sysnet-directory-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-directory-1.1.5.tar", last modified: Tue Mar 28 11:34:19 2023, max compression
+gzip compressed data, was "sysnet-directory-1.1.6.tar", last modified: Wed Apr 12 14:47:27 2023, max compression
```

## Comparing `sysnet-directory-1.1.5.tar` & `sysnet-directory-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 11:34:19.446245 sysnet-directory-1.1.5/
--rw-rw-rw-   0        0        0    12425 2022-12-10 17:50:43.000000 sysnet-directory-1.1.5/LICENSE.md
--rw-rw-rw-   0        0        0    19125 2023-03-28 11:34:19.446245 sysnet-directory-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2023-03-28 11:33:39.000000 sysnet-directory-1.1.5/README.md
--rw-rw-rw-   0        0        0      761 2023-03-28 11:33:39.000000 sysnet-directory-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-28 11:34:19.446245 sysnet-directory-1.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-28 11:34:19.421540 sysnet-directory-1.1.5/sysnet_directory/
--rw-rw-rw-   0        0        0        0 2022-12-07 11:26:06.000000 sysnet-directory-1.1.5/sysnet_directory/__init__.py
--rw-rw-rw-   0        0        0    15574 2023-03-28 11:33:39.000000 sysnet-directory-1.1.5/sysnet_directory/factory.py
-drwxrwxrwx   0        0        0        0 2023-03-28 11:34:19.427051 sysnet-directory-1.1.5/sysnet_directory.egg-info/
--rw-rw-rw-   0        0        0    19125 2023-03-28 11:34:19.000000 sysnet-directory-1.1.5/sysnet_directory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-03-28 11:34:19.000000 sysnet-directory-1.1.5/sysnet_directory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 11:34:19.000000 sysnet-directory-1.1.5/sysnet_directory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-28 11:34:19.000000 sysnet-directory-1.1.5/sysnet_directory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/
+-rw-rw-rw-   0        0        0    12425 2022-12-10 17:50:43.000000 sysnet-directory-1.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0    19125 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2023-03-28 11:33:39.000000 sysnet-directory-1.1.6/README.md
+-rw-rw-rw-   0        0        0      761 2023-04-12 14:46:27.000000 sysnet-directory-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.408621 sysnet-directory-1.1.6/sysnet_directory/
+-rw-rw-rw-   0        0        0        0 2022-12-07 11:26:06.000000 sysnet-directory-1.1.6/sysnet_directory/__init__.py
+-rw-rw-rw-   0        0        0    15648 2023-04-12 14:46:27.000000 sysnet-directory-1.1.6/sysnet_directory/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.408621 sysnet-directory-1.1.6/sysnet_directory.egg-info/
+-rw-rw-rw-   0        0        0    19125 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/top_level.txt
```

### Comparing `sysnet-directory-1.1.5/LICENSE.md` & `sysnet-directory-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sysnet-directory-1.1.5/PKG-INFO` & `sysnet-directory-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-directory
-Version: 1.1.5
+Version: 1.1.6
 Summary: Directory client library
 Author-email: Data Developer <info@sysnet.cz>
 License: # LICENCE PRO DOMÁCÍ POUŽITÍ (SYSNET Home Use License) v 1.0
         
         ## SHUL © SYSNET s.r.o. 2022
         
         <h4 style="text-align: center;">Tato komerční licence SYSNET s.r.o. se vztahuje na dílo (ve smyslu níže uvedených
```

### Comparing `sysnet-directory-1.1.5/README.md` & `sysnet-directory-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sysnet-directory-1.1.5/pyproject.toml` & `sysnet-directory-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-directory"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Directory client library"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-directory-1.1.5/sysnet_directory/factory.py` & `sysnet-directory-1.1.6/sysnet_directory/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
     member = []
     if 'memberOf' in user_item[1]:
         for it in user_item[1]['memberOf']:
             member.append(str(it, 'utf-8'))
     title = _get_item_value_string(user_item[1], 'title')
     name = _get_item_value_string(user_item[1], 'displayName')
     mail = _get_item_value_string(user_item[1], 'mail')
+    username = _get_item_value_string(user_item[1], 'sAMAccountName')
     first_name = _get_item_value_string(user_item[1], 'givenName')
     last_name = _get_item_value_string(user_item[1], 'sn')
     employee_id = _get_item_value_string(user_item[1], 'employeeNumber')
     is_head = _get_item_value_boolean(user_item[1], 'extensionAttribute2')
     head_ou = None
     division = []
     # organizace
@@ -299,15 +300,15 @@
         division.append(organization_level_3)
     degree = _get_item_value_string(user_item[1], 'extensionAttribute8')
     higher = ''
     if len(division) > 1:
         higher = division[-2]['code']
     org_info = {'is_head': is_head, 'ou': head_ou, 'higher_ou': higher}
     out = {
-        'dn': dn, 'member': member, 'title': title, 'name': name, 'username': mail, 'email': mail,
+        'dn': dn, 'member': member, 'title': title, 'name': name, 'username': username, 'email': mail,
         'first_name': first_name, 'last_name': last_name, 'degree': degree, 'division': division,
         'employee_id': employee_id, 'org_info': org_info
     }
     return out
 
 
 def _extract_org_structure(user_list):
```

### Comparing `sysnet-directory-1.1.5/sysnet_directory.egg-info/PKG-INFO` & `sysnet-directory-1.1.6/sysnet_directory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-directory
-Version: 1.1.5
+Version: 1.1.6
 Summary: Directory client library
 Author-email: Data Developer <info@sysnet.cz>
 License: # LICENCE PRO DOMÁCÍ POUŽITÍ (SYSNET Home Use License) v 1.0
         
         ## SHUL © SYSNET s.r.o. 2022
         
         <h4 style="text-align: center;">Tato komerční licence SYSNET s.r.o. se vztahuje na dílo (ve smyslu níže uvedených
```

