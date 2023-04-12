# Comparing `tmp/smartkey_cli-4.8.2070-py2.py3-none-any.whl.zip` & `tmp/smartkey_cli-4.9.2084-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 29325 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        9 b- defN 22-Jul-06 16:53 sdkms_cli/VERSION
--rw-rw-r--  2.0 unx        0 b- defN 22-Jul-06 16:53 sdkms_cli/__init__.py
--rw-rw-r--  2.0 unx   172130 b- defN 22-Jul-06 16:53 sdkms_cli/__main__.py
--rw-rw-r--  2.0 unx     2211 b- defN 22-Jul-06 16:53 sdkms_cli/pycompatible.py
--rw-rw-r--  2.0 unx     1041 b- defN 22-Jul-06 16:53 smartkey_cli-4.8.2070.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 22-Jul-06 16:53 smartkey_cli-4.8.2070.dist-info/WHEEL
--rw-rw-r--  2.0 unx       58 b- defN 22-Jul-06 16:53 smartkey_cli-4.8.2070.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 22-Jul-06 16:53 smartkey_cli-4.8.2070.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      742 b- defN 22-Jul-06 16:53 smartkey_cli-4.8.2070.dist-info/RECORD
-9 files, 176311 bytes uncompressed, 28035 bytes compressed:  84.1%
+Zip file size: 30373 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        9 b- defN 22-Aug-05 08:06 sdkms_cli/VERSION
+-rw-rw-r--  2.0 unx        0 b- defN 22-Aug-05 08:06 sdkms_cli/__init__.py
+-rw-rw-r--  2.0 unx   177944 b- defN 22-Aug-05 08:06 sdkms_cli/__main__.py
+-rw-rw-r--  2.0 unx     2211 b- defN 22-Aug-05 08:06 sdkms_cli/pycompatible.py
+-rw-rw-r--  2.0 unx     1041 b- defN 22-Aug-05 08:06 smartkey_cli-4.9.2084.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Aug-05 08:06 smartkey_cli-4.9.2084.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       58 b- defN 22-Aug-05 08:06 smartkey_cli-4.9.2084.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 22-Aug-05 08:06 smartkey_cli-4.9.2084.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      741 b- defN 22-Aug-05 08:06 smartkey_cli-4.9.2084.dist-info/RECORD
+9 files, 182106 bytes uncompressed, 29083 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sdkms_cli/__main__.py
 Comment: 
 
 Filename: sdkms_cli/pycompatible.py
 Comment: 
 
-Filename: smartkey_cli-4.8.2070.dist-info/METADATA
+Filename: smartkey_cli-4.9.2084.dist-info/METADATA
 Comment: 
 
-Filename: smartkey_cli-4.8.2070.dist-info/WHEEL
+Filename: smartkey_cli-4.9.2084.dist-info/WHEEL
 Comment: 
 
-Filename: smartkey_cli-4.8.2070.dist-info/entry_points.txt
+Filename: smartkey_cli-4.9.2084.dist-info/entry_points.txt
 Comment: 
 
-Filename: smartkey_cli-4.8.2070.dist-info/top_level.txt
+Filename: smartkey_cli-4.9.2084.dist-info/top_level.txt
 Comment: 
 
-Filename: smartkey_cli-4.8.2070.dist-info/RECORD
+Filename: smartkey_cli-4.9.2084.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sdkms_cli/VERSION

```diff
@@ -1 +1 @@
-4.8.2070
+4.9.2084
```

## sdkms_cli/__main__.py

```diff
@@ -7,14 +7,15 @@
 import re
 import os.path
 import sdkms.v1
 import argparse
 import textwrap
 import requests
 import warnings
+import sys
 import traceback
 import textwrap
 import time
 
 from os.path import expanduser
 from getpass import getpass
 from six.moves import http_client, input
@@ -725,16 +726,16 @@
     f.close()
 
 def process_custom_metadata(kwargs):
     if kwargs['custom_metadata'] is not None:
         metadata = json.loads(kwargs['custom_metadata'])
         if not isinstance(metadata, dict):
             raise ClientException('--custom_metadata should be a JSON object ' +
-                                  'e.g. --custom_metadata \'{ "key" = "value" }\'')
-        for key in metadata.keys():
+                                  'e.g. --custom_metadata \'{ "key" : "value" }\'')
+        for key in metadata:
             if not isinstance(metadata[key], string_types):
                 raise ClientException('Value for custom metadata key "{}" must be of type string'.format(key))
         kwargs['custom_metadata'] = metadata
 
 
 def default_ops_for_object(obj_type):
     """
@@ -830,45 +831,46 @@
     request = SobjectRequest(**kwargs)
     # Generic method to make request
     res = make_request(RequiredAuth.EITHER, SecurityObjectsApi, SecurityObjectsApi.rotate_security_object, request)
     if res.kid is not None:
         print("{}".format(res.kid))
 
 def import_key(key_file, **kwargs):
-    process_custom_metadata(kwargs)
-
-    in_key = _read_binary(key_file)
-
-    if kwargs['der']:
-        kwargs['value'] = to_byte_array(in_key)
-    else:
-        if kwargs['obj_type'].upper() in ('RSA', 'EC'):
-            # It is EC or RSA in PEM format
-            # remove PEM related tags if any
-            # for python3: decode in_key as string, because file is opened as rb
-            in_key = in_key.decode()
-            in_key = [x for x in in_key.split(os.linesep) if not x.startswith('-----')]
-            in_key = "".join(in_key)
-            kwargs['value'] = to_byte_array(b64_decode(in_key))
+    if not isinstance(key_file, bytes) or type(key_file)==str:
+        process_custom_metadata(kwargs)
+        in_key = _read_binary(key_file)
+        if kwargs['der']:
+            kwargs['value'] = to_byte_array(in_key)
         else:
-            kwargs['value'] = to_byte_array(hex_decode(in_key))
+            if kwargs['obj_type'].upper() in ('RSA', 'EC'):
+                # It is EC or RSA in PEM format
+                # remove PEM related tags if any
+                # for python3: decode in_key as string, because file is opened as rb
+                in_key = in_key.decode()
+                in_key = [x for x in in_key.split(os.linesep) if not x.startswith('-----')]
+                in_key = "".join(in_key)
+                kwargs['value'] = to_byte_array(b64_decode(in_key))
+            else:
+                kwargs['value'] = to_byte_array(hex_decode(in_key))
+    else:
+        kwargs['value'] = to_byte_array(key_file)
 
     operations = default_ops_for_object(kwargs['obj_type'])
     if kwargs['exportable']:
         operations.append('EXPORT')
         # warn user if exportable is given for AES,DES,DES3 or RSA and EC keys
         # f is for force
         if kwargs['obj_type'].upper() in SECURITY_ALGO and not kwargs['force']:
             print('Do you want to make security object exportable')
             flag = input("This can be security hazard (Y/N):")
             if flag.upper() != 'Y':
                 print('Aborting the key creation')
                 return
     if kwargs['key_ops']:
-        list =kwargs['key_ops'].split(",")
+        list = kwargs['key_ops'].split(",")
         for ops in list:
             operations.append(ops)
 
     del kwargs['exportable']
     del kwargs['force']
     kwargs['key_ops'] = operations
     kwargs['elliptic_curve'] = kwargs["ec_curve"]
@@ -880,32 +882,97 @@
     response = make_request(RequiredAuth.EITHER, SecurityObjectsApi, SecurityObjectsApi.import_security_object,
                             request)
 
     print("{}".format(response.kid))
 
 
 def import_cert(cert_file, **kwargs):
-    process_custom_metadata(kwargs)
-    kwargs['value'] = _read_binary(cert_file)
-    if not kwargs['der']:
-        # simple check to make sure that non der (pem) certificate has required BEGIN TAG
-        # There is no check if der format is selected
-        if b'-----BEGIN' not in kwargs['value']:
-            raise ClientException("Not a valid certificate. The certificate need to have BEGIN and END tag.")
+    if not isinstance(cert_file, bytes) or type(cert_file)==str:
+        process_custom_metadata(kwargs)
+        kwargs['value'] = _read_binary(cert_file)
+        if kwargs['der']: # DER data handling
+            kwargs['value'] = to_byte_array(kwargs['value'])
+        else:
+            # PEM Data handling
+            if b'-----BEGIN' not in kwargs['value']:
+                raise ClientException("Not a valid certificate. The certificate need to have BEGIN and END tag.")
+            in_cert = kwargs['value'].decode()
+            in_cert = [x for x in in_cert.split(os.linesep) if not x.startswith('-----')]
+            in_cert = "".join(in_cert)
+            kwargs['value'] = to_byte_array(b64_decode(in_cert))
+    else:
+        # cert_file here is binary data from import_pfx
+        # It's just easier to re-use the variable name
+        kwargs['value'] = to_byte_array(cert_file)
 
-    kwargs['value'] = to_byte_array(kwargs['value'])
-    kwargs['obj_type'] = 'OPAQUE'
+    kwargs['obj_type'] = 'CERTIFICATE'
     del kwargs['der']
 
     request = SobjectRequest(**kwargs)
     response = make_request(RequiredAuth.EITHER, SecurityObjectsApi, SecurityObjectsApi.import_security_object,
                             request)
     print("{}".format(response.kid))
 
 
+def import_pfx(pfx_file, password=None, **kwargs):
+    # Special import requirements for PFX, requires Python3.6+ ###
+    MIN_PYTHON = (3, 6)
+    assert sys.version_info >= MIN_PYTHON, "requires Python %s or newer" % '.'.join([str(n) for n in MIN_PYTHON])
+    ###############################################################
+    from cryptography.hazmat.primitives.serialization import pkcs12
+    from cryptography.hazmat.primitives import serialization
+    process_custom_metadata(kwargs)
+    pfx = open(pfx_file, 'rb').read()
+
+    p12 = serialization.pkcs12.load_pkcs12(pfx,str(password).encode('utf-8')) \
+            if password else serialization.pkcs12.load_pkcs12(pfx,b'')
+
+    pkey = p12.key.private_bytes(encoding=serialization.Encoding.DER,
+                                 format=serialization.PrivateFormat.PKCS8,
+                                 encryption_algorithm=serialization.NoEncryption())
+    certificate_index=0
+    cert = p12.cert._cert.public_bytes(serialization.Encoding.DER)
+    additional_certs = [x._cert.public_bytes(serialization.Encoding.DER) \
+                        for x in p12.additional_certs if x != p12.cert]
+    # Build custom_metadata
+    dict_of_certs = {"certificate0": cert}
+    dict_of_certs.update({"certificate%d" % (i+1) : \
+        additional_certs[i] for i in range(len(additional_certs))})
+
+    og_name = kwargs['name']
+    og_name+"_cert_"+str(certificate_index)
+
+    # Defining missing kwargs
+    kwargs['der']=False
+    kwargs['name']=og_name+"_pkey"
+    kwargs['obj_type']=kwargs['key_type']
+    # Update custom_metadata
+    kwargs['custom_metadata'] = kwargs['custom_metadata'].update(dict_of_certs) \
+                                      if kwargs['custom_metadata'] else None
+    del kwargs['key_type']
+    print("Importing PKey from PFX file to DSM:")
+    print(kwargs)
+    import_key(pkey, **kwargs)
+    del kwargs['exportable']
+    del kwargs['key_ops']
+    del kwargs['force']
+    del kwargs['ec_curve']
+
+    kwargs['obj_type']="CERTIFICATE"
+    kwargs['name']=og_name+"_cert_"+str(certificate_index)
+    print("Importing Certificate (%s) from PFX file to DSM:" % certificate_index)
+    import_cert(cert, **kwargs)
+
+    for cert in additional_certs:
+        certificate_index+=1
+        print("Importing Additional Certificate (%s) from PFX file to DSM:" % certificate_index)
+        kwargs['name']=og_name+"_cert_"+str(certificate_index)
+        import_cert(cert, **kwargs)
+
+
 def import_secret(secret_file, **kwargs):
     process_custom_metadata(kwargs)
     # using regular expression to remove auto added '\n' char by f.read() method
     secret = _read_binary(secret_file).decode()
     kwargs['value'] = to_byte_array(to_bytes(re.sub(os.linesep + r'\Z', '', secret)))
     # imported secret is exportable
     kwargs['key_ops'] = ['EXPORT', 'APPMANAGEABLE']
@@ -2601,14 +2668,51 @@
                                    action='store_true')
     parser_import_cert.set_defaults(func=import_cert)
     parser_import_cert.add_argument("--custom_metadata", help="""
                                         A JSON object encoding custom metadata for the unwrapped Security Object
                                         as "key" : "value" pairs. Values must be strings (and not integers,
                                         booleans or objects).
                                     """)
+
+    # Parser to support pfx import
+    parser_import_pfx = subparsers.add_parser("import-pfx", help="import a pfx secret",
+                                               formatter_class=argparse.RawDescriptionHelpFormatter,
+                                               epilog=textwrap.dedent('''\
+                                                  Output:
+                                                    1) UUID of disected Pkey from PFX on console.
+                                                    2) UUID of disected Certificate from PFX on console.
+                                                    3) UUID of any additional Certs from PFX on console.
+
+                                                  Exit Status:
+                                                    Zero on success and 1 on error. Error message is printed on stderr.
+                                                        ''')
+                                               )
+
+    _add_version(parser_import_pfx)
+    parser_import_pfx.add_argument("--in", help="Input PFX file path", required=True, dest="pfx_file")
+    parser_import_pfx.add_argument("--key-type", help="Type of key inside PFX file: EC or RSA.", required=True)
+    parser_import_pfx.add_argument("--name", help="Base Name of extracted PFX files", required=True)
+    parser_import_pfx.add_argument("--password", help="PFX password", required=False, dest="password")
+    parser_import_pfx.add_argument("--description", help="Description of certificate",
+                                    default="Created by sdkms-client")
+    parser_import_pfx.add_argument("--ec-curve", help="Elliptic curve name. Required for --key-type EC"
+                                " Supported curve are SecP192K1, SecP224K1, SecP256K1, NistP192, NistP224, NistP256, NistP384, NistP521")
+    parser_import_pfx.add_argument("--group-id", help="Security Group for this key")
+    parser_import_pfx.add_argument("--exportable", help="Allow key to be exported from SDKMS by wrapping",
+                                   action='store_true')
+    parser_import_pfx.add_argument("-f", "--force", help="Force key to be exportable",
+                               action="store_true")
+    parser_import_pfx.add_argument("--key-ops", help="Allowed key operations. Comma separated list of operations")
+    parser_import_pfx.set_defaults(func=import_pfx)
+    parser_import_pfx.add_argument("--custom_metadata", help="""
+                                        A JSON object encoding custom metadata for the unwrapped Security Object
+                                        as "key" : "value" pairs. Values must be strings (and not integers,
+                                        booleans or objects).
+                                    """)
+
     # Parser to support secret import
     parser_import_secret = subparsers.add_parser("import-secret", help="Import a secret into SDKMS",
                                                  formatter_class=argparse.RawDescriptionHelpFormatter,
                                                  epilog=textwrap.dedent('''\
                                                   Output:
                                                     Key UUID of imported secret on console.
```

## Comparing `smartkey_cli-4.8.2070.dist-info/METADATA` & `smartkey_cli-4.9.2084.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartkey-cli
-Version: 4.8.2070
+Version: 4.9.2084
 Summary: Equinix Smartkey CLI
 Home-page: https://support.smartkey.io
 Author: Equinix
 Author-email: support@equinix.com
 License: Apache 2.0
 Keywords: CLI,Equinix Smartkey,Fortanix
 Platform: UNKNOWN
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: argparse (==1.4.0)
 Requires-Dist: requests (==2.18.4)
-Requires-Dist: sdkms (==4.8.2070)
+Requires-Dist: sdkms (==4.9.2084)
 Requires-Dist: six (==1.11.0)
 Requires-Dist: urllib3 (==1.21.1)
 Requires-Dist: enum34 (>=1.1.2) ; python_version <= "3.3"
 
 This is a command line utility for accessing the Equinix Smartkey powered by Fortanix. This includes commands for managing accounts, and for performing cryptographic and key management operations.
```

