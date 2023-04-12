# Comparing `tmp/wavfile-4.6.1.tar.gz` & `tmp/wavfile-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavfile-4.6.1.tar", last modified: Thu Apr  6 13:19:52 2023, max compression
+gzip compressed data, was "wavfile-4.7.0.tar", last modified: Wed Apr 12 20:07:20 2023, max compression
```

## Comparing `wavfile-4.6.1.tar` & `wavfile-4.7.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:19:51.996040 wavfile-4.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-06 13:19:38.000000 wavfile-4.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 13:19:38.000000 wavfile-4.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-06 13:19:51.996040 wavfile-4.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-06 13:19:38.000000 wavfile-4.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:19:51.996040 wavfile-4.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-06 13:19:38.000000 wavfile-4.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:19:51.976040 wavfile-4.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:19:51.980040 wavfile-4.6.1/src/wavfile/
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/wavread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-06 13:19:38.000000 wavfile-4.6.1/src/wavfile/wavwrite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:19:51.980040 wavfile-4.6.1/src/wavfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-06 13:19:51.000000 wavfile-4.6.1/src/wavfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-06 13:19:51.000000 wavfile-4.6.1/src/wavfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:19:51.000000 wavfile-4.6.1/src/wavfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 13:19:51.000000 wavfile-4.6.1/src/wavfile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:19:51.992040 wavfile-4.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/empty.wav
--rw-r--r--   0 runner    (1001) docker     (123)  3969304 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/noise_44100_24bit_w_metadata.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/osc_tri.wav
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/osc_tri_unsigned.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/osc_tri_wrong_chunk_order.wav
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/osc_tri_wrong_size.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1059146 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/test-file-1.wav
--rw-r--r--   0 runner    (1001) docker     (123)   384044 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/test-file-2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   720044 2023-04-06 13:19:38.000000 wavfile-4.6.1/tests/test-file-3.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:20.990669 wavfile-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 20:07:08.000000 wavfile-4.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 20:07:08.000000 wavfile-4.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-12 20:07:20.990669 wavfile-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-12 20:07:08.000000 wavfile-4.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:07:20.990669 wavfile-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 20:07:08.000000 wavfile-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:20.978669 wavfile-4.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:20.978669 wavfile-4.7.0/src/wavfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23485 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/wavread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-12 20:07:08.000000 wavfile-4.7.0/src/wavfile/wavwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:20.978669 wavfile-4.7.0/src/wavfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-12 20:07:20.000000 wavfile-4.7.0/src/wavfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 20:07:20.000000 wavfile-4.7.0/src/wavfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:07:20.000000 wavfile-4.7.0/src/wavfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 20:07:20.000000 wavfile-4.7.0/src/wavfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:07:20.990669 wavfile-4.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/empty.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  3969080 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/noise_44100_24bit_w_metadata.ext.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  3969304 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/noise_44100_24bit_w_metadata.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/osc_tri.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/osc_tri_unsigned.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/osc_tri_wrong_chunk_order.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/osc_tri_wrong_size.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1059146 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/test-file-1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   384044 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/test-file-2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   720044 2023-04-12 20:07:08.000000 wavfile-4.7.0/tests/test-file-3.wav
```

### Comparing `wavfile-4.6.1/LICENSE.txt` & `wavfile-4.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/PKG-INFO` & `wavfile-4.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavfile
-Version: 4.6.1
+Version: 4.7.0
 Summary: Read/write wave audio files to/from lists of native Python types.
 Home-page: https://github.com/chummersone/pywavfile
 Author: Christopher Hummersone
 Author-email: chummersone@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,15 @@
 .. |WavRead| replace:: ``wavfile.wavread.WavRead``
 .. |num_channels| replace:: ``num_channels``
 .. |sample_rate| replace:: ``sample_rate``
 .. |bits_per_sample| replace:: ``bits_per_sample``
 .. |num_frames| replace:: ``num_frames``
 .. |duration| replace:: ``duration``
 .. |hms| replace:: ``hms``
+.. |audio_fmt| replace:: ``audio_fmt``
 .. |format| replace:: ``format``
 .. |metadata| replace:: ``metadata``
 .. |read| replace:: ``read()``
 .. |readN| replace:: ``read([N])``
 .. |read_int| replace:: ``read_int()``
 .. |read_intN| replace:: ``read_int([N])``
 .. |read_float| replace:: ``read_float()``
@@ -105,16 +106,19 @@
 
 |duration|
   The duration of the audio file in seconds.
 
 |hms|
   The duration of the audio file formatted as hh:mm:ss.tt.
 
+|audio_fmt|
+  The audio sample format.
+
 |format|
-  The file audio sample format.
+  The wave format code.
 
 |metadata|
   A dictionary containing metadata encoded in the file.
 
 The object also has the following methods:
 
 |readN|
@@ -172,21 +176,33 @@
                     sample_rate=44100,
                     num_channels=None,
                     bits_per_sample=16,
                     fmt=wavfile.chunk.WavFormat.PCM)
 
 where ``sample_rate`` is the sampling rate for the new file,
 ``num_channels`` is the number of audio channels, ``bits_per_sample`` is
-the number of bits used to encode each sample, and ``fmt`` is the audio
-sample format. If ``num_channels`` is unspecified it will be determined
+the number of bits used to encode each sample, and ``fmt`` is the wave
+format code. If ``num_channels`` is unspecified it will be determined
 automatically from the first block of samples that are written (see
 below). This returns a |WavWrite| object. The object shares its
-properties with the |WavRead| class. The object also offers the same
-|seek|, |tell|, and |close| methods. In addition, the following methods
-are provided for writing audio data:
+properties with the |WavRead| class.
+
+The format code is either ``wavfile.chunk.WavFormat.PCM``,
+``wavfile.chunk.WavFormat.IEEE_FLOAT``, or
+``wavfile.chunk.WavFormat.EXTENSIBLE``. The extensible code corresponds
+to a variation of the wave file format intended for audio with: a bit
+depth of greater than 16 bits, or more than two channels. The file will
+be updated automatically to use the extensible format as appropriate. If
+the extensible format is specified explicitly, then the audio data will
+be PCM encoded. The |audio_fmt| property always reports the audio sample
+format, whereas the |format| property reports the format code that may
+be any of the three aforementioned values.
+
+The object also offers the same |seek|, |tell|, and |close| methods.
+In addition, the following methods are provided for writing audio data:
 
 |write|
   Write frames of audio data to the audio file. The data should be
   contained in a list of lists with size ``(N,C)``, where ``N`` is the
   number of frames and ``C`` is the number of audio channels. The data
   may be ``int`` or ``float``. The data may be converted if they do
   match the format of the destination file.
```

### Comparing `wavfile-4.6.1/README.rst` & `wavfile-4.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. |WavRead| replace:: ``wavfile.wavread.WavRead``
 .. |num_channels| replace:: ``num_channels``
 .. |sample_rate| replace:: ``sample_rate``
 .. |bits_per_sample| replace:: ``bits_per_sample``
 .. |num_frames| replace:: ``num_frames``
 .. |duration| replace:: ``duration``
 .. |hms| replace:: ``hms``
+.. |audio_fmt| replace:: ``audio_fmt``
 .. |format| replace:: ``format``
 .. |metadata| replace:: ``metadata``
 .. |read| replace:: ``read()``
 .. |readN| replace:: ``read([N])``
 .. |read_int| replace:: ``read_int()``
 .. |read_intN| replace:: ``read_int([N])``
 .. |read_float| replace:: ``read_float()``
@@ -86,16 +87,19 @@
 
 |duration|
   The duration of the audio file in seconds.
 
 |hms|
   The duration of the audio file formatted as hh:mm:ss.tt.
 
+|audio_fmt|
+  The audio sample format.
+
 |format|
-  The file audio sample format.
+  The wave format code.
 
 |metadata|
   A dictionary containing metadata encoded in the file.
 
 The object also has the following methods:
 
 |readN|
@@ -153,21 +157,33 @@
                     sample_rate=44100,
                     num_channels=None,
                     bits_per_sample=16,
                     fmt=wavfile.chunk.WavFormat.PCM)
 
 where ``sample_rate`` is the sampling rate for the new file,
 ``num_channels`` is the number of audio channels, ``bits_per_sample`` is
-the number of bits used to encode each sample, and ``fmt`` is the audio
-sample format. If ``num_channels`` is unspecified it will be determined
+the number of bits used to encode each sample, and ``fmt`` is the wave
+format code. If ``num_channels`` is unspecified it will be determined
 automatically from the first block of samples that are written (see
 below). This returns a |WavWrite| object. The object shares its
-properties with the |WavRead| class. The object also offers the same
-|seek|, |tell|, and |close| methods. In addition, the following methods
-are provided for writing audio data:
+properties with the |WavRead| class.
+
+The format code is either ``wavfile.chunk.WavFormat.PCM``,
+``wavfile.chunk.WavFormat.IEEE_FLOAT``, or
+``wavfile.chunk.WavFormat.EXTENSIBLE``. The extensible code corresponds
+to a variation of the wave file format intended for audio with: a bit
+depth of greater than 16 bits, or more than two channels. The file will
+be updated automatically to use the extensible format as appropriate. If
+the extensible format is specified explicitly, then the audio data will
+be PCM encoded. The |audio_fmt| property always reports the audio sample
+format, whereas the |format| property reports the format code that may
+be any of the three aforementioned values.
+
+The object also offers the same |seek|, |tell|, and |close| methods.
+In addition, the following methods are provided for writing audio data:
 
 |write|
   Write frames of audio data to the audio file. The data should be
   contained in a list of lists with size ``(N,C)``, where ``N`` is the
   number of frames and ``C`` is the number of audio channels. The data
   may be ``int`` or ``float``. The data may be converted if they do
   match the format of the destination file.
```

### Comparing `wavfile-4.6.1/setup.py` & `wavfile-4.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/src/wavfile/__init__.py` & `wavfile-4.7.0/src/wavfile/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,27 @@
          fmt: chunk.WavFormat = chunk.WavFormat.PCM) -> Union[wavread.WavRead, wavwrite.WavWrite]:
     """
     Open the wave file.
 
     If writing and ``num_channels`` is unspecified, it is determined automatically from the first
     block of samples.
 
+    The format code is either ``wavfile.chunk.WavFormat.PCM``,
+    ``wavfile.chunk.WavFormat.IEEE_FLOAT``, or ``wavfile.chunk.WavFormat.EXTENSIBLE``. The
+    extensible code corresponds to a variation of the wave file format intended for audio with: a
+    bit depth of greater than 16 bits, or more than two channels. The file will be updated
+    automatically to use the extensible format as appropriate. If the extensible format is specified
+    explicitly, then the audio data will be PCM encoded.
+
     :param f: Either a path to a wave file or a pointer to an open file.
     :param mode: Open the file for reading ('r', 'rb') or writing ('w', 'wb').
     :param sample_rate: The sample rate for the new file (write only).
     :param num_channels: The number of audio channels for the new file (write only).
     :param bits_per_sample: The number of bits to encode each audio sample (write only).
-    :param fmt: The audio format (write only) (:class:`chunk.WavFormat.PCM`, :class:`chunk.WavFormat.IEEE_FLOAT`)
+    :param fmt: The format code (write only) (:class:`chunk.WavFormat`)
     :return: Returns a :class:`wavread.WavRead` object or :class:`wavwrite.WavWrite` object.
     """
     if mode is None:
         if hasattr(f, 'mode'):
             mode = f.mode
         else:
             mode = 'rb'
@@ -89,15 +96,15 @@
     Metadata can be added to the wav file by providing an appropriate dict. See chunk.InfoItem for a
     list of valid metadata fields.
 
     :param path: Path to the newly created wave file.
     :param audio_data: The data to be written to the file.
     :param sample_rate: The sample rate for the new file.
     :param bits_per_sample: The number of bits to encode each audio sample (write only).
-    :param fmt: The audio format (:class:`chunk.WavFormat.PCM`, :class:`chunk.WavFormat.IEEE_FLOAT`)
+    :param fmt: The audio format (:class:`chunk.WavFormat`)
     :param metadata: The metadata to write, provided as a dictionary.
     """
     with open(path, 'w', sample_rate=sample_rate, bits_per_sample=bits_per_sample, fmt=fmt) as wf:
         wf: wavwrite.WavWrite
         if metadata is not None:
             wf.add_metadata(**metadata)
         wf.write(audio_data)
```

### Comparing `wavfile-4.6.1/src/wavfile/base.py` & `wavfile-4.7.0/src/wavfile/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,23 @@
     @property
     def bits_per_sample(self) -> int:
         """Number of bits per audio sample"""
         return self._data_chunk.fmt_chunk.bits_per_sample
 
     @property
     def format(self) -> chunk.WavFormat:
-        """Audio sample format"""
+        """Wave file format code"""
         return self._data_chunk.fmt_chunk.audio_fmt
 
     @property
+    def audio_fmt(self) -> chunk.WavFormat:
+        """Audio sample format"""
+        return self._data_chunk.audio_fmt
+
+    @property
     def num_frames(self) -> int:
         """Number of audio frames in the file"""
         try:
             return self._data_chunk.size // self._block_align
         except ZeroDivisionError:
             return 0
 
@@ -203,14 +208,15 @@
         self._riff_chunk.size = self._get_total_size()
         self._data_chunk.close()
         if self._list_chunk is not None:
             self._list_chunk.close()
         self._riff_chunk.close()
 
     def __del__(self) -> None:
-        self.close()
+        if self._should_close_file:
+            self.close()
 
     def __enter__(self) -> 'Wavfile':
         return self
 
     def __exit__(self, *args: Tuple[Any, ...]) -> None:
         self.close()
```

### Comparing `wavfile-4.6.1/src/wavfile/chunk.py` & `wavfile-4.7.0/src/wavfile/chunk.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Chunk-based helper classes for working with RIFF files.
 """
 
 import struct
 import sys
-from enum import Enum
+from enum import Enum, IntEnum
 from types import DynamicClassAttribute
 from typing import IO, List, Optional, Union, Dict
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
@@ -22,23 +22,14 @@
 
     @DynamicClassAttribute
     def value(self) -> bytes:
         """The value of the Enum member."""
         return self._value_
 
 
-class IntEnum(Enum):
-    """Enum class with bytes values"""
-
-    @DynamicClassAttribute
-    def value(self) -> int:
-        """The value of the Enum member."""
-        return self._value_
-
-
 class RiffFormat(BytesEnum):
     """RIFF file format"""
     WAVE: 'RiffFormat' = b'WAVE'
 
 
 class ChunkID(BytesEnum):
     """RIFF chunk identifiers"""
@@ -49,14 +40,15 @@
     UNKNOWN_CHUNK: 'ChunkID' = b'    '
 
 
 class WavFormat(IntEnum):
     """Wav audio data format"""
     PCM: 'WavFormat' = 0x0001
     IEEE_FLOAT: 'WavFormat' = 0x0003
+    EXTENSIBLE: 'WavFormat' = 0xFFFE
 
 
 class ListType(BytesEnum):
     """LIST chunk list types"""
     INFO: 'ListType' = b'INFO'
 
 
@@ -201,15 +193,15 @@
 
         :param data: The integer to encode.
         :param nbytes: Number of bytes encoding the integer.
         :param signed: Whether the integer is signed.
         :return: The bytes.
         """
         # noinspection PyTypeChecker
-        return data.to_bytes(nbytes, byteorder=self.endianness, signed=signed)
+        return int(data).to_bytes(nbytes, byteorder=self.endianness, signed=signed)
 
     def write_int(self, data: int, nbytes: int, signed: bool = True) -> None:
         """
         Write an integer to the chunk.
 
         :param data: The integer to encode.
         :param nbytes: Number of bytes encoding the integer.
@@ -318,81 +310,154 @@
     num_channels: int
     sample_rate: int
     byte_rate: int
     block_align: int
     bits_per_sample: int
 
     _min_size = 16
-    _audio_fmt_size: int = 2
+    audio_fmt_size: int = 2
     _num_channels_size: int = 2
     _sample_rate_size: int = 4
     _byte_rate_size: int = 4
     _block_align_size: int = 2
     _bits_per_sample_size: int = 2
 
     def __init__(self, fp: IO) -> None:
         """
         Initialise the chunk from a file pointer.
 
         :param fp: Open file pointer.
         """
         self.chunk_id = ChunkID.FMT_CHUNK
-        self.audio_fmt = WavFormat.PCM
+        if not hasattr(self, 'audio_fmt'):
+            self.audio_fmt = WavFormat.PCM
         self.num_channels = 0
         self.sample_rate = 0
         self.byte_rate = 0
         self.block_align = 0
         self.bits_per_sample = 0
 
         Chunk.__init__(self, fp, bigendian=False)
 
         if 'r' in self.fp.mode:
-            if self.chunk_id != ChunkID.FMT_CHUNK:
-                raise exception.ReadError('Chunk is not a FMT chunk')
-            self.audio_fmt = WavFormat(self.read_int(self._audio_fmt_size, signed=False))
-            self.num_channels = self.read_int(self._num_channels_size, signed=False)
-            self.sample_rate = self.read_int(self._sample_rate_size, signed=False)
-            self.byte_rate = self.read_int(self._byte_rate_size, signed=False)
-            self.block_align = self.read_int(self._block_align_size, signed=False)
-            self.bits_per_sample = self.read_int(self._bits_per_sample_size, signed=False)
+            self._read()
         else:
             self.write_fmt()
 
+    def _read(self) -> None:
+        """Read metadata from the chunk"""
+        if self.chunk_id != ChunkID.FMT_CHUNK:
+            raise exception.ReadError('Chunk is not a FMT chunk')
+        self.audio_fmt = WavFormat(self.read_int(self.audio_fmt_size, signed=False))
+        self.num_channels = self.read_int(self._num_channels_size, signed=False)
+        self.sample_rate = self.read_int(self._sample_rate_size, signed=False)
+        self.byte_rate = self.read_int(self._byte_rate_size, signed=False)
+        self.block_align = self.read_int(self._block_align_size, signed=False)
+        self.bits_per_sample = self.read_int(self._bits_per_sample_size, signed=False)
+
     @property
     def bytes_per_sample(self) -> int:
         """Number of bytes per audio sample"""
         return self.bits_per_sample // 8
 
     @property
     def signed(self) -> bool:
         """Whether the integer representation is signed"""
         return self.bytes_per_sample > 1
 
     def write_fmt(self) -> None:
         """Write the format data to the file."""
         self.fp.seek(self.content_start)
-        self.write_int(self.audio_fmt.value, self._audio_fmt_size, signed=False)
+        self.write_int(self.audio_fmt.value, self.audio_fmt_size, signed=False)
         self.write_int(self.num_channels, self._num_channels_size, signed=False)
         self.write_int(self.sample_rate, self._sample_rate_size, signed=False)
         self.write_int(self.byte_rate, self._byte_rate_size, signed=False)
         self.write_int(self.block_align, self._block_align_size, signed=False)
         self.write_int(self.bits_per_sample, self._bits_per_sample_size, signed=False)
 
     def close(self) -> None:
         """Close the chunk and update the header and format data."""
         if 'w' in self.fp.mode and not self.fp.closed:
             self.write_fmt()
         Chunk.close(self)
 
 
+class WavFmtExtensibleChunk(WavFmtChunk):
+
+    extension_size: int
+    valid_bits_per_sample: int
+    channel_mask: bytes
+    sub_format: bytes
+    sub_data_format: WavFormat
+
+    _sub_format_pad: bytes = b'\x00\x00\x00\x00\x10\x00\x80\x00\x00\xAA\x00\x38\x9B\x71'
+
+    _min_size = 18
+    _extension_size_size: int = 2
+    _valid_bits_per_sample_size: int = 2
+    _channel_mask_size: int = 4
+    _sub_format_size: int = 16
+    _sub_data_format_size: int = 2
+
+    def __init__(self, fp: IO) -> None:
+        """
+        Initialise the chunk from a file pointer.
+
+        :param fp: Open file pointer.
+        """
+        self.audio_fmt = WavFormat.EXTENSIBLE
+        self.extension_size = 0
+        self.valid_bits_per_sample = 0
+        self.channel_mask = bytearray(self._channel_mask_size)
+        self.sub_format = bytearray(self._sub_format_size)
+        self.sub_data_format = WavFormat.PCM
+        super().__init__(fp)
+
+    def _read(self) -> None:
+        """Read metadata from the chunk"""
+        super()._read()
+        self.extension_size = self.read_int(self._extension_size_size, signed=False)
+        num_remaining_byes = self.extension_size
+        if num_remaining_byes >= self._valid_bits_per_sample_size:
+            self.valid_bits_per_sample = \
+                self.read_int(self._valid_bits_per_sample_size, signed=False)
+            num_remaining_byes -= self._valid_bits_per_sample_size
+        if num_remaining_byes >= self._channel_mask_size:
+            self.channel_mask = self.read(self._channel_mask_size)
+            num_remaining_byes -= self._channel_mask_size
+        if num_remaining_byes > 0:
+            self.sub_format = self.read(num_remaining_byes)
+            self.sub_data_format = WavFormat(
+                int.from_bytes(
+                    self.sub_format[:self._sub_data_format_size],
+                    signed=False,
+                    byteorder=self.endianness
+                )
+            )
+
+    def write_fmt(self) -> None:
+        """Write the format data to the file."""
+        super().write_fmt()
+        extension_size = \
+            self._extension_size_size + \
+            self._valid_bits_per_sample_size + \
+            self._channel_mask_size + \
+            self._sub_format_size
+        self.write_int(extension_size, self._extension_size_size, signed=False)
+        self.write_int(self.valid_bits_per_sample, self._valid_bits_per_sample_size, signed=False)
+        self.write(self.channel_mask)
+        self.write_int(self.sub_data_format.value, self._sub_data_format_size, signed=False)
+        self.write(self._sub_format_pad)
+
+
 class WavDataChunk(Chunk):
     """Wave data chunk read and write"""
 
     __did_warn: bool
-    fmt_chunk: WavFmtChunk
+    fmt_chunk: Union[WavFmtChunk, WavFmtExtensibleChunk]
 
     def __init__(self, fp: IO, fmt_chunk: WavFmtChunk) -> None:
         """
         Initialise the chunk from a file pointer.
 
         :param fp: Open file pointer.
         :param fmt_chunk: The associated format chunk.
@@ -416,19 +481,27 @@
             return 0
 
     def close(self) -> None:
         """Close the chunk and update the header and format data."""
         self.fmt_chunk.close()
         Chunk.close(self)
 
+    @property
+    def audio_fmt(self) -> WavFormat:
+        """The audio sample format."""
+        if type(self.fmt_chunk) == WavFmtChunk:
+            return self.fmt_chunk.audio_fmt
+        elif type(self.fmt_chunk) == WavFmtExtensibleChunk:
+            return self.fmt_chunk.sub_data_format
+
     def read_sample(self) -> Union[int, float]:
         """Read a sample from the chunk."""
-        if self.fmt_chunk.audio_fmt == WavFormat.PCM:
+        if self.audio_fmt == WavFormat.PCM:
             return self.read_int(self.fmt_chunk.bytes_per_sample, signed=self.fmt_chunk.signed)
-        elif self.fmt_chunk.audio_fmt == WavFormat.IEEE_FLOAT:
+        elif self.audio_fmt == WavFormat.IEEE_FLOAT:
             return self.read_float(self.fmt_chunk.bytes_per_sample)
 
     def read_frames(self, nframes: Optional[int] = None) -> List[List[Union[int, float]]]:
         """
         Read a number of audio frames from the chunk. A frame is a collection of samples, from each
         audio channel, associated with a single time instant.
 
@@ -451,32 +524,32 @@
         ]
 
         return audio
 
     @property
     def _max_val(self) -> Union[float, int]:
         """Maximum value"""
-        if self.fmt_chunk.audio_fmt == WavFormat.PCM:
+        if self.audio_fmt == WavFormat.PCM:
             if self.fmt_chunk.signed:
                 sign_correction = 1
             else:
                 sign_correction = 0
             return (2 ** (self.fmt_chunk.bits_per_sample - sign_correction)) - 1
-        elif self.fmt_chunk.audio_fmt == WavFormat.IEEE_FLOAT:
+        elif self.audio_fmt == WavFormat.IEEE_FLOAT:
             return 1.0
 
     @property
     def _min_val(self) -> Union[float, int]:
         """Minimum value"""
-        if self.fmt_chunk.audio_fmt == WavFormat.PCM:
+        if self.audio_fmt == WavFormat.PCM:
             if self.fmt_chunk.signed:
                 return -self._max_val - 1
             else:
                 return 0
-        elif self.fmt_chunk.audio_fmt == WavFormat.IEEE_FLOAT:
+        elif self.audio_fmt == WavFormat.IEEE_FLOAT:
             return -1.0
 
     def __saturation_warning(self) -> None:
         """Print a warning to stderr about out-of-range sample values."""
         if not self.__did_warn:
             self.__did_warn = True
             print('Saturating one of more sample values that are out-of-range', file=sys.stderr)
@@ -494,17 +567,17 @@
     def write_sample(self, sample: Union[int, float]) -> None:
         """
         Write a sample to the chunk.
 
         :param sample: An audio sample.
         """
         sample = self._saturate(sample)
-        if self.fmt_chunk.audio_fmt == WavFormat.PCM:
+        if self.audio_fmt == WavFormat.PCM:
             self.write_int(sample, self.fmt_chunk.bytes_per_sample, signed=self.fmt_chunk.signed)
-        elif self.fmt_chunk.audio_fmt == WavFormat.IEEE_FLOAT:
+        elif self.audio_fmt == WavFormat.IEEE_FLOAT:
             self.write_float(sample, self.fmt_chunk.bytes_per_sample)
 
     def write_frames(self, audio: List[List[Union[int, float]]]) -> None:
         """
         Write one or more frames of audio to the chunk.
 
         :param audio: The audio frames as a list of lists.
```

### Comparing `wavfile-4.6.1/src/wavfile/wavread.py` & `wavfile-4.7.0/src/wavfile/wavread.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,27 @@
             # rewind to chunk start
             self.fp.seek(-chunk.Chunk.offset, 1)
 
             # interpret each chunk
             if chnk.chunk_id == chunk.ChunkID.RIFF_CHUNK:
                 self._riff_chunk = chunk.RiffChunk(self.fp)
             elif chnk.chunk_id == chunk.ChunkID.FMT_CHUNK:
-                fmt_chunk = chunk.WavFmtChunk(self.fp)
+                # get audio format
+                self.fp.seek(chunk.Chunk.offset, 1)
+                audio_fmt_int = int.from_bytes(
+                    self.fp.read(chunk.WavFmtChunk.audio_fmt_size),
+                    signed=False,
+                    byteorder='little'
+                )
+                audio_fmt = chunk.WavFormat(audio_fmt_int)
+                self.fp.seek(-chunk.Chunk.offset - chunk.WavFmtChunk.audio_fmt_size, 1)
+                if audio_fmt == chunk.WavFormat.EXTENSIBLE:
+                    fmt_chunk = chunk.WavFmtExtensibleChunk(self.fp)
+                else:
+                    fmt_chunk = chunk.WavFmtChunk(self.fp)
             elif chnk.chunk_id == chunk.ChunkID.DATA_CHUNK:
                 if fmt_chunk is None:
                     raise exception.ReadError('DATA chunk read before FMT chunk')
                 self._data_chunk = chunk.WavDataChunk(self.fp, fmt_chunk)
             elif chnk.chunk_id == chunk.ChunkID.LIST_CHUNK:
                 self._list_chunk = chunk.ListChunk(self.fp)
 
@@ -118,15 +130,15 @@
         a list of lists with dimensions `(N,C)`, where `C` is the number of audio channels. Choosing
         `N = None` or `N < 0` will read all remaining samples.
 
         :param num_frames: Maximum number of frames to read.
         :return: The audio samples as a list of lists.
         """
         audio = self._data_chunk.read_frames(num_frames)
-        if self.format == chunk.WavFormat.IEEE_FLOAT:
+        if self.audio_fmt == chunk.WavFormat.IEEE_FLOAT:
             for n in range(len(audio)):
                 for m in range(len(audio[n])):
                     audio[n][m] = self._convert_float_to_int(audio[n][m])
         return audio
 
     def iter_int(self, num_frames: Optional[int] = None) -> Generator[List[List[int]], None, None]:
         """
@@ -144,17 +156,17 @@
         The method returns a list of lists with size `[N][C]`, where `C` is the number of audio
         channels. Choosing `N = None` or `N < 0` will read all remaining samples.
 
         :param num_frames: Maximum number of frames to read.
         :return: The audio samples as a list of lists.
         """
         audio: List[List[Union[int, float]]] = []
-        if self.format == chunk.WavFormat.IEEE_FLOAT:
+        if self.audio_fmt == chunk.WavFormat.IEEE_FLOAT:
             audio = self._data_chunk.read_frames(num_frames)
-        elif self.format == chunk.WavFormat.PCM:
+        elif self.audio_fmt == chunk.WavFormat.PCM:
             audio = self.read_int(num_frames)
             audio = [[self._convert_int_to_float(sample) for sample in frame] for frame in audio]
 
         return audio
 
     def iter_float(self, num_frames: Optional[int] = None) -> \
             Generator[List[List[float]], None, None]:
```

### Comparing `wavfile-4.6.1/src/wavfile/wavwrite.py` & `wavfile-4.7.0/src/wavfile/wavwrite.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Provides the WavWrite class for writing wave files.
 
 The WavWrite class is returned by wavfile.open() when opening a file in write
 mode.
 """
 import os
+import sys
 from typing import IO, List, Optional, Union
 
 from . import base
 from . import chunk
 from . import exception
 
 
@@ -19,31 +20,39 @@
 
     _is_open: bool
 
     def __init__(self, fp: Union[str, os.PathLike, IO], sample_rate: int = 44100,
                  num_channels: Optional[int] = None, bits_per_sample: int = 16,
                  fmt: chunk.WavFormat = chunk.WavFormat.PCM) -> None:
         """
-        Initialise the WavWrite object.
+        Initialise the WavWrite object. The `fmt` argument may be any of the enumerations of
+        `wavfile.chunk.WavFormat`. If `wavfile.chunk.WavFormat.EXTENSIBLE` is specified, then the
+        audio data are PCM-encoded.
 
         :param fp: Either a path to a wave file or a pointer to an open file.
         :param sample_rate: The sample rate for the new file.
         :param num_channels: The number of audio channels for the new file.
         :param bits_per_sample: The number of bits to encode each audio sample.
-        :param fmt: The audio format (:class:`wavfile.chunk.WavFormat.PCM`, :class:`wavfile.chunk.WavFormat.IEEE_FLOAT`)
+        :param fmt: The audio format (:class:`wavfile.chunk.WavFormat`)
         """
         base.Wavfile.__init__(self)
 
         self._is_open = True
         self._init_fp(fp, 'wb')
 
-        # initialise each of the riff chunk
+        # initialise each of the riff chunks
         self._riff_chunk = chunk.RiffChunk(self.fp)
-        fmt_chunk = chunk.WavFmtChunk(self.fp)
-        fmt_chunk.audio_fmt = fmt
+        if bits_per_sample > 16 or (num_channels is not None and num_channels > 2) or \
+                fmt == chunk.WavFormat.EXTENSIBLE:
+            fmt_chunk = chunk.WavFmtExtensibleChunk(self.fp)
+            if fmt != chunk.WavFormat.EXTENSIBLE:
+                fmt_chunk.sub_data_format = fmt
+        else:
+            fmt_chunk = chunk.WavFmtChunk(self.fp)
+            fmt_chunk.audio_fmt = fmt
         self._data_chunk = chunk.WavDataChunk(self.fp, fmt_chunk)
         self._data_chunk.fmt_chunk.sample_rate = int(sample_rate)
         if num_channels is not None:
             self._data_chunk.fmt_chunk.num_channels = int(num_channels)
         self._data_chunk.fmt_chunk.bits_per_sample = int(bits_per_sample)
         self._list_chunk = None
 
@@ -52,15 +61,15 @@
 
     def __repr__(self) -> str:
         """
         Return the object representation in string format.
         """
         return f'{self.__class__.__name__}("{self.fp.name}", sample_rate={self.sample_rate}, ' + \
                f'num_channels={self.num_channels}, bits_per_sample={self.bits_per_sample}, ' + \
-               f'fmt={self.format})'
+               f'fmt={self.format.__class__.__name__}.{self.format.name})'
 
     @staticmethod
     def _data_are_floats(data: List[List[Union[int, float]]]) -> bool:
         """
         Check for any floats in data.
 
         data: Audio buffer to analyse for floats.
@@ -80,15 +89,15 @@
         """
         Write float data to the file. If the file format is `PCM` then the data will be converted to
         floats, otherwise there will be no conversion.
 
         :param audio: Audio frames to write.
         """
         self.__check_metadata()
-        if self.format == chunk.WavFormat.PCM:
+        if self.audio_fmt == chunk.WavFormat.PCM:
             # data are floats but we are writing integers
             for n in range(len(audio)):
                 for m in range(len(audio[n])):
                     audio[n][m] = self._convert_float_to_int(audio[n][m])
 
         self._data_chunk.write_frames(audio)
 
@@ -96,15 +105,15 @@
         """
         Write integer data to the file. If the file format is `IEEE_FLOAT` then the data will be
         converted to floats, otherwise there will be no conversion.
 
         :param audio: Audio frames to write.
         """
         self.__check_metadata()
-        if self.format == chunk.WavFormat.IEEE_FLOAT:
+        if self.audio_fmt == chunk.WavFormat.IEEE_FLOAT:
             # data are integers but we are writing floats
             audio: List[List[Union[int, float]]]
             for n in range(len(audio)):
                 for m in range(len(audio[n])):
                     audio[n][m] = self._convert_int_to_float(audio[n][m])
 
         self._data_chunk.write_frames(audio)
@@ -169,7 +178,13 @@
         if num_align_bytes > 0:
             self._data_chunk.skip(include_pad=False)
             self._data_chunk.write(bytearray(num_align_bytes), update_size=False)
         base.Wavfile.close(self)
         if self._should_close_file:
             self.fp.close()
         self._should_close_file = False
+        if self.format != chunk.WavFormat.EXTENSIBLE and \
+                self.num_channels > 2:
+            print('More than two audio channels are present, but the file does not use the '
+                  'EXTENSIBLE format. The file may not be readable in some software.',
+                  file=sys.stderr
+                  )
```

### Comparing `wavfile-4.6.1/src/wavfile.egg-info/PKG-INFO` & `wavfile-4.7.0/src/wavfile.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavfile
-Version: 4.6.1
+Version: 4.7.0
 Summary: Read/write wave audio files to/from lists of native Python types.
 Home-page: https://github.com/chummersone/pywavfile
 Author: Christopher Hummersone
 Author-email: chummersone@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,15 @@
 .. |WavRead| replace:: ``wavfile.wavread.WavRead``
 .. |num_channels| replace:: ``num_channels``
 .. |sample_rate| replace:: ``sample_rate``
 .. |bits_per_sample| replace:: ``bits_per_sample``
 .. |num_frames| replace:: ``num_frames``
 .. |duration| replace:: ``duration``
 .. |hms| replace:: ``hms``
+.. |audio_fmt| replace:: ``audio_fmt``
 .. |format| replace:: ``format``
 .. |metadata| replace:: ``metadata``
 .. |read| replace:: ``read()``
 .. |readN| replace:: ``read([N])``
 .. |read_int| replace:: ``read_int()``
 .. |read_intN| replace:: ``read_int([N])``
 .. |read_float| replace:: ``read_float()``
@@ -105,16 +106,19 @@
 
 |duration|
   The duration of the audio file in seconds.
 
 |hms|
   The duration of the audio file formatted as hh:mm:ss.tt.
 
+|audio_fmt|
+  The audio sample format.
+
 |format|
-  The file audio sample format.
+  The wave format code.
 
 |metadata|
   A dictionary containing metadata encoded in the file.
 
 The object also has the following methods:
 
 |readN|
@@ -172,21 +176,33 @@
                     sample_rate=44100,
                     num_channels=None,
                     bits_per_sample=16,
                     fmt=wavfile.chunk.WavFormat.PCM)
 
 where ``sample_rate`` is the sampling rate for the new file,
 ``num_channels`` is the number of audio channels, ``bits_per_sample`` is
-the number of bits used to encode each sample, and ``fmt`` is the audio
-sample format. If ``num_channels`` is unspecified it will be determined
+the number of bits used to encode each sample, and ``fmt`` is the wave
+format code. If ``num_channels`` is unspecified it will be determined
 automatically from the first block of samples that are written (see
 below). This returns a |WavWrite| object. The object shares its
-properties with the |WavRead| class. The object also offers the same
-|seek|, |tell|, and |close| methods. In addition, the following methods
-are provided for writing audio data:
+properties with the |WavRead| class.
+
+The format code is either ``wavfile.chunk.WavFormat.PCM``,
+``wavfile.chunk.WavFormat.IEEE_FLOAT``, or
+``wavfile.chunk.WavFormat.EXTENSIBLE``. The extensible code corresponds
+to a variation of the wave file format intended for audio with: a bit
+depth of greater than 16 bits, or more than two channels. The file will
+be updated automatically to use the extensible format as appropriate. If
+the extensible format is specified explicitly, then the audio data will
+be PCM encoded. The |audio_fmt| property always reports the audio sample
+format, whereas the |format| property reports the format code that may
+be any of the three aforementioned values.
+
+The object also offers the same |seek|, |tell|, and |close| methods.
+In addition, the following methods are provided for writing audio data:
 
 |write|
   Write frames of audio data to the audio file. The data should be
   contained in a list of lists with size ``(N,C)``, where ``N`` is the
   number of frames and ``C`` is the number of audio channels. The data
   may be ``int`` or ``float``. The data may be converted if they do
   match the format of the destination file.
```

### Comparing `wavfile-4.6.1/src/wavfile.egg-info/SOURCES.txt` & `wavfile-4.7.0/src/wavfile.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/wavfile/wavread.py
 src/wavfile/wavwrite.py
 src/wavfile.egg-info/PKG-INFO
 src/wavfile.egg-info/SOURCES.txt
 src/wavfile.egg-info/dependency_links.txt
 src/wavfile.egg-info/top_level.txt
 tests/empty.wav
+tests/noise_44100_24bit_w_metadata.ext.wav
 tests/noise_44100_24bit_w_metadata.wav
 tests/osc_tri.wav
 tests/osc_tri_unsigned.wav
 tests/osc_tri_wrong_chunk_order.wav
 tests/osc_tri_wrong_size.wav
 tests/test-file-1.wav
 tests/test-file-2.wav
```

### Comparing `wavfile-4.6.1/tests/noise_44100_24bit_w_metadata.wav` & `wavfile-4.7.0/tests/noise_44100_24bit_w_metadata.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/osc_tri.wav` & `wavfile-4.7.0/tests/osc_tri.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/osc_tri_unsigned.wav` & `wavfile-4.7.0/tests/osc_tri_unsigned.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/osc_tri_wrong_chunk_order.wav` & `wavfile-4.7.0/tests/osc_tri_wrong_chunk_order.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/osc_tri_wrong_size.wav` & `wavfile-4.7.0/tests/osc_tri_wrong_size.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/test-file-1.wav` & `wavfile-4.7.0/tests/test-file-1.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/test-file-2.wav` & `wavfile-4.7.0/tests/test-file-2.wav`

 * *Files identical despite different names*

### Comparing `wavfile-4.6.1/tests/test-file-3.wav` & `wavfile-4.7.0/tests/test-file-3.wav`

 * *Files identical despite different names*

