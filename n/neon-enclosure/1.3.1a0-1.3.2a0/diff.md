# Comparing `tmp/neon_enclosure-1.3.1a0-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.3.2a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11868 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-Mar-10 18:12 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2590 b- defN 23-Mar-10 18:12 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3580 b- defN 23-Mar-10 18:12 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1831 b- defN 23-Mar-10 18:12 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2600 b- defN 23-Mar-10 18:12 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-Mar-10 18:12 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2614 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-Mar-10 18:12 neon_enclosure-1.3.1a0.dist-info/RECORD
-12 files, 20236 bytes uncompressed, 10078 bytes compressed:  50.2%
+Zip file size: 11930 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-12 02:36 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2586 b- defN 23-Apr-12 02:36 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3580 b- defN 23-Apr-12 02:36 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Apr-12 02:36 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2535 b- defN 23-Apr-12 02:36 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2326 b- defN 23-Apr-12 02:36 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2681 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/RECORD
+12 files, 20235 bytes uncompressed, 10140 bytes compressed:  49.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/LICENSE.md
+Filename: neon_enclosure-1.3.2a0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/METADATA
+Filename: neon_enclosure-1.3.2a0.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/WHEEL
+Filename: neon_enclosure-1.3.2a0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/entry_points.txt
+Filename: neon_enclosure-1.3.2a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/top_level.txt
+Filename: neon_enclosure-1.3.2a0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.3.1a0.dist-info/RECORD
+Filename: neon_enclosure-1.3.2a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_enclosure/__main__.py

```diff
@@ -24,21 +24,21 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
-from neon_utils.messagebus_utils import get_messagebus
+from ovos_utils.messagebus import get_mycroft_bus
 
 
 def main(*args, **kwargs):
     init_config_dir()
     init_log(log_name="enclosure")
-    bus = get_messagebus()
+    bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
     init_signal_bus(bus)
     init_signal_handlers()
 
     from .service import NeonHardwareAbstractionLayer
```

## neon_enclosure/admin/__init__.py

```diff
@@ -21,7 +21,8 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
```

## neon_enclosure/admin/__main__.py

```diff
@@ -22,23 +22,22 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-# from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
-from neon_utils.messagebus_utils import get_messagebus
+from ovos_utils.messagebus import get_mycroft_bus
 
 
 def main(*args, **kwargs):
     # init_config_dir()
     init_log(log_name="admin")
-    bus = get_messagebus()
+    bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
     init_signal_bus(bus)
     init_signal_handlers()
 
     from .service import NeonAdminHardwareAbstractionLayer
```

## Comparing `neon_enclosure-1.3.1a0.dist-info/LICENSE.md` & `neon_enclosure-1.3.2a0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.3.1a0.dist-info/METADATA` & `neon_enclosure-1.3.2a0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.3.1a0
+Version: 1.3.2a0
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-PHAL (~=0.0.4)
+Requires-Dist: ovos-PHAL (>=0.0.5a4,~=0.0.4)
 Requires-Dist: neon-utils[network] (>=1.2.4,~=1.2)
+Requires-Dist: ovos-utils[extras] (>=0.0.31a11,~=0.0.30)
 Requires-Dist: ovos-core (~=0.0.5)
 Provides-Extra: docker
 Requires-Dist: ovos-phal-plugin-homeassistant (~=0.0.1) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-notification-widgets (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-color-scheme-manager (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-configuration-provider (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-dashboard (~=0.0.1) ; extra == 'docker'
```

## Comparing `neon_enclosure-1.3.1a0.dist-info/RECORD` & `neon_enclosure-1.3.2a0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_enclosure/__main__.py,sha256=UZijHi1-2hoyaCQOMI-NHQGtxS7YxNx4YEpb3jd7k3Y,2590
+neon_enclosure/__main__.py,sha256=utweyoTXU5MUVrdQHnVUWLU1kEobUp_lug8uqoRjnh0,2586
 neon_enclosure/service.py,sha256=vhCkiAEfodte8ks1Jn-Otik-jLzLOD2ko-FioBy6FiE,3580
-neon_enclosure/admin/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_enclosure/admin/__main__.py,sha256=0veUCoyNAYsxQp1WS-fdJqIpqR4ORbqdGN75t5APQWI,2600
+neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
+neon_enclosure/admin/__main__.py,sha256=23trrM05ZNp0RaWPP55SoHX9zLAbT-xaZgsj9aMj1m0,2535
 neon_enclosure/admin/service.py,sha256=p2y_n5TYBJwYpsiavH476yZB2kDksKHFH2_CO2FlBtQ,2326
-neon_enclosure-1.3.1a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.3.1a0.dist-info/METADATA,sha256=sLRLC4UAX5_udEiZ3beMIMcUzZOOOeCPPZEhyDmtorc,2614
-neon_enclosure-1.3.1a0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-neon_enclosure-1.3.1a0.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
-neon_enclosure-1.3.1a0.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.3.1a0.dist-info/RECORD,,
+neon_enclosure-1.3.2a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.3.2a0.dist-info/METADATA,sha256=qhqwK2SoSj4BN3steyvAYLI0t-foMAQzGks49KMZQGs,2681
+neon_enclosure-1.3.2a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.3.2a0.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
+neon_enclosure-1.3.2a0.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.3.2a0.dist-info/RECORD,,
```

