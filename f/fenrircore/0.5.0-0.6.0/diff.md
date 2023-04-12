# Comparing `tmp/fenrircore-0.5.0.tar.gz` & `tmp/fenrircore-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrircore-0.5.0.tar", last modified: Mon Apr 10 18:30:46 2023, max compression
+gzip compressed data, was "fenrircore-0.6.0.tar", last modified: Wed Apr 12 19:41:59 2023, max compression
```

## Comparing `fenrircore-0.5.0.tar` & `fenrircore-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.5.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-10 18:30:46.511050 fenrircore-0.5.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-01 22:01:01.000000 fenrircore-0.5.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/fenrircore/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-10 17:51:42.000000 fenrircore-0.5.0/fenrircore/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)       65 2023-04-10 17:56:19.000000 fenrircore-0.5.0/fenrircore/__main__.py
--rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/arper.py
--rw-r--r--   0 hannes    (1000) users      (100)     6868 2023-04-10 18:24:20.000000 fenrircore-0.5.0/fenrircore/fenrir.py
--rw-r--r--   0 hannes    (1000) users      (100)     6706 2023-02-19 18:40:50.000000 fenrircore-0.5.0/fenrircore/filehandler.py
--rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/firewall.py
--rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-02-17 12:58:30.000000 fenrircore-0.5.0/fenrircore/getmacvendors.py
--rw-r--r--   0 hannes    (1000) users      (100)     8258 2023-03-25 12:41:10.000000 fenrircore-0.5.0/fenrircore/scanner.py
--rw-r--r--   0 hannes    (1000) users      (100)    11899 2023-04-01 17:09:45.000000 fenrircore-0.5.0/fenrircore/vpn.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-10 18:30:46.511050 fenrircore-0.5.0/fenrircore.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      469 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.5.0/fenrircore.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       53 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-10 18:30:46.000000 fenrircore-0.5.0/fenrircore.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-10 18:30:46.511050 fenrircore-0.5.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      896 2023-04-10 17:51:36.000000 fenrircore-0.5.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-02-17 12:58:30.000000 fenrircore-0.6.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-12 19:41:59.361579 fenrircore-0.6.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)     1673 2023-04-10 18:38:00.000000 fenrircore-0.6.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/fenrircore/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)       65 2023-04-10 17:56:19.000000 fenrircore-0.6.0/fenrircore/__main__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11033 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/arper.py
+-rw-r--r--   0 hannes    (1000) users      (100)     6868 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/fenrir.py
+-rw-r--r--   0 hannes    (1000) users      (100)     7516 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/filehandler.py
+-rw-r--r--   0 hannes    (1000) users      (100)     4923 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/firewall.py
+-rw-r--r--   0 hannes    (1000) users      (100)     2019 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/getmacvendors.py
+-rw-r--r--   0 hannes    (1000) users      (100)     8258 2023-04-10 18:38:00.000000 fenrircore-0.6.0/fenrircore/scanner.py
+-rw-r--r--   0 hannes    (1000) users      (100)    11909 2023-04-12 19:39:27.000000 fenrircore-0.6.0/fenrircore/vpn.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:41:59.361579 fenrircore-0.6.0/fenrircore.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      492 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      469 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-02 11:09:58.000000 fenrircore-0.6.0/fenrircore.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       54 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       11 2023-04-12 19:41:59.000000 fenrircore-0.6.0/fenrircore.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-12 19:41:59.361579 fenrircore-0.6.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      897 2023-04-12 19:39:27.000000 fenrircore-0.6.0/setup.py
```

### Comparing `fenrircore-0.5.0/LICENSE` & `fenrircore-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/README.md` & `fenrircore-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/arper.py` & `fenrircore-0.6.0/fenrircore/arper.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/fenrir.py` & `fenrircore-0.6.0/fenrircore/fenrir.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/filehandler.py` & `fenrircore-0.6.0/fenrircore/filehandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-#!/bin/env python3
+#!/bin/env python3.10
 
 import base64
 import hashlib
 from argparse import ArgumentParser
-from cryptography import fernet
+from Cryptodome.Protocol.KDF import PBKDF2
+from Cryptodome.Random import get_random_bytes
+from Cryptodome.Cipher import AES
+from io import BytesIO
 from os import fdopen
 from tempfile import mkstemp
 
+BLOCK_SIZE = 16
+
 
 class filehandler():
     """ class to contain all filesystem related methods
 
     Handles encryption and decryption for config files
     set default passphrase to hashed mac address if not given
     """
@@ -22,54 +27,68 @@
         """
         if not passphrase:
             with open('/sys/class/net/' + interface + '/address') as f:
                 passphrase = f.readline()
         passphrase.strip()
         hlib = hashlib.md5()
         hlib.update(passphrase.encode('utf-8'))
-        self.__passphrase__ = base64.urlsafe_b64encode(
-            hlib.hexdigest().encode('utf-8'))
+        self.password = base64.urlsafe_b64encode(hlib.hexdigest().encode('utf-8'))
+        self.salt = get_random_bytes(BLOCK_SIZE)
+        self.__passphrase__ = PBKDF2(self.password, self.salt, dkLen=32)
 
     def encode(self, plaintext) -> bytes:
         """ encode/ encrypt given plaintext
 
         :param plaintext: plaintext to be encoded with pre-set passphrase
         """
-        f = fernet.Fernet(self.__passphrase__)
-        return f.encrypt(plaintext.encode('utf-8'))
+        cipher = AES.new(self.__passphrase__, AES.MODE_EAX)
+        buffer = BytesIO()
+        buffer.write(self.salt)
+        if isinstance(plaintext, str):
+            plaintext = plaintext.encode('utf-8')
+        ciphertext, tag = cipher.encrypt_and_digest(plaintext)
+        [buffer.write(x) for x in (cipher.nonce, tag, ciphertext)]
+        return buffer.getvalue()
 
-    def decode(self, ciphertext) -> bytes:
+    def decode(self, cipherbuffertext) -> bytes:
         """ decode/ decrypt given ciphertext
 
         :param ciphertext: ciphertext to be decoded with pre-set passphrase
         """
-        f = fernet.Fernet(self.__passphrase__)
-        return f.decrypt(ciphertext.encode('utf-8'))
+        if isinstance(cipherbuffertext, str):
+            buffer = BytesIO(cipherbuffertext.encode('utf-8'))
+        else:
+            buffer = BytesIO(cipherbuffertext)
+        salt = buffer.read(BLOCK_SIZE)
+        key = PBKDF2(self.password, salt, dkLen=32)
+        cipher = AES.new(key, AES.MODE_EAX, nonce=buffer.read(BLOCK_SIZE))
+        tag = buffer.read(BLOCK_SIZE)
+        return cipher.decrypt_and_verify(buffer.read(), tag).decode('utf-8')
 
     def checkpassword(self, ciphertext) -> bool:
         """ check if currently set password is correct
 
         :param ciphertext: test cipher to decrypt with given password
         """
         try:
-            self.decode(ciphertext.decode('utf-8'))
-        except fernet.InvalidToken:
+            self.decode(ciphertext)
+        except ValueError:
             return False
         return True
 
     def decrypttofile(self, ciphertext):
         """ decrypt given ciphertext and return path do decrypted file
 
         :param ciphertext: text to be decrypted
 
         creates new file with decrypted content
         """
         fd, authpath = mkstemp()
         with fdopen(fd, 'w') as fp:
-            fp.write(self.decode(ciphertext).decode('utf-8'))
+            fp.write(self.decode(ciphertext))
         return authpath
 
     def decryptfile(self, inputfile) -> str:
         """ decrypt given file and return path do decrypted file
 
         :param inputfile: path for file to be decrypted
 
@@ -116,15 +135,15 @@
     desitnationtext = ''
     if isencrypt:
         desitnationtext = fenc.encode(sourcetext)
     else:
         desitnationtext = fenc.decode(sourcetext)
 
     with open(destinationfile, 'w') as f:
-        f.write(desitnationtext.decode('utf-8'))
+        f.write(desitnationtext)
 
 
 def encrypt(sourcefile, destinationfile, passphrase=None, interface=None) -> None:
     """ encrypt given sourcefile to destinationfile
 
     :param sourcefile: file to be encrypted
     :param destinationfile: file for ciphertext to be stored
```

### Comparing `fenrircore-0.5.0/fenrircore/firewall.py` & `fenrircore-0.6.0/fenrircore/firewall.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/getmacvendors.py` & `fenrircore-0.6.0/fenrircore/getmacvendors.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/scanner.py` & `fenrircore-0.6.0/fenrircore/scanner.py`

 * *Files identical despite different names*

### Comparing `fenrircore-0.5.0/fenrircore/vpn.py` & `fenrircore-0.6.0/fenrircore/vpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
                  dbpath='/var/cache/fenrir/fenrir.sqlite') -> None:
         """ initialization
 
         :param interface: if given use as VPN interface
         :param dbpath: path to vpn settings database
         :param password: password for encryption
         """
-        self.inputinterface = inputinterface
-        self.vpninterface = vpninterface
+        self.inputinterface = inputinterface if inputinterface else 'eth0'
+        self.vpninterface = vpninterface if vpninterface else 'tun0'
         self.dbpath = dbpath
         self.pipepath = str(join(dirname(self.dbpath), 'fenrirvpn.pipe'))
         self.endnow = False
         self.password = password
         self.connectionprofiles = {}
         self.vpnconnectionprocesses = {}
         self.vpnauthfiles = {}
@@ -139,21 +139,21 @@
             # new connection -> create conntection folder and files
             if profilename not in self.vpnconnectionprocesses.keys():
                 debug(f'starting connection process for {profilename}...')
                 fh = filehandler(passphrase=self.password)
                 # create common auth file for username and password
                 encuser = self.connectionprofiles[profilename]['username']
                 encpass = self.connectionprofiles[profilename]['password']
-                authfile = fh.decrypttofile(encuser.decode('utf-8'))
-                tmppass = fh.decrypttofile(encpass.decode('utf-8'))
+                authfile = fh.decrypttofile(encuser)
+                tmppass = fh.decrypttofile(encpass)
                 with open(authfile, 'a') as writefile:
                     with open(tmppass, 'r') as readfile:
                         writefile.write('\n' + readfile.read())
                 unlink(tmppass)
-                config = fh.decrypttofile(self.connectionprofiles[profilename]['config'].decode('utf-8'))
+                config = fh.decrypttofile(self.connectionprofiles[profilename]['config'])
                 interface = self.vpninterface
                 if not self.connectionprofiles[profilename]['isdefault']:
                     interface = 'tun' + md5(profilename.encode('utf-8')).hexdigest()[:3]
                 debug(f'using {config} for config, {authfile} for auth and {interface} as interface...')
                 self.vpnauthfiles[profilename] = {'config': config, 'authfile': authfile}
                 startcmd = ['/usr/sbin/openvpn', '--auth-nocache']
                 startcmd += ['--config', self.vpnauthfiles[profilename]['config']]
```

### Comparing `fenrircore-0.5.0/setup.py` & `fenrircore-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 
 This is done via ARP Spoofing. Determined default GW on inputinterface is spoofed to configured device.
     """,
     authors=['Hannes Hofer <Hannes.Hofer@gmail.com>'],
     packages=['fenrircore'],
     include_package_data=True,
     zip_safe=False,
-    install_requires=['cryptography', 'pyroute2', 'python_iptables', 'requests', 'scapy'],
+    install_requires=['pycryptodomex', 'pyroute2', 'python_iptables', 'requests', 'scapy'],
     entry_points={'console_scripts': ['fenrir = fenrircore.fenrir:main', ]},
     project_urls={
         'Source': 'https://github.com/HannesHofer/fenrir',
         'Tracker': 'https://github.com/HannesHofer/fenrir/issues'
     }
 )
```

