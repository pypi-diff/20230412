# Comparing `tmp/showcert-0.1.8-py3-none-any.whl.zip` & `tmp/showcert-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7779 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx    12417 b- defN 22-Aug-23 15:35 showcert-0.1.8.data/scripts/showcert
--rw-r--r--  2.0 unx     1074 b- defN 22-Aug-23 15:35 showcert-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4113 b- defN 22-Aug-23 15:35 showcert-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-23 15:35 showcert-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Aug-23 15:35 showcert-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      484 b- defN 22-Aug-23 15:35 showcert-0.1.8.dist-info/RECORD
-6 files, 18181 bytes uncompressed, 6901 bytes compressed:  62.0%
+Zip file size: 7832 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx    12564 b- defN 22-Sep-06 18:51 showcert-0.1.9.data/scripts/showcert
+-rw-r--r--  2.0 unx     1074 b- defN 22-Sep-06 18:51 showcert-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4113 b- defN 22-Sep-06 18:51 showcert-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Sep-06 18:51 showcert-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 22-Sep-06 18:51 showcert-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      484 b- defN 22-Sep-06 18:51 showcert-0.1.9.dist-info/RECORD
+6 files, 18328 bytes uncompressed, 6954 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: showcert-0.1.8.data/scripts/showcert
+Filename: showcert-0.1.9.data/scripts/showcert
 Comment: 
 
-Filename: showcert-0.1.8.dist-info/LICENSE
+Filename: showcert-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: showcert-0.1.8.dist-info/METADATA
+Filename: showcert-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: showcert-0.1.8.dist-info/WHEEL
+Filename: showcert-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: showcert-0.1.8.dist-info/top_level.txt
+Filename: showcert-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: showcert-0.1.8.dist-info/RECORD
+Filename: showcert-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `showcert-0.1.8.data/scripts/showcert` & `showcert-0.1.9.data/scripts/showcert`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from datetime import datetime
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from collections import namedtuple
 
 
 
-version = '0.1.8'
+version = '0.1.9'
 args = None
 
 phrase = namedtuple('Phrase', 'say wait expect')
 
 class CertException(Exception):
     pass
 
@@ -151,14 +151,17 @@
     
     context.set_verify(SSL.VERIFY_PEER)
     context.load_verify_locations(cafile=args.ca)
 
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.settimeout(args.limit)
     s.connect((host, port))
+
+    sock_host, sock_port = s.getpeername()
+    
     start_tls(s, args.starttls, port)
 
     conn = SSL.Connection(
         context, socket=s
     )
         
     # conn.settimeout(5)
@@ -166,15 +169,16 @@
     conn.setblocking(1)
 
     conn.set_tlsext_host_name(name.encode())
     
     conn.set_connect_state()
     conn.do_handshake()
 
-    return conn.get_peer_cert_chain()
+    chain = conn.get_peer_cert_chain()
+    return sock_host, chain
 
 
 def is_local(cert):
     """ guesses is cert is local file or not """
     if os.path.exists(cert) or cert == '-':
         return True
     return False
@@ -310,44 +314,47 @@
 
 
 def print_dnames(crt):
     names = get_names(crt)
     print('-d', ' -d '.join(names))
 
 
-def print_cert(crt, location=None):
+def print_cert(crt, addr=None):
 
     def tlist2str(tlist):
         return ' '.join([ '{}={}'.format(t[0].decode(), t[1].decode()) for t in tlist ])
 
     nbefore = datetime.strptime(crt.get_notBefore().decode(), '%Y%m%d%H%M%SZ')
     nafter = datetime.strptime(crt.get_notAfter().decode(), '%Y%m%d%H%M%SZ')
     daysold = (datetime.now() - nbefore).days
     daysleft = (nafter - datetime.now()).days
     issuer = tlist2str(crt.get_issuer().get_components())
 
     names = get_names(crt)
 
+    if addr:
+        print("IP:", addr)
     print("Names:", ' '.join(names))
     print("notBefore: {nbefore} ({days} days old)".format(nbefore=nbefore, days=daysold))
     print("notAfter: {nafter} ({days} days left)".format(nafter=nafter, days = daysleft))
     print("Issuer:", issuer)
 
 def process_cert(CERT, name=None, insecure=False, warn=False, starttls='auto'):
 
     retcode = 0
     hostname = None
     out = args.output.lower()
+    sock_host = None
 
     try:
         if is_local(CERT):
             chain = get_local_certs(CERT)
         else:
             hostname = name or CERT.split(':')[0]
-            chain = get_remote_certs(location=CERT, name=name, insecure=insecure, starttls=starttls)
+            sock_host, chain = get_remote_certs(location=CERT, name=name, insecure=insecure, starttls=starttls)
     except SSL.Error as e:
         print("{CERT} Certificate verification error (use -i): {exception}".format(CERT=CERT, exception=e),
             file=sys.stderr)
         return 1
     except socket.timeout as e:
         print("Timeout connecting to {}".format(CERT), file=sys.stderr)
         return 1
@@ -381,15 +388,15 @@
             r = dump_certificate(FILETYPE_PEM, _c)
             print(r.decode(), end='')
         return 0
     elif out == 'brief':
         for i,_c in enumerate(chain):
             if i>0:
                 print()
-            print_cert(_c, location=CERT)
+            print_cert(_c, addr=sock_host)
 
     elif out == 'full':
         for i,_c in enumerate(chain):
             if i>0:
                 print()
             print_full_cert(_c)
```

## Comparing `showcert-0.1.8.dist-info/LICENSE` & `showcert-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `showcert-0.1.8.dist-info/METADATA` & `showcert-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showcert
-Version: 0.1.8
+Version: 0.1.9
 Summary: dump local/remote certificate info
 Home-page: https://github.com/yaroslaff/showcert
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

