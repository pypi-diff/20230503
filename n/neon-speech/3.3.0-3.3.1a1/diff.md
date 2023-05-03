# Comparing `tmp/neon_speech-3.3.0-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23506 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-20 02:17 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2632 b- defN 23-Apr-20 02:17 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-Apr-20 02:17 neon_speech/cli.py
--rw-r--r--  2.0 unx     9996 b- defN 23-Apr-20 02:17 neon_speech/listener.py
--rw-r--r--  2.0 unx     4810 b- defN 23-Apr-20 02:17 neon_speech/mic.py
--rw-r--r--  2.0 unx    21837 b- defN 23-Apr-20 02:17 neon_speech/service.py
--rw-r--r--  2.0 unx     4396 b- defN 23-Apr-20 02:17 neon_speech/stt.py
--rw-r--r--  2.0 unx     4294 b- defN 23-Apr-20 02:17 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2544 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      112 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1131 b- defN 23-Apr-20 02:17 neon_speech-3.3.0.dist-info/RECORD
-14 files, 60406 bytes uncompressed, 21638 bytes compressed:  64.2%
+Zip file size: 23633 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-03 01:57 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2632 b- defN 23-May-03 01:57 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-May-03 01:57 neon_speech/cli.py
+-rw-r--r--  2.0 unx     9996 b- defN 23-May-03 01:57 neon_speech/listener.py
+-rw-r--r--  2.0 unx     5115 b- defN 23-May-03 01:57 neon_speech/mic.py
+-rw-r--r--  2.0 unx    21837 b- defN 23-May-03 01:57 neon_speech/service.py
+-rw-r--r--  2.0 unx     4396 b- defN 23-May-03 01:57 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4294 b- defN 23-May-03 01:57 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2551 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-May-03 01:57 neon_speech-3.3.1a1.dist-info/RECORD
+14 files, 60729 bytes uncompressed, 21741 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/LICENSE.md
+Filename: neon_speech-3.3.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/METADATA
+Filename: neon_speech-3.3.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/WHEEL
+Filename: neon_speech-3.3.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/entry_points.txt
+Filename: neon_speech-3.3.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/top_level.txt
+Filename: neon_speech-3.3.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.0.dist-info/RECORD
+Filename: neon_speech-3.3.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/mic.py

```diff
@@ -22,21 +22,20 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from mycroft.audio import is_speaking
-from mycroft.client.speech.mic import get_silence, ResponsiveRecognizer
-from neon_utils import LOG
+from ovos_utils.log import LOG
 from speech_recognition import AudioSource, AudioData
-
 from neon_transformers.audio_transformers import AudioTransformersService
 
+from mycroft.client.speech.mic import ResponsiveRecognizer
+
 
 class NeonResponsiveRecognizer(ResponsiveRecognizer):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._in_speech = False
         self.audio_consumers = AudioTransformersService(self.loop.bus,
@@ -67,14 +66,24 @@
         For example when we are in a dialog with the user.
         """
         if self._listen_triggered:
             self._listen_triggered = False
             return True
         return False
 
+    def feed_hotwords(self, chunk):
+        try:
+            if len(self.loop.hot_words) < 1:
+                raise RuntimeWarning("No hotword engines configured!")
+            ResponsiveRecognizer.feed_hotwords(self, chunk)
+        except Exception as e:
+            LOG.exception(e)
+            self.stop()
+            self.loop.needs_reload = True
+
     def check_for_hotwords(self, audio_data, source):
         found = False
         for ww in super().check_for_hotwords(audio_data, source):
             found = True
             yield ww
         if not found:
             self.audio_consumers.feed_audio(audio_data)
```

## Comparing `neon_speech-3.3.0.dist-info/LICENSE.md` & `neon_speech-3.3.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.0.dist-info/METADATA` & `neon_speech-3.3.1a1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.0
+Version: 3.3.1a1
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: ovos-core (~=0.0.7)
 Requires-Dist: SpeechRecognition (~=3.8)
 Requires-Dist: PyAudio (~=0.2)
 Requires-Dist: mycroft-messagebus-client (~=0.10)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: ovos-plugin-manager (~=0.0.19)
 Requires-Dist: pydub (~=0.23)
@@ -57,9 +57,7 @@
 -v ~/.config/pulse/cookie:/tmp/pulse_cookie:ro \
 -v ${XDG_RUNTIME_DIR}/pulse:${XDG_RUNTIME_DIR}/pulse:ro \
 --device=/dev/snd:/dev/snd \
 -e PULSE_SERVER=unix:${XDG_RUNTIME_DIR}/pulse/native \
 -e PULSE_COOKIE=/tmp/pulse_cookie \
 neon_speech
 ```
-
-
```

## Comparing `neon_speech-3.3.0.dist-info/RECORD` & `neon_speech-3.3.1a1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 neon_speech/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_speech/__main__.py,sha256=GYsKldh4iN7sY2kLnHtSYj1D56GQgdHuMXlUIf-d5ks,2632
 neon_speech/cli.py,sha256=2BiU-fTcmOyT3CJ6gmoCtUsP7bAUcDOt8-MkPEfMJX0,5085
 neon_speech/listener.py,sha256=Cct3GOVTrjEBUBq2pvrcDH7iixBo_6jvJCV02BeCwNE,9996
-neon_speech/mic.py,sha256=gcarKLkWfrzToACsiwRWDX5qeBizyJ0vquuqdg5EMeU,4810
+neon_speech/mic.py,sha256=6M2l1zOqR6tPYrpIVWA76R8-GUfPKtt5iwiBCfqVTdg,5115
 neon_speech/service.py,sha256=oLQ7978avvH4eGbUFWSIV1ylWFvxh7Td1UUloMKYLrk,21837
 neon_speech/stt.py,sha256=rCl2v2m1D1-t-92Me1qyA57gfw7i9jSzs7j0bQXTGOc,4396
 neon_speech/utils.py,sha256=5RNtze-kwo-_WvYNk8GoqG8vVdkbPs6hBdpF7Pn7Iqc,4294
-neon_speech-3.3.0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_speech-3.3.0.dist-info/METADATA,sha256=DNocK_h2IE1uXJwMNkVhWu0uLW7DyOGCEeWwL3q5LnE,2544
-neon_speech-3.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_speech-3.3.0.dist-info/entry_points.txt,sha256=dpTgmCJLklfefZfFO1cgx312bj5zQB6thg6j2FSJ7Xg,112
-neon_speech-3.3.0.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
-neon_speech-3.3.0.dist-info/RECORD,,
+neon_speech-3.3.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_speech-3.3.1a1.dist-info/METADATA,sha256=WbTm_35roxmsIqn-CbQtDS38xCV0lhIJWKb42DLwBD8,2551
+neon_speech-3.3.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_speech-3.3.1a1.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
+neon_speech-3.3.1a1.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
+neon_speech-3.3.1a1.dist-info/RECORD,,
```

