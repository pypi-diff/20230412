# Comparing `tmp/heifip-1.0.0.tar.gz` & `tmp/heifip-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heifip-1.0.0.tar", last modified: Tue Apr  4 12:30:44 2023, max compression
+gzip compressed data, was "heifip-1.1.0.tar", last modified: Wed Apr 12 08:32:26 2023, max compression
```

## Comparing `heifip-1.0.0.tar` & `heifip-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.168027 heifip-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-04 12:30:32.000000 heifip-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-04-04 12:30:44.168027 heifip-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-04 12:30:32.000000 heifip-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.164027 heifip-1.0.0/heifip/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.164027 heifip-1.0.0/heifip/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.168027 heifip-1.0.0/heifip/images/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/images/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/images/markovchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/images/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.168027 heifip-1.0.0/heifip/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/layers/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.168027 heifip-1.0.0/heifip/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/plugins/header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.168027 heifip-1.0.0/heifip/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-04 12:30:32.000000 heifip-1.0.0/heifip/protocols/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:30:44.164027 heifip-1.0.0/heifip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-04-04 12:30:44.000000 heifip-1.0.0/heifip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-04 12:30:44.000000 heifip-1.0.0/heifip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:30:44.000000 heifip-1.0.0/heifip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 12:30:44.000000 heifip-1.0.0/heifip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 12:30:44.000000 heifip-1.0.0/heifip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-04 12:30:32.000000 heifip-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-04 12:30:44.168027 heifip-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.503359 heifip-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-12 08:32:14.000000 heifip-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-04-12 08:32:26.503359 heifip-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-12 08:32:14.000000 heifip-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.499359 heifip-1.1.0/heifip/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.499359 heifip-1.1.0/heifip/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.499359 heifip-1.1.0/heifip/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/flow_tiled_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/flow_tiled_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/markovchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/images/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.503359 heifip-1.1.0/heifip/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/layers/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.503359 heifip-1.1.0/heifip/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/plugins/header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.503359 heifip-1.1.0/heifip/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-12 08:32:14.000000 heifip-1.1.0/heifip/protocols/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:32:26.499359 heifip-1.1.0/heifip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-04-12 08:32:26.000000 heifip-1.1.0/heifip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 08:32:26.000000 heifip-1.1.0/heifip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:32:26.000000 heifip-1.1.0/heifip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:32:26.000000 heifip-1.1.0/heifip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 08:32:26.000000 heifip-1.1.0/heifip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-12 08:32:14.000000 heifip-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 08:32:26.503359 heifip-1.1.0/setup.cfg
```

### Comparing `heifip-1.0.0/LICENSE` & `heifip-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/PKG-INFO` & `heifip-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heifip
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool to convert network traffic into images for ML use cases.
 Author-email: Stefan Machmeier <stefan.machmeier@uni-heidelberg.de>
 License: EUROPEAN UNION PUBLIC LICENCE v. 1.2
         EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined below) which is provided under the
         terms of this Licence. Any use of the Work, other than as authorised under this Licence is prohibited (to the extent such
```

### Comparing `heifip-1.0.0/README.md` & `heifip-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/extractor.py` & `heifip-1.1.0/heifip/extractor.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import numpy as np
 from PIL import Image as PILImage
 from scapy.all import Packet
 
 from heifip.exceptions import FIPWrongParameterException
 from heifip.images import NetworkTrafficImage
 from heifip.images.flow import FlowImage
+from heifip.images.flow_tiled_auto import FlowImageTiledAuto
+from heifip.images.flow_tiled_fixed import FlowImageTiledFixed
 from heifip.images.markovchain import (MarkovTransitionMatrixFlow,
                                        MarkovTransitionMatrixPacket)
 from heifip.images.packet import PacketImage
 from heifip.layers import PacketProcessor, PacketProcessorType
 
 
 class FIPExtractor:
@@ -116,14 +118,40 @@
             if max_packets_per_flow != 0 and len(packets) > max_packets_per_flow:
                 packets = packets[:max_packets_per_flow]
 
             image = FlowImage(packets, *args)
             if self.verify(image.matrix, min_image_dim, max_image_dim, remove_duplicates):
                 images.append(image.matrix)
 
+        elif image_type == FlowImageTiledFixed:
+            # when no file matches the preprocessing
+            if len(packets) == 0 or len(packets) < min_packets_per_flow:
+                return images
+
+            # cut packets when too many are there
+            if max_packets_per_flow != 0 and len(packets) > max_packets_per_flow:
+                packets = packets[:max_packets_per_flow]
+
+            image = FlowImageTiledFixed(packets, *args)
+            if self.verify(image.matrix, min_image_dim, max_image_dim, remove_duplicates):
+                images.append(image.matrix)
+
+        elif image_type == FlowImageTiledAuto:
+            # when no file matches the preprocessing
+            if len(packets) == 0 or len(packets) < min_packets_per_flow:
+                return images
+
+            # cut packets when too many are there
+            if max_packets_per_flow != 0 and len(packets) > max_packets_per_flow:
+                packets = packets[:max_packets_per_flow]
+
+            image = FlowImageTiledAuto(packets, *args)
+            if self.verify(image.matrix, min_image_dim, max_image_dim, remove_duplicates):
+                images.append(image.matrix)
+
         elif image_type  == PacketImage:
 
             for packet in packets:
                 image = PacketImage(packet, *args)
                 if self.verify(image.matrix, min_image_dim, max_image_dim, remove_duplicates):
                     images.append(image.matrix)
 
@@ -144,18 +172,23 @@
             for packet in packets:
                 image = MarkovTransitionMatrixPacket(packet, *args)
                 if self.verify(image.matrix, min_image_dim, max_image_dim, remove_duplicates):
                     images.append(image.matrix)
         else:
             raise FIPWrongParameterException
 
+        return images
+
     def save_image(self, img, output_dir):
         pil_img = PILImage.fromarray(self.convert(img, 0, 255, np.uint8))
         if not os.path.exists(os.path.realpath(os.path.dirname(output_dir))):
-            os.makedirs(os.path.realpath(os.path.dirname(output_dir)))
+            try:
+                os.makedirs(os.path.realpath(os.path.dirname(output_dir)))
+            except:
+                pass
         pil_img.save(f"{output_dir}_processed.png")
 
     def convert(self, img, target_type_min, target_type_max, target_type):
         imin = img.min()
         imax = img.max()
 
         a = (target_type_max - target_type_min) / (imax - imin)
```

### Comparing `heifip-1.0.0/heifip/images/flow.py` & `heifip-1.1.0/heifip/images/flow_tiled_auto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,75 +3,29 @@
 
 import numpy as np
 from scapy.all import Packet, raw
 
 from heifip.images import NetworkTrafficImage
 
 
-class FlowImage(NetworkTrafficImage):
+class FlowImageTiledAuto(NetworkTrafficImage):
     def __init__(
         self,
         packets,
-        dim=8,
+        dim=16,
         fill=0,
-        width=128,
-        tiled=False,
         auto_dim=False,
-        append=False,
     ) -> None:
         NetworkTrafficImage.__init__(self, fill, dim)
-        self.width = width
         self.packets = packets
         self.auto_dim = auto_dim
-        self.matrix, self.binaries = (
-            self.__get_matrix_tiled(self.dim, self.auto_dim, packets)
-            if tiled
-            else self.__get_matrix(append, packets)
-        )
+        self.matrix, self.binaries = self.__get_matrix_tiled(self.fill, self.dim, self.auto_dim, packets)
         del packets
-        
 
-    def __tile_images(self, images, cols):
-        """Tile images of same size to grid with given number of columns.
-
-        Args:
-            images (collection of ndarrays)
-            cols (int): number of colums
-
-        Returns:
-            ndarray: stitched image
-        """
-        logging.debug("Building tiled image")
-        images = iter(images)
-        first = True
-        rows = []
-        i = 0
-        while True:
-            try:
-                im = next(images)
-                logging.debug(f"add image, shape: {im.shape}, type: {im.dtype}")
-            except StopIteration:
-                if first:
-                    break
-                else:
-                    im = np.zeros_like(im)  # black background
-            if first:
-                row = im  # start next row
-                first = False
-            else:
-                row = np.concatenate((row, im), axis=1)  # append to row
-            i += 1
-            if not i % cols:
-                logging.debug(f"row done, shape: {row.shape}")
-                rows.append(row)  # finished row
-                first = True
-        tiled = np.concatenate(rows)  # stitch rows
-        return tiled
-
-    def __get_matrix_tiled(self, dim: int, auto_dim: bool, packets: [Packet]):
+    def __get_matrix_tiled(self, fill: int, dim: int, auto_dim: bool, packets: [Packet]):
         """
             Creates a matrix of a list of Scapy Packet.
             Packets are tiled into a quadratic representation.
         """
         binaries = []
         for packet in self.packets:
             # get Hex data
@@ -85,46 +39,51 @@
         # Get dim of packet, using auto_dim uses the largest packet as dim reference
         if auto_dim:
             dim = int(np.ceil(np.sqrt(length)))
 
         result = []
         for x in binaries:
             x = x[: dim * dim]
-            x = np.array(x + [self.fill] * (dim * dim - len(x)))
+            x = np.array(x + [fill] * (dim * dim - len(x)))
             x = x.reshape(dim, dim)
             result.append(x)
 
         # Get size of total image
         length_total = len(result)
         dim_total = int(np.ceil(np.sqrt(length_total)))
+        # dim_total = 4
 
         # Create tiled image
-        fh = self.__tile_images(result, dim_total)
+        fh = self.__tile_images(result, dim_total, dim)
         # Convert to int
         fh = np.uint8(fh)
         return fh, binaries
 
-    def __get_matrix(self, append: bool, packets: [Packet]):
-        """
-            Creates a matrix of a list of Scapy Packet.
-        """
-        binaries = []
-        for packet in self.packets:
-            # get Hex data
-            hexst = binascii.hexlify(raw(packet.packet))
-            # Append octet as integer
-            binaries.append(
-                [int(hexst[i : i + 2], 16) for i in range(0, len(hexst), 2)]
-            )
-        fh = None
-        # Append packets after another or write each packet in a row
-        if append:
-            fh = np.concatenate([np.array(xi) for xi in binaries])
-            rn = len(fh) // self.width
-            fh = np.reshape(fh[: rn * self.width], (-1, self.width))
-        else:
-            length = max(map(len, binaries))
-            fh = np.array([xi + [255] * (length - len(xi)) for xi in binaries])
+    def __tile_images(self, images, cols: int, dim: int):
+        """Tile images of same size to grid with given number of columns.
 
-        fh = np.uint8(fh)
+        Args:
+            images (collection of ndarrays)
+            cols (int): number of colums
 
-        return fh, binaries
+        Returns:
+            ndarray: stitched image
+        """
+        k = 0
+        rows = []
+        for i in range(0, cols):
+            row = None
+            for j in range(0, cols):
+                if len(images) > k:
+                    im = images[k]
+                else:
+                    im = np.zeros((dim, dim))
+                
+                if row is None:
+                    row = im
+                else:
+                    row = np.concatenate((row, im), axis=1)
+                k += 1
+            rows.append(row)
+        tiled = np.concatenate(rows)
+
+        return tiled
```

### Comparing `heifip-1.0.0/heifip/images/markovchain.py` & `heifip-1.1.0/heifip/images/flow_tiled_fixed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,80 @@
+import binascii
 import logging
 
 import numpy as np
-from scapy.all import Packet, chexdump, hexdump, raw
+from scapy.all import Packet, raw
 
 from heifip.images import NetworkTrafficImage
 
 
-class MarkovTransitionMatrix(NetworkTrafficImage):
+class FlowImageTiledFixed(NetworkTrafficImage):
     def __init__(
         self,
+        packets,
+        dim=16,
+        fill=0,
+        cols=3,
     ) -> None:
-        NetworkTrafficImage.__init__(self)
-
-    def bit_array(self, packet):
-        bytes_as_bits =  ''.join(format(byte, '08b') for byte in bytes(packet.packet))
-        transition = []
-        for i in range(0, len(bytes_as_bits), 4):
-            transition.append(int(bytes_as_bits[i:i+4], 2))
-        return transition
-
-    def transition_matrix(self, transitions):
-        n = 16
-
-        M = [[0]*n for _ in range(n)]
-
-        for (i,j) in zip(transitions,transitions[1:]):
-            M[i][j] += 1
-
-        #now convert to probabilities:
-        for row in M:
-            s = sum(row)
-            if s > 0:
-                row[:] = [f/s for f in row]
-        return M
+        NetworkTrafficImage.__init__(self, fill, dim)
+        self.packets = packets
+        self.cols = cols
+        self.matrix, self.binaries = self.__get_matrix_tiled(self.fill, self.dim, self.cols, packets)
+        del packets
 
-class MarkovTransitionMatrixFlow(MarkovTransitionMatrix):
-    def __init__(
-        self,
-        packets: [Packet],
-    ) -> None:
-        MarkovTransitionMatrix.__init__(self)
+    def __get_matrix_tiled(self, fill: int, dim: int, cols: int, packets: [Packet]):
+        """
+            Creates a matrix of a list of Scapy Packet.
+            Packets are tiled into a quadratic representation.
+        """
+        binaries = []
+        for packet in self.packets:
+            # get Hex data
+            hexst = binascii.hexlify(raw(packet.packet))
+            # Append octet as integer
+            binaries.append(
+                [int(hexst[i : i + 2], 16) for i in range(0, len(hexst), 2)]
+            )
 
         result = []
-        for packet in packets:
-            transition = self.bit_array(packet)
-            m = self.transition_matrix(transition)
-            result.append(np.array(m))
-
-        # Get size of total image
-        length_total = len(result)
-        dim_total = int(np.ceil(np.sqrt(length_total)))
+        for x in binaries:
+            x = x[: dim * dim]
+            x = np.array(x + [fill] * (dim * dim - len(x)))
+            x = x.reshape(dim, dim)
+            result.append(x)
+
         # Create tiled image
-        fh = self.__tile_images(result, dim_total)
+        fh = self.__tile_images(result, cols, dim)
         # Convert to int
-        self.matrix = fh
-        del packets
+        fh = np.uint8(fh)
+        return fh, binaries
 
-    def __tile_images(self, images, cols):
+    def __tile_images(self, images, cols: int, dim: int):
         """Tile images of same size to grid with given number of columns.
 
         Args:
             images (collection of ndarrays)
             cols (int): number of colums
 
         Returns:
             ndarray: stitched image
         """
-        logging.debug("Building tiled image")
-        images = iter(images)
-        first = True
+        k = 0
         rows = []
-        i = 0
-        while True:
-            try:
-                im = next(images)
-                logging.debug(f"add image, shape: {im.shape}, type: {im.dtype}")
-            except StopIteration:
-                if first:
-                    break
+        for i in range(0, cols):
+            row = None
+            for j in range(0, cols):
+                if len(images) > k:
+                    im = images[k]
                 else:
-                    im = np.zeros_like(im)  # black background
-            if first:
-                row = im  # start next row
-                first = False
-            else:
-                row = np.concatenate((row, im), axis=1)  # append to row
-            i += 1
-            if not i % cols:
-                logging.debug(f"row done, shape: {row.shape}")
-                rows.append(row)  # finished row
-                first = True
-        tiled = np.concatenate(rows)  # stitch rows
-        return tiled
-
-class MarkovTransitionMatrixPacket(MarkovTransitionMatrix):
-    def __init__(
-        self,
-        packet: Packet,
-    ) -> None:
-        MarkovTransitionMatrix.__init__(self)
-
-        transition = self.bit_array(packet)
-        m = self.transition_matrix(transition)
-        self.matrix = np.array(m)
+                    im = np.zeros((dim, dim))
+                
+                if row is None:
+                    row = im
+                else:
+                    row = np.concatenate((row, im), axis=1)
+                k += 1
+                
+            rows.append(row)
+        tiled = np.concatenate(rows)
 
-        del packet
+        return tiled
```

### Comparing `heifip-1.0.0/heifip/images/packet.py` & `heifip-1.1.0/heifip/images/packet.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,28 +13,28 @@
         packet: Packet,
         dim=8,
         fill=0,
         auto_dim=False
     ) -> None:
         NetworkTrafficImage.__init__(self, fill, dim)
         self.auto_dim = auto_dim
-        self.matrix, self.binaries = self.__get_matrix(self.dim, self.auto_dim, packet)
+        self.matrix, self.binaries = self.__get_matrix(self.dim, self.auto_dim, self.fill, packet)
 
         del packet
 
-    def __get_matrix(self, dim: int, auto_dim: int, packet: Packet):
+    def __get_matrix(self, dim: int, auto_dim: int, fill: int, packet: Packet):
         # get Hex data
         hexst = binascii.hexlify(raw(packet.packet))
         # Append octet as integer
         binaries = [int(hexst[i: i + 2], 16) for i in range(0, len(hexst), 2)]
         # Get min dim
         length = len(binaries)
         if auto_dim:
             dim = int(np.ceil(np.sqrt(length)))
 
         # Create array and shape it to dim
-        fh = np.array(binaries + [self.fill] * (self.dim * self.dim - len(binaries)))
-        fh = fh[0:self.dim * self.dim].reshape(self.dim, self.dim)
+        fh = np.array(binaries + [fill] * (dim * dim - len(binaries)))
+        fh = fh[0:dim * dim].reshape(dim, dim)
 
         fh = np.uint8(fh)
 
         return fh, binaries
```

### Comparing `heifip-1.0.0/heifip/layers/__init__.py` & `heifip-1.1.0/heifip/layers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from heifip.layers.packet import EtherPacket, FIPPacket, UnknownPacket
 from heifip.layers.transport import TransportPacket
 
 __author__ = "Stefan Machmeier"
 __copyright__ = "Copyright 2023, heiFIP"
 __credits__ = ["Manuel Trageser"]
 __license__ = "EUPL"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __maintainer__ = "Stefan Machmeier"
 __email__ = "stefan.machmeier@uni-heidelberg.de"
 __status__ = "Production"
 
 SUPPORTED_HEADERS = [IP, IPv6, DNS, HTTPRequest, HTTPResponse, TCP, UDP]
```

### Comparing `heifip-1.0.0/heifip/layers/dns.py` & `heifip-1.1.0/heifip/layers/dns.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/layers/http.py` & `heifip-1.1.0/heifip/layers/http.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/layers/ip.py` & `heifip-1.1.0/heifip/layers/ip.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/layers/packet.py` & `heifip-1.1.0/heifip/layers/packet.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/layers/transport.py` & `heifip-1.1.0/heifip/layers/transport.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/main.py` & `heifip-1.1.0/heifip/main.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/plugins/header.py` & `heifip-1.1.0/heifip/plugins/header.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip/protocols/ssh.py` & `heifip-1.1.0/heifip/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `heifip-1.0.0/heifip.egg-info/PKG-INFO` & `heifip-1.1.0/heifip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heifip
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool to convert network traffic into images for ML use cases.
 Author-email: Stefan Machmeier <stefan.machmeier@uni-heidelberg.de>
 License: EUROPEAN UNION PUBLIC LICENCE v. 1.2
         EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined below) which is provided under the
         terms of this Licence. Any use of the Work, other than as authorised under this Licence is prohibited (to the extent such
```

### Comparing `heifip-1.0.0/heifip.egg-info/SOURCES.txt` & `heifip-1.1.0/heifip.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 heifip.egg-info/SOURCES.txt
 heifip.egg-info/dependency_links.txt
 heifip.egg-info/entry_points.txt
 heifip.egg-info/top_level.txt
 heifip/exceptions/__init__.py
 heifip/images/__init__.py
 heifip/images/flow.py
+heifip/images/flow_tiled_auto.py
+heifip/images/flow_tiled_fixed.py
 heifip/images/markovchain.py
 heifip/images/packet.py
 heifip/layers/__init__.py
 heifip/layers/dns.py
 heifip/layers/http.py
 heifip/layers/ip.py
 heifip/layers/packet.py
```

### Comparing `heifip-1.0.0/pyproject.toml` & `heifip-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=62.0.0" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "heifip"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Stefan Machmeier", email="stefan.machmeier@uni-heidelberg.de" },
 ]
 description = "A tool to convert network traffic into images for ML use cases."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -49,15 +49,15 @@
 exclude = [
     "test*",
     "assets*",
 ]
 
 [tool.poetry]
 name = "heiFIP"
-version = "1.0.0"
+version = "1.1.0"
 description = "A tool to convert network traffic into images for ML use cases."
 license = "EUPL-1.2"
 authors = ["Stefan Machmeier"]
 
 [[tool.poetry_bumpversion.replacements]]
 files = ["heifip/__init__.py", "heifip/exceptions/__init__.py", "heifip/images/__init__.py", "heifip/layers/__init__.py", "heifip/plugins/__init__.py", "heifip/protocols/__init__.py"]
 search = '__version__ = "{current_version}"'
```

