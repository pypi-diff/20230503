# Comparing `tmp/ogsapi-0.4.1.tar.gz` & `tmp/ogsapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.4.1.tar", last modified: Wed Apr 26 05:00:25 2023, max compression
+gzip compressed data, was "ogsapi-0.5.0.tar", last modified: Wed May  3 03:37:30 2023, max compression
```

## Comparing `ogsapi-0.4.1.tar` & `ogsapi-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.374884 ogsapi-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-26 05:00:08.000000 ogsapi-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 05:00:25.374884 ogsapi-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4998 2023-04-26 05:00:08.000000 ogsapi-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-26 05:00:08.000000 ogsapi-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 05:00:25.374884 ogsapi-0.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.369884 ogsapi-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.371884 ogsapi-0.4.1/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 05:00:08.000000 ogsapi-0.4.1/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34578 2023-04-26 05:00:08.000000 ogsapi-0.4.1/src/ogsapi/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.373884 ogsapi-0.4.1/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.497280 ogsapi-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-05-03 03:37:14.000000 ogsapi-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-05-03 03:37:30.497280 ogsapi-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2023-05-03 03:37:14.000000 ogsapi-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-03 03:37:14.000000 ogsapi-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 03:37:30.497280 ogsapi-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.492280 ogsapi-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.494280 ogsapi-0.5.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 03:37:14.000000 ogsapi-0.5.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41525 2023-05-03 03:37:14.000000 ogsapi-0.5.0/src/ogsapi/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.496280 ogsapi-0.5.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5554 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/top_level.txt
```

### Comparing `ogsapi-0.4.1/LICENSE` & `ogsapi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.4.1/PKG-INFO` & `ogsapi-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.4.1
+Version: 0.5.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +17,16 @@
 
 ## Summary
 
 An API wrapper written in python for the Online-Go Server's (OGS) REST API and Realtime (SocketIO) API
 
 **THIS IS STILL HEAVILY IN DEVELOPMENT. VERY MUCH NOT READY FOR USE**
 
+Read the documentation here for more info: https://ogs-python.dakotamarshall.net/
+
 ## Install
 
 ### Pip Package
 
 ```bash
 python3 -m pip install ogsapi
 ```
@@ -135,23 +137,23 @@
     - [ ] GET - id/games
     - [ ] GET - id/groups
     - [ ] GET - id/ladders
     - [ ] GET - id/tournaments
 - [ ] Realtime API Game Events
   - [ ] Server to Client
     - [ ] auto_resign
-    - [ ] chat
+    - [ ] chat (This is for chat rooms, low priority)
     - [ ] chat/remove
     - [ ] clear_auto_resign
     - [x] clock
     - [ ] conditional_moves
-    - [ ] error
+    - [x] error
     - [x] gamedata
     - [x] latency
-    - [ ] phase
+    - [x] phase
     - [ ] removed_stones
     - [ ] removed_stones_accepted
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
@@ -174,10 +176,10 @@
     - [ ] removed_stones/set
     - [x] resign
     - [ ] resume
     - [ ] timed_out
     - [x] undo/accept
     - [ ] undo/cancel
     - [ ] undo/request
-- [ ] Implement proper challenge creation
-- [ ] Create open challenge
+- [x] Implement proper challenge creation
+- [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

### Comparing `ogsapi-0.4.1/README.md` & `ogsapi-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 ## Summary
 
 An API wrapper written in python for the Online-Go Server's (OGS) REST API and Realtime (SocketIO) API
 
 **THIS IS STILL HEAVILY IN DEVELOPMENT. VERY MUCH NOT READY FOR USE**
 
+Read the documentation here for more info: https://ogs-python.dakotamarshall.net/
+
 ## Install
 
 ### Pip Package
 
 ```bash
 python3 -m pip install ogsapi
 ```
@@ -123,23 +125,23 @@
     - [ ] GET - id/games
     - [ ] GET - id/groups
     - [ ] GET - id/ladders
     - [ ] GET - id/tournaments
 - [ ] Realtime API Game Events
   - [ ] Server to Client
     - [ ] auto_resign
-    - [ ] chat
+    - [ ] chat (This is for chat rooms, low priority)
     - [ ] chat/remove
     - [ ] clear_auto_resign
     - [x] clock
     - [ ] conditional_moves
-    - [ ] error
+    - [x] error
     - [x] gamedata
     - [x] latency
-    - [ ] phase
+    - [x] phase
     - [ ] removed_stones
     - [ ] removed_stones_accepted
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
@@ -162,10 +164,10 @@
     - [ ] removed_stones/set
     - [x] resign
     - [ ] resume
     - [ ] timed_out
     - [x] undo/accept
     - [ ] undo/cancel
     - [ ] undo/request
-- [ ] Implement proper challenge creation
-- [ ] Create open challenge
+- [x] Implement proper challenge creation
+- [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

### Comparing `ogsapi-0.4.1/pyproject.toml` & `ogsapi-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.4.1/src/ogsapi/api.py` & `ogsapi-0.5.0/src/ogsapi/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import urllib.parse
 import socketio
 from typing import Callable
 from time import sleep, time
 
 # TODO: This will eventually need to be moved to `termination-api` instead of `/api/v1/`
 # TODO: Should probably implement a user class that contains all user info and functions
+# TODO: Break REST API functions into their own class, leaving the OGSClient class to be the interface for the user client
 
 class OGSApiException(Exception):
     """Exception raised for errors in the OGS API."""
     pass
 
 class OGSClient:
     """Connect to and interact with the OGS REST API and SocketIO API.
@@ -335,65 +336,144 @@
         """
 
         encoded_name = urllib.parse.quote(player_username)
         endpoint = f'/players/'
         return self.get_rest_endpoint(endpoint=endpoint, params={'username' : encoded_name})['results'][0]
 
     # TODO: Need to make these customizable 
-    def challenge_player(self, player_username):
-        """Challenge a player to a game. WIP
-        
-        Args:
-            player_username (str): Username of the player to challenge.
-            
-        Returns:
-            dict: JSON response from the endpoint
-        """
-
-        game_settings = {
-            "initialized": False,
-            "min_ranking": -1000,
-            "max_ranking": 1000,
-            "challenger_color": "black",
-            "game": {
-                "name": "test",
-                "rules": "japanese",
-                "ranked":False,
-                "width":9,
-                "height":9,
-                "handicap": "0",
-                "komi_auto": "custom",
-                "komi":0,
-                "disable_analysis":False,
-                "initial_state": None,
-                "private": False,
-                "time_control": "byoyomi",
-                "time_control_parameters": {
-                    "system": "byoyomi",
-                    "speed": "60000",
-                    "total_time":60000,
-                    "initial_time":60000,
-                    "time_increment":60000,
-                    "max_time":60000,
-                    "main_time":660000,
-                    "period_time":60000,
-                    "periods":60000,
-                    "per_move":60000,
-                    "stones_per_period":10,
-                    "pause_on_weekends": False,
-                    "time_control": "byoyomi"
-                },
-                "pause_on_weekends": False
+    def create_challenge(self, player_username: str = None, **game_settings):
+        """Create either an open challenge or a challenge to a specific player.
+        The time control settings are built depending on which time control is used.
+        Make sure that you pass the correct time control settings for the time control you want to use.
+        The other time control settings will be ignored.
+        
+        Example:
+            >>> ogs.create_challenge(player_username='test', main_time=300, byoyomi_time=30, byoyomi_stones=5)
+            Challenging player: test - 1234567
+            (20328495, 53331333)
+
+        Args:
+            player_username (str): Username of the player to challenge. 
+                If used will issue the challenge to the player. Defaults to None.
+        
+        Keyword Args:
+            min_rank (int): Minimum rank of the player to challenge. Defaults to 7.
+            max_rank (int): Maximum rank of the player to challenge. Defaults to 18.
+            challenger_color (str): Color of the challenger. Defaults to 'white'.
+            aga_ranked (bool): Whether or not the game is AGA ranked. Defaults to False.
+            invite_only (bool): Whether or not the game is invite only. Defaults to False.  
+            game_name (str): Name of the game. Defaults to 'Friendly Game'.
+            game_rules (str): Rules of the game. Defaults to 'japanese'.
+            game_ranked (bool): Whether or not the game is ranked. Defaults to False.
+            game_width (int): Width of the board. Defaults to 19.
+            game_height (int): Height of the board. Defaults to 19.
+            game_handicap (int): Handicap of the game. Defaults to 0.
+            game_komi_auto (bool): Whether or not to use automatic komi. Defaults to True.
+            game_komi (float): Komi of the game. Defaults to 6.5.
+                Not needed if using auto komi.            
+            game_disable_analysis (bool): Whether or not to disable analysis. Defaults to False.
+            game_initial_state (str): Initial state of the game. Defaults to None.   
+            game_private (bool): Whether or not the game is private. Defaults to False.
+            game_time_control (str): Time control of the game. Defaults to 'byoyomi'.
+            byoyomi_main_time (int): Main time of the game in seconds. Defaults to 2400.
+                only used if byoyomi time control is used.
+            byoyomi_period_time (int): Period time of the game in seconds. Defaults to 30.
+                only used if byoyomi time control is used.
+            byoyomi_periods (int): Number of periods in the game. Defaults to 5.
+                only used if byoyomi time control is used.
+            byoyomi_periods_min (int): Minimum periods of the game. Defaults to 5.
+                only used if byoyomi time control is used.
+            byoyomi_periods_max (int): Maximum periods of the game. Defaults to 5.
+                only used if byoyomi time control is used.
+            fisher_time_initial_time (int): Initial time of the game in seconds. Defaults to 900.
+                only used if fisher time control is used.
+            fisher_time_increment (int): Increment of the game in seconds. Defaults to 0.
+                only used if fisher time control is used.
+            fisher_time_max_time (int): Maximum time of the game in seconds. Defaults to 1800.
+                only used if fisher time control is used.       
+            
+        Returns:
+            challenge_id (int): ID of the challenge created
+            game_id (int): ID of the game created
+        """
+        time_control = game_settings.get('time_control', 'byoyomi')
+        # Set common parameters
+        time_control_parameters = {}
+        time_control_parameters['speed'] = game_settings.get('speed', 'correspondence')
+        time_control_parameters['pause_on_weekends'] = game_settings.get('pause_on_weekends', False)
+        time_control_parameters['time_control'] = time_control
+
+        # Create time control paramters depending on time control used
+        match time_control:
+            case 'byoyomi':
+                time_control_parameters = {
+                    'system' : 'byoyomi',
+                    'main_time' : game_settings.get('byoyomi_main_time', 2400),
+                    'period_time' : game_settings.get('byoyomi_period_time', 30),
+                    'periods' : game_settings.get('byoyomi_periods', 5),
+                    'periods_min' : game_settings.get('byoyomi_periods_min', 1),
+                    'periods_max' : game_settings.get('byoyomi_periods_max', 300),
+
+                }
+            case 'fischer':
+                time_control_parameters = {
+                    'system' : 'fischer',
+                    'initial_time' : game_settings.get('fischer_initial_time', 2400),
+                    'time_increment' : game_settings.get('fischer_time_increment', 30),
+                    'max_time' : game_settings.get('fischer_max_time', 300),
+                }
+            case 'canadian':
+                # TODO: Implement
+                time_control_parameters = {}
+            case 'absolute':
+                # TODO: Implement
+                time_control_parameters = {}
+            case 'none':
+                time_control_parameters = {
+                    'system' : 'none',
+                    'speed' : 'correspondence',
+                    'time_control' : 'none',
+                    'pause_on_weekends' : False
+                }
+
+        # Create challenge from kwargs
+        challenge = {
+            'initialized' : False,
+            'min_ranking' : game_settings.get('min_ranking', 7),
+            'max_ranking' : game_settings.get('max_ranking', 18),
+            'challenger_color' : game_settings.get('challenger_color', 'white'),
+            'game' : {
+                'name' : game_settings.get('game_name', 'Friendly Game'),
+                'rules' : game_settings.get('game_rules', 'japanese'),
+                'ranked' : game_settings.get('game_ranked', False),
+                'width' : game_settings.get('game_width', 19),
+                'height' : game_settings.get('game_height', 19),
+                'handicap' : game_settings.get('game_handicap', '0'),
+                'komi_auto' : game_settings.get('game_komi_auto', True),
+                'komi' : game_settings.get('game_komi', '6.5'),
+                'disable_analysis' : game_settings.get('game_disable_analysis', False),
+                'initial_state' : game_settings.get('game_initial_state', None),
+                'private' : game_settings.get('game_private', False),
+                'time_control' : time_control,
+                'time_control_parameters' : time_control_parameters
             },
-            "aga_ranked": False
+            'aga_ranked' : game_settings.get('aga_ranked', False),
+            'invite_only' : game_settings.get('invite_only', False),
         }
-        player_id = self.get_player(player_username)['id']
-        print(f"Challenging player: {player_username} - {player_id}")
-        endpoint = f'/players/{player_id}/challenge/'
-        response = self.post_rest_endpoint(endpoint, game_settings)
+
+        if player_username is not None:
+            player_id = self.get_player(player_username)['id']
+            print(f"Challenging player: {player_username} - {player_id}")
+            endpoint = f'/players/{player_id}/challenge/'
+            response = self.post_rest_endpoint(endpoint, challenge)
+        else:
+            endpoint = '/challenges/'
+            print("Creating open challenge")
+            response = self.post_rest_endpoint(endpoint, challenge)
+
         challenge_id = response['challenge']
         game_id = response['game']
         return challenge_id, game_id
 
     # Challenges
 
     # TODO: Change these to use the 'challenger' parameter instead of looping through all challenges
@@ -548,33 +628,35 @@
         }
         self.start_time: int = None
         self.clock = {}
         self.latency = 100
         self.callback_func = {
             'on_move': None,
             'on_clock': None,
+            'on_phase_change': None,
             'on_undo_requested': None,
             'on_undo_accepted': None,
-            'on_undo_rejected': None,
+            'on_undo_canceled': None,
         }
 
     def __del__(self):
         self.disconnect()
 
     def register_callback(self, event: str, callback: Callable):
         """Register a callback function for receiving data from the API.
         
         Args:
             event (str): Event to register the callback function for.
                 Accepted events are:
                     - on_move
                     - on_clock
+                    - on_phase_change
                     - on_undo_requested
                     - on_undo_accepted
-                    - on_undo_rejected
+                    - on_undo_canceled
             callback (Callable): Callback function to register.   
         """
         self.callback_func[event] = callback
 
     # Low level socket functions
     def _game_call_backs(self):
 
@@ -666,14 +748,23 @@
             
             # Call the on_clock callback
             try:
                 self.callback_func['on_clock'](self.clock)
             except TypeError as e:
                 raise OGSApiException("Callback function 'on_clock' must be Type Callable") from e
 
+        @self.socket.on(f'game/{self.game_id}/phase')
+        def _on_game_phase(data):
+            print(f"Got Phase Change: {data}")
+            self.phase = data
+            try:
+                self.callback_func['on_phase_change'](self.phase)
+            except TypeError as e:
+                raise OGSApiException("Callback function 'on_phase_change' must be Type Callable") from e
+
         @self.socket.on(f'game/{self.game_id}/latency')
         def _on_game_latency(data):
             print(f'Got Latency: {data}')
             self.latency = data['latency']
 
         @self.socket.on(f'game/{self.game_id}/undo_requested')
         def _on_undo_requested(data):
@@ -689,21 +780,21 @@
             #TODO: Handle This
             print(f'Got Accepted Undo: {data}')
             try:
                 self.callback_func['on_undo_accepted'](data)
             except TypeError as e:
                 raise OGSApiException("Callback function 'on_undo_accepted' must be Type Callable") from e
         
-        @self.socket.on(f'game/{self.game_id}/undo_cancelled')
-        def _on_undo_cancelled(data):
-            print(f"Got Cancelled Undo: {data}")
+        @self.socket.on(f'game/{self.game_id}/undo_canceled')
+        def _on_undo_canceled(data):
+            print(f"Got Canceled Undo: {data}")
             try:
-                self.callback_func['on_undo_cancelled'](data)
+                self.callback_func['on_undo_canceled'](data)
             except TypeError as e:
-                raise OGSApiException("Callback function 'on_undo_cancelled' must be Type Callable") from e
+                raise OGSApiException("Callback function 'on_undo_canceled' must be Type Callable") from e
     
     # Send functions
     def connect(self):
         """Connect to the game"""
         print(f"Connecting to game {self.game_id}")
         self.socket.emit(event="game/connect", data={'game_id': self.game_id, 'player_id': self.user_data['id'], 'chat': False})
 
@@ -777,14 +868,15 @@
     Attributes:
         clock_drift (float): The clock drift of the socket
         clock_latency (float): The clock latency of the socket
         last_ping (int): The last ping time of the socket
         last_issued_ping (int): The last time a ping was issued
         games (dict): A dict of connected game objects
         bearer_token (str): The bearer token used for authentication
+        client_callbacks (dict): A dict of socket level callbacks
         auth_data (dict): The auth data returned from the OGS API
         user_data (dict): The user data returned from the OGS API
         socket (socketio.Client): The socketio client object
         
     """
 
     def __init__(self, bearer_token: str, debug: bool = False):
@@ -792,38 +884,55 @@
         self.clock_drift = 0.0
         self.clock_latency = 0.0
         self.last_ping = 0
         self.last_issued_ping = 0
         # Dict of connected game objects
         self.games = {}
         self.bearer_token = bearer_token
-        # TODO: Allow user to enable logger functions when creating the object
+        # Socket level callbacks
+        self.client_callbacks = {
+            'notification': None,
+            'error': None,
+        }
         self.socket = socketio.Client(logger=debug, engineio_logger=False)
         try:
             self.auth_data = requests.get('https://online-go.com/api/v1/ui/config', headers={'Authorization': f'Bearer {bearer_token}'}).json()
         except requests.exceptions.RequestException as e:
             raise OGSApiException("Failed to get auth_data") from e
         
         # Grab user data as its own variable for ease of use
         self.user_data = self.auth_data['user']
 
     def __del__(self):
         self.disconnect()
 
     def connect(self):
         """Connect to the socket"""
-        self.call_backs()
+        self.socket_callbacks()
         print("Connecting to Websocket")
         try:
             self.socket.connect('https://online-go.com/socket.io/?EIO=4', transports='websocket', headers={"Authorization" : f"Bearer {self.bearer_token}"})
         except:
             raise OGSApiException("Failed to connect to OGS Websocket")
 
+    def register_callback(self, event: str, callback: Callable):
+        """Register a callback function for receiving data from the API.
+        
+        Args:
+            event (str): Event to register the callback function for.
+                Accepted events are:
+                    - notification
+                    - chat
+                    - error
+            callback (Callable): Callback function to register.   
+        """
+        self.client_callbacks[event] = callback
+
     # Listens to events received from the socket via the decorators, and calls the appropriate function
-    def call_backs(self):
+    def socket_callbacks(self):
         """Set the callback functions for the socket"""
 
         @self.socket.on('connect')
         def authenticate():
             """Authenticate to the socket"""
             print("Connected to socket, authenticating")
             self.socket.emit(event="authenticate", data={"auth": self.auth_data['chat_auth'], "player_id": self.user_data['id'], "username": self.user_data['username'], "jwt": self.auth_data['user_jwt']})
@@ -846,24 +955,28 @@
             print(f"Got pong: {data}")
         
         @self.socket.on('active_game')
         def on_active_game(data):
             """Called when an active game is received on the socket"""
             print(f"Got active game: {data}")
 
-        @self.socket.on('game/*')
-        def on_game(data):
-            """Catch all for game events"""
-            print(f"Got game data: {data}")
-
         @self.socket.on('notification')
         def on_notification(data):
             """Called when a notification is received on the socket"""
             print(f"Got notification: {data}")
 
+        @self.socket.on('ERROR')
+        def on_error(data):
+            """Called when an error is received from the server"""
+            print(f"Got error: {data}")
+            try:
+                self.client_callbacks['error'](data)
+            except TypeError as e:
+                raise OGSApiException("Callback function 'error' must be Type Callable") from e
+
         @self.socket.on('*')
         def catch_all(event, data):
             """Catch all for events"""
             print(f"Got Event: {event} \n {data}")
 
     # Get info on connected server
     def host_info(self):
```

### Comparing `ogsapi-0.4.1/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.5.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.4.1
+Version: 0.5.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +17,16 @@
 
 ## Summary
 
 An API wrapper written in python for the Online-Go Server's (OGS) REST API and Realtime (SocketIO) API
 
 **THIS IS STILL HEAVILY IN DEVELOPMENT. VERY MUCH NOT READY FOR USE**
 
+Read the documentation here for more info: https://ogs-python.dakotamarshall.net/
+
 ## Install
 
 ### Pip Package
 
 ```bash
 python3 -m pip install ogsapi
 ```
@@ -135,23 +137,23 @@
     - [ ] GET - id/games
     - [ ] GET - id/groups
     - [ ] GET - id/ladders
     - [ ] GET - id/tournaments
 - [ ] Realtime API Game Events
   - [ ] Server to Client
     - [ ] auto_resign
-    - [ ] chat
+    - [ ] chat (This is for chat rooms, low priority)
     - [ ] chat/remove
     - [ ] clear_auto_resign
     - [x] clock
     - [ ] conditional_moves
-    - [ ] error
+    - [x] error
     - [x] gamedata
     - [x] latency
-    - [ ] phase
+    - [x] phase
     - [ ] removed_stones
     - [ ] removed_stones_accepted
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
@@ -174,10 +176,10 @@
     - [ ] removed_stones/set
     - [x] resign
     - [ ] resume
     - [ ] timed_out
     - [x] undo/accept
     - [ ] undo/cancel
     - [ ] undo/request
-- [ ] Implement proper challenge creation
-- [ ] Create open challenge
+- [x] Implement proper challenge creation
+- [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

