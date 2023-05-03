# Comparing `tmp/slippistats-0.1.0.tar.gz` & `tmp/slippistats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippistats-0.1.0.tar", last modified: Fri Apr 28 04:47:26 2023, max compression
+gzip compressed data, was "slippistats-0.1.1.tar", last modified: Wed May  3 00:09:23 2023, max compression
```

## Comparing `slippistats-0.1.0.tar` & `slippistats-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.827221 slippistats-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4969 2023-04-28 04:47:26.826220 slippistats-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3238 2023-04-28 04:38:04.000000 slippistats-0.1.0/README.md
--rw-rw-rw-   0        0        0      605 2023-04-28 04:28:48.000000 slippistats-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 04:47:26.827221 slippistats-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-04-25 21:47:20.000000 slippistats-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.771710 slippistats-0.1.0/slippistats/
--rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.0/slippistats/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.0/slippistats/controller.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.805716 slippistats-0.1.0/slippistats/enums/
--rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.0/slippistats/enums/__init__.py
--rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/enums/attack.py
--rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/enums/character.py
--rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/enums/item.py
--rw-rw-rw-   0        0        0     3309 2023-04-26 00:48:25.000000 slippistats-0.1.0/slippistats/enums/stage.py
--rw-rw-rw-   0        0        0    51488 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/enums/state.py
--rw-rw-rw-   0        0        0    61534 2023-04-25 21:47:23.000000 slippistats-0.1.0/slippistats/event.py
--rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/game.py
--rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/log.py
--rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/metadata.py
--rw-rw-rw-   0        0        0    12529 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/parse.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.819718 slippistats-0.1.0/slippistats/stats/
--rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/stats/__init__.py
--rw-rw-rw-   0        0        0    14153 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/stats/combo_computer.py
--rw-rw-rw-   0        0        0    17798 2023-04-25 21:47:23.000000 slippistats-0.1.0/slippistats/stats/common.py
--rw-rw-rw-   0        0        0    11145 2023-04-25 21:47:23.000000 slippistats-0.1.0/slippistats/stats/computer.py
--rw-rw-rw-   0        0        0    33926 2023-04-26 01:15:54.000000 slippistats-0.1.0/slippistats/stats/stat_types.py
--rw-rw-rw-   0        0        0    35890 2023-04-27 08:10:16.000000 slippistats-0.1.0/slippistats/stats/stats_computer.py
--rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.0/slippistats/util.py
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.791714 slippistats-0.1.0/slippistats.egg-info/
--rw-rw-rw-   0        0        0     4969 2023-04-28 04:47:26.000000 slippistats-0.1.0/slippistats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-04-28 04:47:26.000000 slippistats-0.1.0/slippistats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 04:47:26.000000 slippistats-0.1.0/slippistats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-28 04:47:26.000000 slippistats-0.1.0/slippistats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-28 04:47:26.000000 slippistats-0.1.0/slippistats.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 04:47:26.823719 slippistats-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.0/test/__init__.py
--rw-rw-rw-   0        0        0    16245 2023-04-25 21:47:22.000000 slippistats-0.1.0/test/replays_test.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.152197 slippistats-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5002 2023-05-03 00:09:23.106398 slippistats-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2023-05-02 01:59:46.000000 slippistats-0.1.1/README.md
+-rw-rw-rw-   0        0        0      605 2023-05-03 00:08:40.000000 slippistats-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 00:09:23.152197 slippistats-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-04-25 21:47:20.000000 slippistats-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.047388 slippistats-0.1.1/slippistats/
+-rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.1/slippistats/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.1/slippistats/controller.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.085394 slippistats-0.1.1/slippistats/enums/
+-rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.1/slippistats/enums/__init__.py
+-rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/attack.py
+-rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/character.py
+-rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/item.py
+-rw-rw-rw-   0        0        0     3309 2023-04-26 00:48:25.000000 slippistats-0.1.1/slippistats/enums/stage.py
+-rw-rw-rw-   0        0        0    51488 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/state.py
+-rw-rw-rw-   0        0        0    61534 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/event.py
+-rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/game.py
+-rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/log.py
+-rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/metadata.py
+-rw-rw-rw-   0        0        0    12567 2023-04-28 04:58:24.000000 slippistats-0.1.1/slippistats/parse.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.099898 slippistats-0.1.1/slippistats/stats/
+-rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/stats/__init__.py
+-rw-rw-rw-   0        0        0    13781 2023-05-02 02:16:47.000000 slippistats-0.1.1/slippistats/stats/combo_computer.py
+-rw-rw-rw-   0        0        0    17798 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/stats/common.py
+-rw-rw-rw-   0        0        0    11145 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/stats/computer.py
+-rw-rw-rw-   0        0        0    33926 2023-04-26 01:15:54.000000 slippistats-0.1.1/slippistats/stats/stat_types.py
+-rw-rw-rw-   0        0        0    35890 2023-04-27 08:10:16.000000 slippistats-0.1.1/slippistats/stats/stats_computer.py
+-rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/util.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.069893 slippistats-0.1.1/slippistats.egg-info/
+-rw-rw-rw-   0        0        0     5002 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-03 00:09:23.000000 slippistats-0.1.1/slippistats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.103398 slippistats-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0    16245 2023-04-25 21:47:22.000000 slippistats-0.1.1/test/replays_test.py
```

### Comparing `slippistats-0.1.0/LICENSE.txt` & `slippistats-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/PKG-INFO` & `slippistats-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Stats library for SSBM replay files
 Home-page: https://github.com/Walnut356/py-slippi-stats
 Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
@@ -32,14 +32,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SlippiStats
 
+```pip install slippistats```
+
 Please refer to the [wiki](https://github.com/Walnut356/SlippiStats/wiki) for quick start and API reference. Also check out [StatsExamples](https://github.com/Walnut356/SlippiStats/tree/main/StatsExamples) jupyter notebooks, which contain some example stat generations from ~1400 of my own replays.
 
 SlippiStats is a Python parser for [.slp](https://github.com/project-slippi/slippi-wiki/blob/master/SPEC.md) game replay files for [Super Smash Brothers Melee](https://en.wikipedia.org/wiki/Super_Smash_Bros._Melee) for the Nintendo GameCube. These replays are generated by Jas Laferriere's [Project Slippi](https://github.com/JLaferri/project-slippi), which runs on a Wii or the [Dolphin](https://dolphin-emu.org/) emulator.
 
 ## Overview
 
 SlippiStats is a library for slippi replay parsing and automatic stat/combo generation. It is based heavily on both slippi-js and py-slippi, though with some modifications.
```

### Comparing `slippistats-0.1.0/README.md` & `slippistats-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # SlippiStats
 
+```pip install slippistats```
+
 Please refer to the [wiki](https://github.com/Walnut356/SlippiStats/wiki) for quick start and API reference. Also check out [StatsExamples](https://github.com/Walnut356/SlippiStats/tree/main/StatsExamples) jupyter notebooks, which contain some example stat generations from ~1400 of my own replays.
 
 SlippiStats is a Python parser for [.slp](https://github.com/project-slippi/slippi-wiki/blob/master/SPEC.md) game replay files for [Super Smash Brothers Melee](https://en.wikipedia.org/wiki/Super_Smash_Bros._Melee) for the Nintendo GameCube. These replays are generated by Jas Laferriere's [Project Slippi](https://github.com/JLaferri/project-slippi), which runs on a Wii or the [Dolphin](https://dolphin-emu.org/) emulator.
 
 ## Overview
 
 SlippiStats is a library for slippi replay parsing and automatic stat/combo generation. It is based heavily on both slippi-js and py-slippi, though with some modifications.
```

### Comparing `slippistats-0.1.0/pyproject.toml` & `slippistats-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2273 6c69 7070 6973  .name = "slippis
 00000070: 7461 7473 220d 0a61 7574 686f 7273 203d  tats"..authors =
 00000080: 205b 0d0a 2020 2020 7b6e 616d 6520 3d20   [..    {name = 
 00000090: 2257 616c 6e75 7433 3536 222c 2065 6d61  "Walnut356", ema
 000000a0: 696c 203d 2022 7761 6c6e 7574 3335 3640  il = "walnut356@
 000000b0: 676d 6169 6c2e 636f 6d22 7d0d 0a5d 0d0a  gmail.com"}..]..
-000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e30  version = "0.1.0
+000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e31  version = "0.1.1
 000000d0: 220d 0a64 6570 656e 6465 6e63 6965 7320  "..dependencies 
 000000e0: 3d20 5b0d 0a20 2020 2022 7079 2d75 626a  = [..    "py-ubj
 000000f0: 736f 6e7e 3d30 2e31 3622 2c0d 0a20 2020  son~=0.16",..   
 00000100: 2022 747a 6c6f 6361 6c7e 3d34 2e33 222c   "tzlocal~=4.3",
 00000110: 0d0a 2020 2020 2270 6f6c 6172 737e 3d30  ..    "polars~=0
 00000120: 2e31 372e 3922 2c0d 0a5d 0d0a 636c 6173  .17.9",..]..clas
 00000130: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..
```

### Comparing `slippistats-0.1.0/setup.py` & `slippistats-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/controller.py` & `slippistats-0.1.1/slippistats/controller.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/enums/attack.py` & `slippistats-0.1.1/slippistats/enums/attack.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/enums/character.py` & `slippistats-0.1.1/slippistats/enums/character.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/enums/item.py` & `slippistats-0.1.1/slippistats/enums/item.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/enums/stage.py` & `slippistats-0.1.1/slippistats/enums/stage.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/enums/state.py` & `slippistats-0.1.1/slippistats/enums/state.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/event.py` & `slippistats-0.1.1/slippistats/event.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/game.py` & `slippistats-0.1.1/slippistats/game.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/metadata.py` & `slippistats-0.1.1/slippistats/metadata.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/parse.py` & `slippistats-0.1.1/slippistats/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             log.info("ignoring unknown event type: 0x%02x" % code)
 
     # log.debug(f'event payload sizes: {sizes}')
     return (2 + this_size, sizes)
 
 
 # This essentially acts as a jump table in _parse_event,
-# saves a lot of processing on a potentially very hot match statement and enum call
+# saves a lot of processing (~15% over py-slippi) on a very hot match statement and enum call
 # If python was compiled, this would probably be unnecessary.
 EVENT_PARSE_DISPATCH = {
     EventType.GAME_START: lambda stream: Start._parse(stream),
     EventType.FRAME_START: lambda stream: Frame.Event(Frame.Event.Id(stream), Frame.Event.Type.START, stream),
     EventType.FRAME_PRE: lambda stream: Frame.Event(Frame.Event.PortId(stream), Frame.Event.Type.PRE, stream),
     EventType.FRAME_POST: lambda stream: Frame.Event(Frame.Event.PortId(stream), Frame.Event.Type.POST, stream),
     EventType.ITEM: lambda stream: Frame.Event(Frame.Event.Id(stream), Frame.Event.Type.ITEM, stream),
@@ -280,14 +280,15 @@
     handlers,
     *_,
 ):
     handlers[End](event)
     return current_frame
 
 
+# _parse_events jump table
 BUILD_GAME_DISPATCH = {
     EventType.GAME_START: _game_start,
     EventType.FRAME_START: _start_frame,
     EventType.FRAME_PRE: _pre_frame,
     EventType.FRAME_POST: _post_frame,
     EventType.ITEM: _item_frame,
     EventType.FRAME_END: _end_frame,
```

### Comparing `slippistats-0.1.0/slippistats/stats/combo_computer.py` & `slippistats-0.1.1/slippistats/stats/combo_computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,17 @@
 
     def reset_data(self):
         self.combos = []
         self.combo_state = ComboState()
         self.queue = []
 
     def to_json(self, combo: ComboData):
+        self.queue.append({})
         self.queue[-1]["path"] = self.replay_path
-        self.queue[-1]["gameStartAt"] = getattr(
-            getattr(self, "metadata"), "date"
-        ).strftime("%m/%d/%y %I:%M %p")
+        self.queue[-1]["gameStartAt"] = self.replay.metadata.date.strftime("%m/%d/%y %I:%M %p")
         self.queue[-1]["startFrame"] = combo.start_frame - PRE_COMBO_BUFFER_FRAMES
         self.queue[-1]["endFrame"] = combo.end_frame + POST_COMBO_BUFFER_FRAMES
         return self.queue
 
     def combo_compute(
         self,
         connect_code: str | None = None,
@@ -148,17 +147,15 @@
         shield_break_check=True,
         ledge_check=True,
     ) -> list[ComboData]:
         """Generates list of combos from the replay information parsed using prime_replay(), returns nothing.
         Output is also accessible as a list through ComboComputer.combos"""
 
         if connect_code is None and player is None:
-            raise ValueError(
-                "Combo compute functions require either a connect_code or player and opponent argument"
-            )
+            raise ValueError("Combo compute functions require either a connect_code or player and opponent argument")
 
         if connect_code is not None:
             player = self.get_player(connect_code)
             opponent = self.get_opponent(connect_code)
 
         for i, player_frame in enumerate(player.frames):
             player_state: ActionState | int = player_frame.post.state
@@ -166,45 +163,36 @@
 
             opponent_frame: Frame.Port.Data = opponent.frames[i]
             opnt_action_state = opponent_frame.post.state
             prev_opponent_frame: Frame.Port.Data = opponent.frames[i - 1]
 
             opnt_is_damaged = is_damaged(opnt_action_state)
             # Bitflags are used because the hitstun frame count is used for a bunch of other things as well
-            opnt_is_in_hitstun = (
-                is_in_hitstun(opponent_frame.post.flags) and hitstun_check
-            )
+            opnt_is_in_hitstun = is_in_hitstun(opponent_frame.post.flags) and hitstun_check
             opnt_is_grabbed = is_grabbed(opnt_action_state)
             opnt_is_cmd_grabbed = is_cmd_grabbed(opnt_action_state)
-            opnt_damage_taken = calc_damage_taken(opponent_frame, prev_opponent_frame)
+            opnt_damage_taken = calc_damage_taken(opponent_frame.post, prev_opponent_frame.post)
 
             # "Keep track of whether actionState changes after a hit. Used to compute move count
             # When purely using action state there was a bug where if you did two of the same
             # move really fast (such as ganon's jab), it would count as one move. Added
             # the actionStateCounter at this point which counts the number of frames since
             # an animation started. Should be more robust, for old files it should always be
             # null and null < null = false" - official parser
-            action_changed_since_hit = not (
-                player_state == self.combo_state.last_hit_animation
-            )
+            action_changed_since_hit = not (player_state == self.combo_state.last_hit_animation)
             action_frame_counter = player_frame.post.state_age
             prev_action_counter = prev_player_frame.post.state_age
             action_state_reset = action_frame_counter < prev_action_counter
             if action_changed_since_hit or action_state_reset:
                 self.combo_state.last_hit_animation = None
 
             # I throw in the extra hitstun check to make it extra robust in case we're forgetting some animation.
             # Don't include hitlag check unless you want shield hits to start combo events.
             # There might be false positives on self damage like fully charged roy neutral b
-            if (
-                opnt_is_damaged
-                or opnt_is_grabbed
-                or opnt_is_cmd_grabbed
-                or opnt_is_in_hitstun
-            ):
+            if opnt_is_damaged or opnt_is_grabbed or opnt_is_cmd_grabbed or opnt_is_in_hitstun:
                 # if the opponent has been hit and there's no "active" combo, start a new combo
                 if self.combo_state.combo is None:
                     self.combo_state.combo = ComboData(
                         player_stocks=player_frame.post.stocks_remaining,
                         opponent_stocks=opponent_frame.post.stocks_remaining,
                         start_frame=i - 123,
                         start_percent=prev_opponent_frame.post.percent,
@@ -237,46 +225,37 @@
                 continue
 
             # Otherwise check all other relevant statistics and determine whether to continue or terminate the combo
             opnt_is_in_hitlag = is_in_hitlag(opponent_frame.post.flags) and hitlag_check
             opnt_is_teching = is_teching(opnt_action_state) and tech_check
             opnt_is_downed = is_downed(opnt_action_state) and downed_check
             opnt_is_dying = is_dying(opnt_action_state)
-            opnt_is_offstage = (
-                is_offstage(opponent_frame.post.position, self.replay.start.stage)
-                and offstage_check
-            )
+            opnt_is_offstage = is_offstage(opponent_frame.post.position, self.replay.start.stage) and offstage_check
             opnt_is_dodging = (
                 is_dodging(opnt_action_state)
                 and dodge_check
-                and not is_wavedashing(
-                    opnt_action_state, opponent.port, i, opponent.frames
-                )
+                and not is_wavedashing(opnt_action_state, i, opponent.frames)
             )
             opnt_is_shielding = is_shielding(opnt_action_state) and shield_check
-            opnt_is_shield_broken = (
-                is_shield_broken(opnt_action_state) and shield_break_check
-            )
-            opnt_did_lose_stock = did_lose_stock(opponent_frame, prev_opponent_frame)
+            opnt_is_shield_broken = is_shield_broken(opnt_action_state) and shield_break_check
+            opnt_did_lose_stock = did_lose_stock(opponent_frame.post, prev_opponent_frame.post)
             opnt_is_ledge_action = is_ledge_action(opnt_action_state) and ledge_check
             opnt_is_maybe_juggled = is_maybe_juggled(
                 opponent_frame.post.position,
-                getattr(opponent_frame, "is_airborne"),
+                getattr(opponent_frame.post, "is_airborne"),
                 self.replay.start.stage,
             )  # TODO and juggled check
             opnt_is_special_fall = is_special_fall(opnt_action_state)
-            opnt_is_upb_lag = is_upb_lag(
-                opnt_action_state, prev_opponent_frame.post.state
-            )
+            opnt_is_upb_lag = is_upb_lag(opnt_action_state, prev_opponent_frame.post.state)
             # opnt_is_recovery_lag = is_recovery_lag(opponent_frame.character, opnt_action_state)
 
             if not opnt_did_lose_stock:
                 self.combo_state.combo.current_percent = opponent_frame.post.percent
 
-            player_did_lose_stock = did_lose_stock(player_frame, prev_player_frame)
+            player_did_lose_stock = did_lose_stock(player_frame.post, prev_player_frame.post)
 
             # reset the combo timeout timer to 0 if the opponent meets the following conditions
             # list expanded from official parser to allow for higher combo variety
             #  and captures more of what we would count as "combos"
             # noteably, this list will allow mid-combo shield pressure and edgeguards to be counted as part of a combo
             if (
                 opnt_is_damaged
@@ -300,17 +279,15 @@
             else:
                 self.combo_state.reset_counter += 1
 
             should_terminate = False
 
             # All combo termination checks below
             if opnt_is_dying:
-                self.combo_state.combo.death_direction = get_death_direction(
-                    opnt_action_state
-                )
+                self.combo_state.combo.death_direction = get_death_direction(opnt_action_state)
 
             if opnt_did_lose_stock:
                 self.combo_state.combo.did_kill = True
                 if opponent_frame.post.stocks_remaining == 0:
                     self.combo_state.combo.did_end_game = True
 
                 should_terminate = True
@@ -318,12 +295,11 @@
             if self.combo_state.reset_counter > COMBO_LENIENCY or player_did_lose_stock:
                 should_terminate = True
 
             # If the combo should end, finalize the values, reset the temp storage
             if should_terminate:
                 self.combo_state.combo.end_frame = i - 123
                 self.combo_state.combo.end_percent = prev_opponent_frame.post.percent
-
                 self.combo_state.combo = None
                 self.combo_state.move = None
 
         return player.combos
```

### Comparing `slippistats-0.1.0/slippistats/stats/common.py` & `slippistats-0.1.1/slippistats/stats/common.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/stats/computer.py` & `slippistats-0.1.1/slippistats/stats/computer.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/stats/stat_types.py` & `slippistats-0.1.1/slippistats/stats/stat_types.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/stats/stats_computer.py` & `slippistats-0.1.1/slippistats/stats/stats_computer.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats/util.py` & `slippistats-0.1.1/slippistats/util.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/slippistats.egg-info/PKG-INFO` & `slippistats-0.1.1/slippistats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Stats library for SSBM replay files
 Home-page: https://github.com/Walnut356/py-slippi-stats
 Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
@@ -32,14 +32,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SlippiStats
 
+```pip install slippistats```
+
 Please refer to the [wiki](https://github.com/Walnut356/SlippiStats/wiki) for quick start and API reference. Also check out [StatsExamples](https://github.com/Walnut356/SlippiStats/tree/main/StatsExamples) jupyter notebooks, which contain some example stat generations from ~1400 of my own replays.
 
 SlippiStats is a Python parser for [.slp](https://github.com/project-slippi/slippi-wiki/blob/master/SPEC.md) game replay files for [Super Smash Brothers Melee](https://en.wikipedia.org/wiki/Super_Smash_Bros._Melee) for the Nintendo GameCube. These replays are generated by Jas Laferriere's [Project Slippi](https://github.com/JLaferri/project-slippi), which runs on a Wii or the [Dolphin](https://dolphin-emu.org/) emulator.
 
 ## Overview
 
 SlippiStats is a library for slippi replay parsing and automatic stat/combo generation. It is based heavily on both slippi-js and py-slippi, though with some modifications.
```

### Comparing `slippistats-0.1.0/slippistats.egg-info/SOURCES.txt` & `slippistats-0.1.1/slippistats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.0/test/replays_test.py` & `slippistats-0.1.1/test/replays_test.py`

 * *Files identical despite different names*

