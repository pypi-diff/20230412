# Comparing `tmp/MyCaesarCipher-0.3.0.tar.gz` & `tmp/MyCaesarCipher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyCaesarCipher-0.3.0.tar", last modified: Sun Feb 12 09:42:03 2023, max compression
+gzip compressed data, was "MyCaesarCipher-0.4.0.tar", last modified: Wed Apr 12 15:58:09 2023, max compression
```

## Comparing `MyCaesarCipher-0.3.0.tar` & `MyCaesarCipher-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 09:42:03.994361 MyCaesarCipher-0.3.0/
--rw-rw-rw-   0        0        0    35823 2022-02-09 18:54:43.000000 MyCaesarCipher-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       15 2022-04-12 00:56:14.000000 MyCaesarCipher-0.3.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-02-12 09:42:03.978363 MyCaesarCipher-0.3.0/MyCaesarCipher/
--rw-rw-rw-   0        0        0       30 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/MyCaesarCipher/__init__.py
--rw-rw-rw-   0        0        0     4241 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/MyCaesarCipher/main.py
-drwxrwxrwx   0        0        0        0 2023-02-12 09:42:03.991362 MyCaesarCipher-0.3.0/MyCaesarCipher/tests/
--rw-rw-rw-   0        0        0     2611 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/MyCaesarCipher/tests/MyCaesarCipher_Test.py
--rw-rw-rw-   0        0        0        0 2022-03-20 01:03:15.000000 MyCaesarCipher-0.3.0/MyCaesarCipher/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 09:42:03.988376 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/
--rw-rw-rw-   0        0        0     7658 2023-02-12 09:42:03.000000 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-02-12 09:42:03.000000 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 09:42:03.000000 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-02-12 09:42:03.000000 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-12 09:42:03.000000 MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7658 2023-02-12 09:42:03.993366 MyCaesarCipher-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6515 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/README.md
--rw-rw-rw-   0        0        0       20 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 09:42:03.994361 MyCaesarCipher-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1528 2023-02-12 09:34:58.000000 MyCaesarCipher-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:58:09.151300 MyCaesarCipher-0.4.0/
+-rw-rw-rw-   0        0        0    35823 2022-02-09 18:54:43.000000 MyCaesarCipher-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-04-12 00:56:14.000000 MyCaesarCipher-0.4.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-12 15:58:09.130354 MyCaesarCipher-0.4.0/MyCaesarCipher/
+-rw-rw-rw-   0        0        0        0 2023-04-12 15:33:01.000000 MyCaesarCipher-0.4.0/MyCaesarCipher/__init__.py
+-rw-rw-rw-   0        0        0     4255 2023-04-12 15:49:51.000000 MyCaesarCipher-0.4.0/MyCaesarCipher/main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:58:09.148306 MyCaesarCipher-0.4.0/MyCaesarCipher/tests/
+-rw-rw-rw-   0        0        0     3924 2023-04-12 14:24:59.000000 MyCaesarCipher-0.4.0/MyCaesarCipher/tests/MyCaesarCipher_Test.py
+-rw-rw-rw-   0        0        0        0 2022-03-20 01:03:15.000000 MyCaesarCipher-0.4.0/MyCaesarCipher/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:58:09.143319 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/
+-rw-rw-rw-   0        0        0     7854 2023-04-12 15:58:09.000000 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-12 15:58:09.000000 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:58:09.000000 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 15:58:09.000000 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 15:58:09.000000 MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7854 2023-04-12 15:58:09.150300 MyCaesarCipher-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6695 2023-04-12 15:47:49.000000 MyCaesarCipher-0.4.0/README.md
+-rw-rw-rw-   0        0        0       20 2023-04-12 14:27:52.000000 MyCaesarCipher-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:58:09.151300 MyCaesarCipher-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-04-12 15:49:34.000000 MyCaesarCipher-0.4.0/setup.py
```

### Comparing `MyCaesarCipher-0.3.0/LICENSE` & `MyCaesarCipher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MyCaesarCipher-0.3.0/MyCaesarCipher/main.py` & `MyCaesarCipher-0.4.0/MyCaesarCipher/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
 from random import randint
 from typing import Optional
 
+__version__ = '0.4.0'
+
 
 class CaesarCipher:
-    """Cryptographic encryption/decryption techniques using the Caesar-Cipher algorithm.
+    """Cryptographic encryption/decryption using the Caesar-Cipher algorithm.
 
     ---
 
     - Substitutes each letter of a message with new "matching" letter shifted down alphabetically by a given amount.
 
     - Not intended for real-world cryptographic applications, as the Caesar-Cipher algorithm is notoriously easy to crack.
 
@@ -17,15 +19,15 @@
         - https://en.wikipedia.org/wiki/Caesar_cipher
     """
 
     @staticmethod
     def encrypt(text: str,
                 key: Optional[int] = None,
                 stdout_output: bool = True) -> str:
-        """Encrypt text using the Caesar-Cypher cryptography algorithm.
+        """Encrypt text using the Caesar-Cipher cryptography algorithm.
 
         - Generates encrypted form of :param:`text` using the Caesar-Cipher algorithm.
         - If no :param:`key` is provided, a random integer value is generated.
         - Optionally disable output of encrypted text results to stdout by toggling :param:`stdout_output` to `False`.
 
         ---
 
@@ -60,15 +62,15 @@
             elif (char.isdigit()):
                 output += str((int(char) + key) % 10)
 
             #@ Leave all non-alphanumeric characters unchanged.
             else:
                 output += char
 
-        info: str = f'> Original Msg : {text}\n\n> Shift-key : {key}\n\n> Encrypted Result: {output}\n'
+        info: str = f'> Original Txt : {text}\n\n> Shift-key : {key}\n\n> Encrypted Result: {output}\n'
 
         if stdout_output:
             print(info)
 
         return output
 
     @staticmethod
```

### Comparing `MyCaesarCipher-0.3.0/MyCaesarCipher.egg-info/PKG-INFO` & `MyCaesarCipher-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,58 @@
-Metadata-Version: 2.1
-Name: MyCaesarCipher
-Version: 0.3.0
-Summary: Simple cryptographic substitution-based cipher for encoding plaintext.
-Home-page: https://github.com/schlopp96/MyCaesarCipher
-Author: schlopp96
-Author-email: schloppdaddy@gmail.com
-License: UNKNOWN
-Keywords: cryptography,Caesar-Cipher,Caesar,Cipher,encryption,decryption,cryptographic,module,script,python
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MyCaesarCipher
 
 > Simple cryptographic substitution-based cipher for encoding plaintext.
 
 ---
 
 ## About
 
 - The [Caesar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher) is one of the most simple and well-known encryption techniques.
 
   - Each letter in the plaintext entry is replaced by a letter found at a certain number of positions down the alphabet.
 
-- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced python programmers interested in cryptography!
+- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced Python programmers interested in cryptography!
 
 ---
 
 ## Installation
 
 ### Using pip _(Recommended)_
 
-> _Easiest_ method. _**Highly recommended over manual installation.**_
+> **_Easiest_ method.**
+> _Highly recommended over manual installation._
 
 - Run the following to install _**`MyCaesarCipher`**_ using `pip`:
 
   - ```python
     pip install MyCaesarCipher
     ```
 
-- You should now be able to import/run _**`MyCaesarCipher`**_ within your python environment by entering the following:
+- You should now be able to import/run _**`MyCaesarCipher`**_ within your Python environment by entering the following:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
     ...
     ```
 
 - Done!
 
 ---
 
 ### Manual Installation
 
-> _Not_ recommended. _**Only use this method if you are unable to use `pip`**_.
+> **_Not_ recommended.**
+> _Only use this method if you are unable to install using `pip`_.
 
 1. Before use, navigate to the intended installation location, and create a new directory.
 
 2. Please only do one of the following:
 
     - **A.** Clone repository with the git client of your preference.
-    - **B.** Download and extract the source code `zip` archive from the ["[releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
+    - **B.** Download and extract the source code `zip` archive from the ["releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
 
 3. Install all dependencies for this package within the installation directory using the following command:
 
     - ```python
       pip install -r requirements.txt
       ```
 
@@ -86,83 +62,83 @@
 
 ---
 
 ## Usage
 
 - Within a Python environment or **`.py`** project, simply import the _**`MyCaesarCipher`**_ module to start encryption/decryption of ciphers.
 
-### Message Encryption
+### Text Encryption
 
 - For encrypting text, use the **`CaesarCipher.encrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
-    >>> msg = 'Test Cipher'
-    >>> cipher.encrypt(text=msg, key=200, stdout_output=True)
+    >>> txt = 'Test Cipher'
+    >>> cipher.encrypt(text=txt, key=15, stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
-    > Shift-Key : 200
+    > Shift-Key : 15
 
-    > Encrypted Result: Lwkl Uahzwj
+    > Encrypted Result: Ithi Rxewtg
     ```
 
-- Therefore the final encrypted result of "Test Cipher" using a shift key of 200 is:
+- Therefore the final encrypted result of "Test Cipher" using a shift key of 15 is:
 
-  - "**`LwklfUahzwj`**".
+  - "**`Ithi Rxewtg`**".
 
 - Note that the `key` parameter is _optional_, and if not provided, a random key between 1 and 25 will be generated:
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 19
 
     > Encrypted Result: Mxlm Vbiaxk
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 24
 
     > Encrypted Result: Rcqr Agnfcp
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 4
 
     > Encrypted Result: Xiwx Gmtliv
     ```
 
 ---
 
-### Message Decryption
+### Text Decryption
 
 - For decrypting text, use the **`CaesarCipher.decrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
@@ -217,27 +193,28 @@
     > Decrypted Shift-Key 22 : Sdrs Bhogdq
 
     > Decrypted Shift-Key 23 : Rcqr Agnfcp
 
     > Decrypted Shift-Key 24 : Qbpq Zfmebo
 
     > Decrypted Shift-Key 25 : Paop Yeldan
+    ```
 
+- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted text as a dictionary.
+  - This is NOT printed to stdout even if the `stdout_output` parameter is set to `True`.
+
+  - ```python
     {'Ozno Xdkczm': 0, 'Nymn Wcjbyl': 1, 'Mxlm Vbiaxk': 2, 'Lwkl Uahzwj': 3, 'Kvjk Tzgyvi': 4, 'Juij Syfxuh': 5, 'Ithi Rxewtg': 6, 'Hsgh Qwdvsf': 7, 'Grfg Pvcure': 8, 'Fqef Oubtqd': 9, 'Epde Ntaspc': 10, 'Docd Mszrob': 11, 'Cnbc Lryqna': 12, 'Bmab Kqxpmz': 13, 'Alza Jpwoly': 14, 'Zkyz Iovnkx': 15, 'Yjxy Hnumjw': 16, 'Xiwx Gmtliv': 17, 'Whvw Flskhu': 18, 'Vguv Ekrjgt': 19, 'Uftu Djqifs': 20, 'Test Cipher': 21, 'Sdrs Bhogdq': 22, 'Rcqr Agnfcp': 23, 'Qbpq Zfmebo': 24, 'Paop Yeldan': 25}
     ```
 
-- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted message as a dictionary.
+- **_Generally_**, the _most legible_ key output will be the correct decrypted text (assuming the encrypted text was legible initially).
 
-- **_Generally_**, the _most legible_ key output will be the correct decrypted message, assuming the encrypted message was legible initially.
-
-- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet 26 and the number of possible integers [0-9].
-  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases.
+- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet [26] and the number of possible integers [0-9].
+  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases, as it is rather simple to decipher Caesar-Cipher encrypted text.
 
 ---
 
 ## Contact
 
 - If you have any questions, comments, or concerns that cannot be alleviated through the [project's GitHub repository](https://github.com/schlopp96/MyCaesarCipher), please feel free to contact me through my email address:
 
   - `schloppdaddy@gmail.com`
-
-
```

### Comparing `MyCaesarCipher-0.3.0/PKG-INFO` & `MyCaesarCipher-0.4.0/MyCaesarCipher.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MyCaesarCipher
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple cryptographic substitution-based cipher for encoding plaintext.
 Home-page: https://github.com/schlopp96/MyCaesarCipher
 Author: schlopp96
 Author-email: schloppdaddy@gmail.com
 License: UNKNOWN
-Keywords: cryptography,Caesar-Cipher,Caesar,Cipher,encryption,decryption,cryptographic,module,script,python
+Keywords: cryptography,Caesar-Cipher,Caesar,Cipher,encryption,decryption,cryptographic,module,script,encrypt,decrypt,python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
@@ -32,51 +32,53 @@
 
 ## About
 
 - The [Caesar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher) is one of the most simple and well-known encryption techniques.
 
   - Each letter in the plaintext entry is replaced by a letter found at a certain number of positions down the alphabet.
 
-- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced python programmers interested in cryptography!
+- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced Python programmers interested in cryptography!
 
 ---
 
 ## Installation
 
 ### Using pip _(Recommended)_
 
-> _Easiest_ method. _**Highly recommended over manual installation.**_
+> **_Easiest_ method.**
+> _Highly recommended over manual installation._
 
 - Run the following to install _**`MyCaesarCipher`**_ using `pip`:
 
   - ```python
     pip install MyCaesarCipher
     ```
 
-- You should now be able to import/run _**`MyCaesarCipher`**_ within your python environment by entering the following:
+- You should now be able to import/run _**`MyCaesarCipher`**_ within your Python environment by entering the following:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
     ...
     ```
 
 - Done!
 
 ---
 
 ### Manual Installation
 
-> _Not_ recommended. _**Only use this method if you are unable to use `pip`**_.
+> **_Not_ recommended.**
+> _Only use this method if you are unable to install using `pip`_.
 
 1. Before use, navigate to the intended installation location, and create a new directory.
 
 2. Please only do one of the following:
 
     - **A.** Clone repository with the git client of your preference.
-    - **B.** Download and extract the source code `zip` archive from the ["[releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
+    - **B.** Download and extract the source code `zip` archive from the ["releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
 
 3. Install all dependencies for this package within the installation directory using the following command:
 
     - ```python
       pip install -r requirements.txt
       ```
 
@@ -86,83 +88,83 @@
 
 ---
 
 ## Usage
 
 - Within a Python environment or **`.py`** project, simply import the _**`MyCaesarCipher`**_ module to start encryption/decryption of ciphers.
 
-### Message Encryption
+### Text Encryption
 
 - For encrypting text, use the **`CaesarCipher.encrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
-    >>> msg = 'Test Cipher'
-    >>> cipher.encrypt(text=msg, key=200, stdout_output=True)
+    >>> txt = 'Test Cipher'
+    >>> cipher.encrypt(text=txt, key=15, stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
-    > Shift-Key : 200
+    > Shift-Key : 15
 
-    > Encrypted Result: Lwkl Uahzwj
+    > Encrypted Result: Ithi Rxewtg
     ```
 
-- Therefore the final encrypted result of "Test Cipher" using a shift key of 200 is:
+- Therefore the final encrypted result of "Test Cipher" using a shift key of 15 is:
 
-  - "**`LwklfUahzwj`**".
+  - "**`Ithi Rxewtg`**".
 
 - Note that the `key` parameter is _optional_, and if not provided, a random key between 1 and 25 will be generated:
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 19
 
     > Encrypted Result: Mxlm Vbiaxk
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 24
 
     > Encrypted Result: Rcqr Agnfcp
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 4
 
     > Encrypted Result: Xiwx Gmtliv
     ```
 
 ---
 
-### Message Decryption
+### Text Decryption
 
 - For decrypting text, use the **`CaesarCipher.decrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
@@ -217,24 +219,27 @@
     > Decrypted Shift-Key 22 : Sdrs Bhogdq
 
     > Decrypted Shift-Key 23 : Rcqr Agnfcp
 
     > Decrypted Shift-Key 24 : Qbpq Zfmebo
 
     > Decrypted Shift-Key 25 : Paop Yeldan
+    ```
+
+- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted text as a dictionary.
+  - This is NOT printed to stdout even if the `stdout_output` parameter is set to `True`.
 
+  - ```python
     {'Ozno Xdkczm': 0, 'Nymn Wcjbyl': 1, 'Mxlm Vbiaxk': 2, 'Lwkl Uahzwj': 3, 'Kvjk Tzgyvi': 4, 'Juij Syfxuh': 5, 'Ithi Rxewtg': 6, 'Hsgh Qwdvsf': 7, 'Grfg Pvcure': 8, 'Fqef Oubtqd': 9, 'Epde Ntaspc': 10, 'Docd Mszrob': 11, 'Cnbc Lryqna': 12, 'Bmab Kqxpmz': 13, 'Alza Jpwoly': 14, 'Zkyz Iovnkx': 15, 'Yjxy Hnumjw': 16, 'Xiwx Gmtliv': 17, 'Whvw Flskhu': 18, 'Vguv Ekrjgt': 19, 'Uftu Djqifs': 20, 'Test Cipher': 21, 'Sdrs Bhogdq': 22, 'Rcqr Agnfcp': 23, 'Qbpq Zfmebo': 24, 'Paop Yeldan': 25}
     ```
 
-- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted message as a dictionary.
-
-- **_Generally_**, the _most legible_ key output will be the correct decrypted message, assuming the encrypted message was legible initially.
+- **_Generally_**, the _most legible_ key output will be the correct decrypted text (assuming the encrypted text was legible initially).
 
-- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet 26 and the number of possible integers [0-9].
-  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases.
+- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet [26] and the number of possible integers [0-9].
+  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases, as it is rather simple to decipher Caesar-Cipher encrypted text.
 
 ---
 
 ## Contact
 
 - If you have any questions, comments, or concerns that cannot be alleviated through the [project's GitHub repository](https://github.com/schlopp96/MyCaesarCipher), please feel free to contact me through my email address:
```

### Comparing `MyCaesarCipher-0.3.0/README.md` & `MyCaesarCipher-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,84 @@
+Metadata-Version: 2.1
+Name: MyCaesarCipher
+Version: 0.4.0
+Summary: Simple cryptographic substitution-based cipher for encoding plaintext.
+Home-page: https://github.com/schlopp96/MyCaesarCipher
+Author: schlopp96
+Author-email: schloppdaddy@gmail.com
+License: UNKNOWN
+Keywords: cryptography,Caesar-Cipher,Caesar,Cipher,encryption,decryption,cryptographic,module,script,encrypt,decrypt,python
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MyCaesarCipher
 
 > Simple cryptographic substitution-based cipher for encoding plaintext.
 
 ---
 
 ## About
 
 - The [Caesar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher) is one of the most simple and well-known encryption techniques.
 
   - Each letter in the plaintext entry is replaced by a letter found at a certain number of positions down the alphabet.
 
-- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced python programmers interested in cryptography!
+- This project was created as an exercise while I was taking the ["Cracking Codes with Python"](https://inventwithpython.com/cracking/) course - which I _highly_ recommend for both beginners and experienced Python programmers interested in cryptography!
 
 ---
 
 ## Installation
 
 ### Using pip _(Recommended)_
 
-> _Easiest_ method. _**Highly recommended over manual installation.**_
+> **_Easiest_ method.**
+> _Highly recommended over manual installation._
 
 - Run the following to install _**`MyCaesarCipher`**_ using `pip`:
 
   - ```python
     pip install MyCaesarCipher
     ```
 
-- You should now be able to import/run _**`MyCaesarCipher`**_ within your python environment by entering the following:
+- You should now be able to import/run _**`MyCaesarCipher`**_ within your Python environment by entering the following:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
     ...
     ```
 
 - Done!
 
 ---
 
 ### Manual Installation
 
-> _Not_ recommended. _**Only use this method if you are unable to use `pip`**_.
+> **_Not_ recommended.**
+> _Only use this method if you are unable to install using `pip`_.
 
 1. Before use, navigate to the intended installation location, and create a new directory.
 
 2. Please only do one of the following:
 
     - **A.** Clone repository with the git client of your preference.
-    - **B.** Download and extract the source code `zip` archive from the ["[releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
+    - **B.** Download and extract the source code `zip` archive from the ["releases"](https://github.com/schlopp96/MyCaesarCipher/releases) page to the newly created directory.
 
 3. Install all dependencies for this package within the installation directory using the following command:
 
     - ```python
       pip install -r requirements.txt
       ```
 
@@ -60,83 +88,83 @@
 
 ---
 
 ## Usage
 
 - Within a Python environment or **`.py`** project, simply import the _**`MyCaesarCipher`**_ module to start encryption/decryption of ciphers.
 
-### Message Encryption
+### Text Encryption
 
 - For encrypting text, use the **`CaesarCipher.encrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
-    >>> msg = 'Test Cipher'
-    >>> cipher.encrypt(text=msg, key=200, stdout_output=True)
+    >>> txt = 'Test Cipher'
+    >>> cipher.encrypt(text=txt, key=15, stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
-    > Shift-Key : 200
+    > Shift-Key : 15
 
-    > Encrypted Result: Lwkl Uahzwj
+    > Encrypted Result: Ithi Rxewtg
     ```
 
-- Therefore the final encrypted result of "Test Cipher" using a shift key of 200 is:
+- Therefore the final encrypted result of "Test Cipher" using a shift key of 15 is:
 
-  - "**`LwklfUahzwj`**".
+  - "**`Ithi Rxewtg`**".
 
 - Note that the `key` parameter is _optional_, and if not provided, a random key between 1 and 25 will be generated:
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 19
 
     > Encrypted Result: Mxlm Vbiaxk
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 24
 
     > Encrypted Result: Rcqr Agnfcp
     ```
 
     ---
 
   - ```python
     >>> cipher.encrypt('Test Cipher', stdout_output=True)
 
     ------------------------------------
 
-    > Original Msg : Test Cipher
+    > Original Txt : Test Cipher
 
     > Shift-key : 4
 
     > Encrypted Result: Xiwx Gmtliv
     ```
 
 ---
 
-### Message Decryption
+### Text Decryption
 
 - For decrypting text, use the **`CaesarCipher.decrypt`** class method:
 
   - ```python
     >>> from MyCaesarCipher import CaesarCipher
 
     >>> cipher = CaesarCipher() # Create new class instance.
@@ -191,25 +219,30 @@
     > Decrypted Shift-Key 22 : Sdrs Bhogdq
 
     > Decrypted Shift-Key 23 : Rcqr Agnfcp
 
     > Decrypted Shift-Key 24 : Qbpq Zfmebo
 
     > Decrypted Shift-Key 25 : Paop Yeldan
+    ```
 
+- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted text as a dictionary.
+  - This is NOT printed to stdout even if the `stdout_output` parameter is set to `True`.
+
+  - ```python
     {'Ozno Xdkczm': 0, 'Nymn Wcjbyl': 1, 'Mxlm Vbiaxk': 2, 'Lwkl Uahzwj': 3, 'Kvjk Tzgyvi': 4, 'Juij Syfxuh': 5, 'Ithi Rxewtg': 6, 'Hsgh Qwdvsf': 7, 'Grfg Pvcure': 8, 'Fqef Oubtqd': 9, 'Epde Ntaspc': 10, 'Docd Mszrob': 11, 'Cnbc Lryqna': 12, 'Bmab Kqxpmz': 13, 'Alza Jpwoly': 14, 'Zkyz Iovnkx': 15, 'Yjxy Hnumjw': 16, 'Xiwx Gmtliv': 17, 'Whvw Flskhu': 18, 'Vguv Ekrjgt': 19, 'Uftu Djqifs': 20, 'Test Cipher': 21, 'Sdrs Bhogdq': 22, 'Rcqr Agnfcp': 23, 'Qbpq Zfmebo': 24, 'Paop Yeldan': 25}
     ```
 
-- The **`CaesarCipher.decrypt`** method will return all possible shifted-key variations of the given encrypted message as a dictionary.
+- **_Generally_**, the _most legible_ key output will be the correct decrypted text (assuming the encrypted text was legible initially).
 
-- **_Generally_**, the _most legible_ key output will be the correct decrypted message, assuming the encrypted message was legible initially.
-
-- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet 26 and the number of possible integers [0-9].
-  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases.
+- Regardless, the correct output **MUST** be one of the output values due to the limitations of the algorithm being tied to the length of the alphabet [26] and the number of possible integers [0-9].
+  - This is also the reason why the algorithm is not recommended for serious real-world cryptography use cases, as it is rather simple to decipher Caesar-Cipher encrypted text.
 
 ---
 
 ## Contact
 
 - If you have any questions, comments, or concerns that cannot be alleviated through the [project's GitHub repository](https://github.com/schlopp96/MyCaesarCipher), please feel free to contact me through my email address:
 
   - `schloppdaddy@gmail.com`
+
+
```

### Comparing `MyCaesarCipher-0.3.0/setup.py` & `MyCaesarCipher-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path("readme.md").read_text()
 reqs = pathlib.Path("requirements.txt").read_text()
 setup(name="MyCaesarCipher",
-      version="0.3.0",
+      version='0.4.0',
       description=
       'Simple cryptographic substitution-based cipher for encoding plaintext.',
       url='https://github.com/schlopp96/MyCaesarCipher',
       author='schlopp96',
       author_email='schloppdaddy@gmail.com',
       long_description=readme,
       long_description_content_type='text/markdown',
@@ -28,9 +28,10 @@
           "Programming Language :: Python :: 3.11",
           "Topic :: Software Development :: Libraries :: Python Modules",
           "Topic :: Security :: Cryptography",
           "Topic :: Utilities",
       ],
       keywords=[
           'cryptography', 'Caesar-Cipher', 'Caesar', 'Cipher', 'encryption',
-          'decryption', 'cryptographic', 'module', 'script', 'python'
+          'decryption', 'cryptographic', 'module', 'script', 'encrypt',
+          'decrypt', 'python'
       ])
```

