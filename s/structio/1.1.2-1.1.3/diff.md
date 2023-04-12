# Comparing `tmp/structio-1.1.2.tar.gz` & `tmp/structio-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.1.2.tar", last modified: Fri Apr  7 12:17:11 2023, max compression
+gzip compressed data, was "structio-1.1.3.tar", last modified: Wed Apr 12 11:57:47 2023, max compression
```

## Comparing `structio-1.1.2.tar` & `structio-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:17:11.080571 structio-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-07 12:17:11.080571 structio-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-07 12:16:51.000000 structio-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-07 12:16:51.000000 structio-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 12:17:11.080571 structio-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 12:17:11.080571 structio-1.1.2/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-07 12:17:11.000000 structio-1.1.2/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 12:17:11.000000 structio-1.1.2/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 12:17:11.000000 structio-1.1.2/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 12:17:11.000000 structio-1.1.2/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11119 2023-04-07 12:16:51.000000 structio-1.1.2/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:57:47.008119 structio-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-12 11:57:47.008119 structio-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-12 11:57:28.000000 structio-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 11:57:28.000000 structio-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:57:47.008119 structio-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:57:47.008119 structio-1.1.3/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-12 11:57:47.000000 structio-1.1.3/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 11:57:47.000000 structio-1.1.3/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:57:47.000000 structio-1.1.3/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 11:57:47.000000 structio-1.1.3/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-12 11:57:28.000000 structio-1.1.3/structio.py
```

### Comparing `structio-1.1.2/PKG-INFO` & `structio-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -188,14 +188,26 @@
 
 Appends bytes object *b* to the object at the current location.
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
+**delete(length)**
+
+Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+
+**find(bytes_sequence, n=1)**
+
+Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
+
+**index(bytes_sequence, n=1)**
+
+Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
+
 **read_bool()**
 
 Read one byte from the object and converts it into a boolean.
 
 **write_bool(boolean)**
 
 Writes *boolean* to the object.
@@ -299,19 +311,7 @@
 **append_7bint(number)**
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
 Overwrites the 7 bit integer at the current position with *number*.
-
-**delete(length)**
-
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
-
-**find(bytes_sequence, n=1)**
-
-Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
-
-**index(bytes_sequence, n=1)**
-
-Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
```

### Comparing `structio-1.1.2/README.md` & `structio-1.1.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,26 @@
 
 Appends bytes object *b* to the object at the current location.
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
+**delete(length)**
+
+Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+
+**find(bytes_sequence, n=1)**
+
+Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
+
+**index(bytes_sequence, n=1)**
+
+Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
+
 **read_bool()**
 
 Read one byte from the object and converts it into a boolean.
 
 **write_bool(boolean)**
 
 Writes *boolean* to the object.
@@ -290,20 +302,8 @@
 
 **append_7bint(number)**
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
-Overwrites the 7 bit integer at the current position with *number*.
-
-**delete(length)**
-
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
-
-**find(bytes_sequence, n=1)**
-
-Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
-
-**index(bytes_sequence, n=1)**
-
-Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
+Overwrites the 7 bit integer at the current position with *number*.
```

### Comparing `structio-1.1.2/structio.egg-info/PKG-INFO` & `structio-1.1.3/structio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -188,14 +188,26 @@
 
 Appends bytes object *b* to the object at the current location.
 
 **overwrite(self, start, end, b)**
 
 Replaces the bytes between positions *start* and *end* with *b*.
 
+**delete(length)**
+
+Deletes *length* bytes from the object starting from *current position - length* to *current position*.
+
+**find(bytes_sequence, n=1)**
+
+Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
+
+**index(bytes_sequence, n=1)**
+
+Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
+
 **read_bool()**
 
 Read one byte from the object and converts it into a boolean.
 
 **write_bool(boolean)**
 
 Writes *boolean* to the object.
@@ -299,19 +311,7 @@
 **append_7bint(number)**
 
 Converts *number* into a 7 bit integer and appends it to the object.
 
 **overwrite_7bint(number)**
 
 Overwrites the 7 bit integer at the current position with *number*.
-
-**delete(length)**
-
-Deletes *length* bytes from the object starting from *current position - length* to *current position*.
-
-**find(bytes_sequence, n=1)**
-
-Searches the object for *bytes_sequence*. Returns the location in which the *nth* occurrence of *bytes_sequence* can be found, returns -1 if it's not found. Starts searching from the current position in the buffer.
-
-**index(bytes_sequence, n=1)**
-
-Same as find but raises a *ValueError* if it fails to find *bytes_sequence*.
```

### Comparing `structio-1.1.2/structio.py` & `structio-1.1.3/structio.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,46 +61,60 @@
         
     def unpack_str(self, b):
         return b.decode(self.encoding, errors=self.errors)
         
     def pack_str(self, string):
         return string.encode(self.encoding, errors=self.errors)
         
-    def unpack_cstr(self, b, start=0):
+    def _get_cstr_end(self, b, start=0):
         end = b.find(b'\x00', start)
         
         if end == -1:
             raise ValueError('null termination not found')
             
-        return self.unpack_str(b[start:end])
+        return end + 1
+        
+    def unpack_cstr(self, b, start=0):
+        self._end = end = self._get_cstr_end(b, start)
+        return self.unpack_str(b[start:(end - 1)])
         
     def pack_cstr(self, string):
         return self.pack_str(string) + b'\x00'
         
+    def _get_pstr_end(self, b, numbytes, endian=None, start=0):
+        return start + numbytes + self.unpack_int(b[start:(start + numbytes)], endian)
+        
     def unpack_pstr(self, b, numbytes, endian=None, start=0):
-        int_end = start + numbytes
-        length = self.unpack_int(b[start:int_end], endian)
-        return self.unpack_str(b[int_end:(int_end + length)])
+        self._end = end = self._get_pstr_end(b, numbytes, endian, start)
+        return self.unpack_str(b[(start + numbytes):end])
         
     def pack_pstr(self, string, numbytes, endian=None):
-        return self.pack_int(len(string), numbytes, endian) + self.pack_str(string)
+        b = self.pack_str(string)
+        return self.pack_int(len(b), numbytes, endian) + b
+        
+    def _get_7bint_end(self, b, start=0):
+        i = 0
+        while b[start + i] & 0b10000000 != 0:
+            i += 1
+            
+        return start + i + 1
         
     def unpack_7bint(self, b, start=0):
         number = 0
         i = 0
         
         byte = b[start + i]
         while byte & 0b10000000 != 0:
             number |= (byte & 0b01111111) << (7 * i)
             i += 1
             
             byte = b[start + i]
             
         number |= byte << (7 * i)
-        
+        self._end = start + i + 1
         return number
         
     def pack_7bint(self, number):
         b = bytearray()
         
         while number > 127:
             b += self.pack_int(number & 0b01111111 | 0b10000000, 1) 
@@ -183,14 +197,46 @@
         self.seek(start)
         length = self.write(b)
         self.write(buffer)
         self.truncate()
         self.seek(start + length)
         return length
         
+    def delete(self, length):
+        current_position = self.tell()
+        
+        if current_position - length < 0:
+            length = current_position
+            
+        start = current_position - length
+        self.overwrite(start, current_position, b'')
+        
+        return length
+        
+    def find(self, bytes_sequence, n=1):
+        start = self.tell()
+        content = self.getvalue()
+        location = content.find(bytes_sequence, start)
+        
+        for i in range(1, n):
+            location = content.find(bytes_sequence, location + 1)
+            
+            if location == -1:
+                break
+                
+        return location
+        
+    def index(self, bytes_sequence, n=1):
+        end = self.find(bytes_sequence, n)
+        
+        if end == -1:
+            raise ValueError('{} not found'.format(bytes_sequence))
+            
+        return end
+        
     def read_bool(self):
         return self._struct.unpack_bool(self.read(1))
         
     def write_bool(self, boolean):
         return self.write(self._struct.pack_bool(boolean))
         
     def append_bool(self, boolean):
@@ -233,108 +279,56 @@
         return self.append(self._struct.pack_str(string))
         
     def overwrite_str(self, string, length):
         start = self.tell()
         return self.overwrite(start, start + length, self._struct.pack_str(string))
         
     def read_cstr(self):
-        end = self.find(b'\x00')
-        
-        if end == -1:
-            raise ValueError('null termination not found')
-            
         start = self.tell()
-        string = self._struct.unpack_str(self.read(end - start))
-        self.seek(1, 1)
-        return string
+        value = self._struct.unpack_cstr(self.getvalue(), start=start)
+        self.seek(self._struct._end)
+        return value
         
     def write_cstr(self, string):
         return self.write(self._struct.pack_cstr(string))
         
     def append_cstr(self, string):
         return self.append(self._struct.pack_cstr(string))
         
     def overwrite_cstr(self, string):
-        end = self.find(b'\x00')
-        
-        if end == -1:
-            raise ValueError('null termination not found')
-            
         start = self.tell()
-        return self.overwrite(start, end + 1, self._struct.pack_cstr(string))
+        end = self._struct._get_cstr_end(self.getvalue(), start=start)
+        return self.overwrite(start, end, self._struct.pack_cstr(string))
         
     def read_pstr(self, numbytes, endian=None):
-        return self.read_str(self.read_int(numbytes, endian))
+        start = self.tell()
+        value = self._struct.unpack_pstr(self.getvalue(), numbytes, endian, start=start)
+        self.seek(self._struct._end)
+        return value
         
     def write_pstr(self, string, numbytes, endian=None):
-        return self.write_int(len(string), numbytes, endian) + self.write_str(string)
+        return self.write(self._struct.pack_pstr(string, numbytes, endian))
         
     def append_pstr(self, string, numbytes, endian=None):
         return self.append(self._struct.pack_pstr(string, numbytes, endian))
         
     def overwrite_pstr(self, string, numbytes, endian=None):
         start = self.tell()
-        length = self.read_int(numbytes, endian)
-        return self.overwrite(start, start + numbytes + length, self._struct.pack_pstr(string, numbytes, endian))
+        end = self._struct._get_pstr_end(self.getvalue(), numbytes, endian, start=start)
+        return self.overwrite(start, end, self._struct.pack_pstr(string, numbytes, endian))
         
     def read_7bint(self):
-        number = 0
-        i = 0
-        
-        byte = self.read_int(1)
-        while byte & 0b10000000 != 0:
-            number |= (byte & 0b01111111) << (7 * i)
-            i += 1
-            
-            byte = self.read_int(1)
-            
-        number |= byte << (7 * i)
-        
-        return number
+        start = self.tell()
+        value = self._struct.unpack_7bint(self.getvalue(), start=start)
+        self.seek(self._struct._end)
+        return value
         
     def write_7bint(self, number):
         return self.write(self._struct.pack_7bint(number))
         
     def append_7bint(self, number):
         return self.append(self._struct.pack_7bint(number))
         
     def overwrite_7bint(self, number):
         start = self.tell()
-        
-        while self.read_int(1) & 0b10000000 != 0:
-            pass
-            
-        end = self.tell()
-        
-        return self.overwrite(start, end, self._struct.pack_7bint(number))
-        
-    def delete(self, length):
-        current_position = self.tell()
-        
-        if current_position - length < 0:
-            length = current_position
-            
-        start = current_position - length
-        self.overwrite(start, current_position, b'')
-        
-        return length
-        
-    def find(self, bytes_sequence, n=1):
-        start = self.tell()
-        content = self.getvalue()
-        location = content.find(bytes_sequence, start)
-        
-        for i in range(1, n):
-            location = content.find(bytes_sequence, location + 1)
-            
-            if location == -1:
-                break
-                
-        return location
-        
-    def index(self, bytes_sequence, n=1):
-        end = self.find(bytes_sequence, n)
-        
-        if end == -1:
-            raise ValueError('{} not found'.format(bytes_sequence))
-            
-        return end
+        end = self._struct._get_7bint_end(self.getvalue(), start=start)
+        return self.overwrite(start, end, self._struct.pack_7bint(number))
```

