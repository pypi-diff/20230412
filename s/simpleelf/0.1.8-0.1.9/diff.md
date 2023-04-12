# Comparing `tmp/simpleelf-0.1.8.tar.gz` & `tmp/simpleelf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpleelf-0.1.8.tar", last modified: Thu Jun 25 19:52:40 2020, max compression
+gzip compressed data, was "dist/simpleelf-0.1.9.tar", last modified: Thu Jul  2 23:21:07 2020, max compression
```

## Comparing `simpleelf-0.1.8.tar` & `simpleelf-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-06-25 19:52:40.000000 simpleelf-0.1.8/
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)      267 2020-06-25 19:52:40.000000 simpleelf-0.1.8/PKG-INFO
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)     2144 2020-06-24 19:12:59.000000 simpleelf-0.1.8/README.md
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)       38 2020-06-25 19:52:40.000000 simpleelf-0.1.8/setup.cfg
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)      412 2020-06-25 19:50:38.000000 simpleelf-0.1.8/setup.py
-drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-06-25 19:52:40.000000 simpleelf-0.1.8/simpleelf/
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)     7666 2020-04-07 15:07:01.000000 simpleelf-0.1.8/simpleelf/elf_builder.py
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)     9724 2020-04-07 15:07:01.000000 simpleelf-0.1.8/simpleelf/elf_consts.py
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)    15544 2020-06-24 19:12:12.000000 simpleelf-0.1.8/simpleelf/elf_structs.py
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-04-07 15:07:01.000000 simpleelf-0.1.8/simpleelf/__init__.py
-drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-06-25 19:52:40.000000 simpleelf-0.1.8/simpleelf.egg-info/
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)        1 2020-06-25 19:52:39.000000 simpleelf-0.1.8/simpleelf.egg-info/dependency_links.txt
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)      267 2020-06-25 19:52:39.000000 simpleelf-0.1.8/simpleelf.egg-info/PKG-INFO
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)       35 2020-06-25 19:52:39.000000 simpleelf-0.1.8/simpleelf.egg-info/requires.txt
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)      320 2020-06-25 19:52:39.000000 simpleelf-0.1.8/simpleelf.egg-info/SOURCES.txt
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)       16 2020-06-25 19:52:39.000000 simpleelf-0.1.8/simpleelf.egg-info/top_level.txt
-drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-06-25 19:52:40.000000 simpleelf-0.1.8/tests/
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)     1392 2020-06-24 19:13:49.000000 simpleelf-0.1.8/tests/test_build_elf.py
--rwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-04-07 15:07:01.000000 simpleelf-0.1.8/tests/__init__.py
+drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-07-02 23:21:07.000000 simpleelf-0.1.9/
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)      267 2020-07-02 23:21:07.000000 simpleelf-0.1.9/PKG-INFO
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)     2183 2020-06-25 20:00:24.000000 simpleelf-0.1.9/README.md
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)       38 2020-07-02 23:21:07.000000 simpleelf-0.1.9/setup.cfg
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)      370 2020-07-02 23:14:08.000000 simpleelf-0.1.9/setup.py
+drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf/
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)     7684 2020-07-02 23:13:19.000000 simpleelf-0.1.9/simpleelf/elf_builder.py
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)     9724 2020-04-07 15:07:01.000000 simpleelf-0.1.9/simpleelf/elf_consts.py
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)    15544 2020-06-24 19:12:12.000000 simpleelf-0.1.9/simpleelf/elf_structs.py
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-04-07 15:07:01.000000 simpleelf-0.1.9/simpleelf/__init__.py
+drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)        1 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)      267 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/PKG-INFO
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)       19 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/requires.txt
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)      320 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)       16 2020-07-02 23:21:07.000000 simpleelf-0.1.9/simpleelf.egg-info/top_level.txt
+drwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-07-02 23:21:07.000000 simpleelf-0.1.9/tests/
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)     1392 2020-06-24 19:13:49.000000 simpleelf-0.1.9/tests/test_build_elf.py
+-rwxrwxrwx   0 doronz    (1000) doronz    (1000)        0 2020-04-07 15:07:01.000000 simpleelf-0.1.9/tests/__init__.py
```

### Comparing `simpleelf-0.1.8/README.md` & `simpleelf-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 open just an ordinary `.bin` file and running several IDAPython scripts
 (I'm sick of `Load additional binary file...` option).
 
 Pull Requests are of course more than welcome :smirk:.
 
 # Installation
 
+Support: Python 2.7 and Python 3.x.
+
 Use `pip`:
 
 ```bash
 python3 -m pip install simpleelf
 ```
 
 Or from the sources from sources:
```

### Comparing `simpleelf-0.1.8/simpleelf/elf_builder.py` & `simpleelf-0.1.9/simpleelf/elf_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,30 +24,29 @@
         self._e_shnum = 0
         self._e_shoff = self._e_phoff + self._e_phentsize * self._e_phnum
         self._strtab_text = b'\x00.strtab\x00'
 
         self.add_section(self._structs.Elf_SectionType.SHT_NULL, 0,
             0, 0, 0)
 
-
     def set_endianity(self, endianity):
         self._endianity = endianity
         self._structs = ElfStructs(endianity)        
 
     def add_segment(self, address, contents, flags):
         self._e_phnum += 1
         self._e_shoff += self._e_phentsize + len(contents)
 
         segment = self.Segment(address=address,
            flags=flags,
            contents=contents)
 
         self._segments.append(segment)
 
-    def find_loaded_data(self, address):
+    def find_loaded_data(self, address, size=None):
         offset = self._e_phoff
         data = None
 
         for segment in self._segments:
             # skip program header
             offset += self._e_phentsize
 
@@ -58,14 +57,17 @@
                 if data is None:
                     # skip current segment contents
                     offset += len(segment.contents)
 
         if data is None:
             return None
 
+        if size is not None:
+            data = data[:size]
+
         return offset, data
 
     def add_section(self, type_, address, size, name, flags):
         if name is not None:
             if type(name) is str:
                 self._strtab_text += name.encode() + b'\x00'
 
@@ -138,16 +140,14 @@
             },
             'segments': [],
             'sections': [],
         }
 
         # add segments
         segment_data_offset = self._e_phoff + self._e_phnum * self._e_phentsize
-        # print(hex(segment_data_offset))
-        # fsdfds
 
         for segment in self._segments:
             elf['segments'].append({
                 'p_type': self._structs.Elf_SegmentType.PT_LOAD,
                 'p_offset': segment_data_offset,
                 'p_vaddr': segment.address,
                 'p_paddr': segment.address,
@@ -169,15 +169,15 @@
                 if type(section.name) is int:
                     sh_name = section.name
                 else:
                     sh_name = self._strtab_text.find(section.name.encode() + b'\x00')
 
             if section.type == self._structs.Elf_SectionType.SHT_PROGBITS:
                 size = section.size
-                offset, contents = self.find_loaded_data(section.address)
+                offset, contents = self.find_loaded_data(section.address, size)
             else:  
                 # every non-loaded data into memory, which resides only in ELF
                 # will be pointed by `end_of_segments_offset`.
                 # we can append data there
                 offset = end_of_segments_offset
 
                 if section.type == self._structs.Elf_SectionType.SHT_STRTAB:
```

### Comparing `simpleelf-0.1.8/simpleelf/elf_consts.py` & `simpleelf-0.1.9/simpleelf/elf_consts.py`

 * *Files identical despite different names*

### Comparing `simpleelf-0.1.8/simpleelf/elf_structs.py` & `simpleelf-0.1.9/simpleelf/elf_structs.py`

 * *Files identical despite different names*

### Comparing `simpleelf-0.1.8/tests/test_build_elf.py` & `simpleelf-0.1.9/tests/test_build_elf.py`

 * *Files identical despite different names*

