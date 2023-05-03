# Comparing `tmp/PlatitudeTerminal-1.0.2.tar.gz` & `tmp/PlatitudeTerminal-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlatitudeTerminal-1.0.2.tar", last modified: Wed May  3 04:06:02 2023, max compression
+gzip compressed data, was "PlatitudeTerminal-1.0.3.tar", last modified: Wed May  3 04:48:29 2023, max compression
```

## Comparing `PlatitudeTerminal-1.0.2.tar` & `PlatitudeTerminal-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.574087 PlatitudeTerminal-1.0.2/
--rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:06:02.574142 PlatitudeTerminal-1.0.2/PKG-INFO
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.572099 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      457 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       43 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/entry_points.txt
--rw-r--r--   0 louis      (501) staff       (20)      154 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.2/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.573873 PlatitudeTerminal-1.0.2/peregrine/
--rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.2/peregrine/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    29668 2023-05-03 04:00:43.000000 PlatitudeTerminal-1.0.2/peregrine/cli.py
--rw-r--r--   0 louis      (501) staff       (20)     3098 2023-04-23 07:52:41.000000 PlatitudeTerminal-1.0.2/peregrine/client.py
--rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.2/peregrine/colorutils.py
--rw-r--r--   0 louis      (501) staff       (20)      246 2023-04-22 22:46:59.000000 PlatitudeTerminal-1.0.2/peregrine/errors.py
--rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-03 03:58:08.000000 PlatitudeTerminal-1.0.2/peregrine/install.py
--rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.2/peregrine/main.py
--rw-r--r--   0 louis      (501) staff       (20)     2838 2023-05-02 19:16:55.000000 PlatitudeTerminal-1.0.2/peregrine/stateutils.py
--rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.2/pyproject.toml
--rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-03 04:06:02.574570 PlatitudeTerminal-1.0.2/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.2/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:48:29.073709 PlatitudeTerminal-1.0.3/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:48:29.073769 PlatitudeTerminal-1.0.3/PKG-INFO
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:48:29.071658 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      457 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       43 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/entry_points.txt
+-rw-r--r--   0 louis      (501) staff       (20)      154 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-03 04:48:29.000000 PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.3/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:48:29.073493 PlatitudeTerminal-1.0.3/peregrine/
+-rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.3/peregrine/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    29099 2023-05-03 04:47:52.000000 PlatitudeTerminal-1.0.3/peregrine/cli.py
+-rw-r--r--   0 louis      (501) staff       (20)     3098 2023-04-23 07:52:41.000000 PlatitudeTerminal-1.0.3/peregrine/client.py
+-rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.3/peregrine/colorutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      214 2023-05-03 04:10:35.000000 PlatitudeTerminal-1.0.3/peregrine/errors.py
+-rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-03 04:48:12.000000 PlatitudeTerminal-1.0.3/peregrine/install.py
+-rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.3/peregrine/main.py
+-rw-r--r--   0 louis      (501) staff       (20)     2971 2023-05-03 04:34:25.000000 PlatitudeTerminal-1.0.3/peregrine/stateutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.3/pyproject.toml
+-rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-03 04:48:29.073974 PlatitudeTerminal-1.0.3/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.3/setup.py
```

### Comparing `PlatitudeTerminal-1.0.2/PKG-INFO` & `PlatitudeTerminal-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlatitudeTerminal
-Version: 1.0.2
+Version: 1.0.3
 Summary: "Natural language command line queries."
 Author: Louis Smidt
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 
 # Platitude Terminal
 ## by Platitude.ai
```

### Comparing `PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/PKG-INFO` & `PlatitudeTerminal-1.0.3/PlatitudeTerminal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlatitudeTerminal
-Version: 1.0.2
+Version: 1.0.3
 Summary: "Natural language command line queries."
 Author: Louis Smidt
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 
 # Platitude Terminal
 ## by Platitude.ai
```

### Comparing `PlatitudeTerminal-1.0.2/README.md` & `PlatitudeTerminal-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.2/peregrine/cli.py` & `PlatitudeTerminal-1.0.3/peregrine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,44 +680,42 @@
             refreshed_user = auth.refresh(saved_refresh_token)
             if refreshed_user['idToken']:
                 email = stateutils.loadUserEmail()
                 stateutils.saveUserTokens(email=email, id_token=refreshed_user['idToken'], refresh_token=refreshed_user['refreshToken'])                
                 return True
             else:
                 # stored tokens are too old, re-auth!
-                raise stateutils.PeregrineExpiredLoginError()
+                raise errors.PeregrineExpiredLoginError()
             
-    except stateutils.PeregrineExpiredLoginError as e:
-        typer.echo(f"Oh no! Your login has expired. Please login again: {e}")
+    except errors.PeregrineExpiredLoginError as e:
+        typer.echo(f"Your login has expired. Please login again.")
+        login(ctx=AppState())
         return False
     except Exception as e:
         # user may have no stored tokens
         typer.echo(f"Encountered an error when attempting to login: {e}")
         return False
        
 
 @app.callback()
 def main(ctx: typer.Context):
 
-    # print(f"About to execute command: {ctx.invoked_subcommand}")
     try:
         version(verbose=False)
 
         # create / load env
         if not stateutils.envExists():
             stateutils.createNewEnv() 
         else:
             stateutils.loadFromEnv()
 
         # pass main flow for terminal commands
         if ctx.invoked_subcommand in ['logout']:
             return
 
-        # print(stateutils.getEnv())
-
         if stateutils.getTier() == stateutils.tier.NONE:
             # print sign up flow
 
             typer.echo(
                 '''
                 =======================================================================
                 |                                                                     |
@@ -731,30 +729,22 @@
 
             typer.echo("Welcome to Platitude Terminal, an AI assistant for the command line! Create an account or login to get started. \n")
             
             env = stateutils.writeDefaultEnv() #save blank env and copy into memory
             stateutils.clearUserTokens()
             ctx.obj = AppState(idToken = "", refreshToken = "", env = env)
 
-            create_or_login = typer.prompt("1 = Login to an existing account \n2 = Create a new account \n\nType choice and press Enter ", type=int)
+            create_or_login = typer.prompt("1 = Create new Platitude.ai account \n2 = Login with existing account \n\nType choice and press Enter ", type=int)
 
             if create_or_login == 1:
-                login(ctx)
-                raise typer.Exit()
-            elif create_or_login == 2:
                 signup(ctx)
                 raise typer.Exit()    
-            
-            # selection = typer.prompt("1 = Join our secure  $1/mo priority subscription with access to powerful new AI features as they're developed. \n2 = Enter an OpenAI API paid account key for basic usage. \n Type choice and press Enter ", type=int)
-            # if selection == 1:
-            #     typer.secho("Thanks for choosing our managed subscription. \n")
-            #     upgrade(ctx=signup_ctx)
-
-            # elif selection == 2:
-            #     key()
+            elif create_or_login == 2:
+                login(ctx)
+                raise typer.Exit()
 
         else:
         # user was once on a paid plan and tokens should exist
             try:
                 # first check if tokens exist and are valid / can be refreshed
                 existing_idT_is_valid = savedTokensAreValid()
```

### Comparing `PlatitudeTerminal-1.0.2/peregrine/client.py` & `PlatitudeTerminal-1.0.3/peregrine/client.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.2/peregrine/colorutils.py` & `PlatitudeTerminal-1.0.3/peregrine/colorutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.2/peregrine/stateutils.py` & `PlatitudeTerminal-1.0.3/peregrine/stateutils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dotenv
 import os
 from pathlib import Path
 import keyring
+from datetime import datetime
 
 class models:
     DEFAULT = "A"
     ADVANCED = "A"
     BASIC = "B"
 
 class tier:
@@ -16,15 +17,15 @@
 APP_DOMAIN = "https://platitude.ai/"
 API_DOMAIN = "https://us-central1-peregrine-ai.cloudfunctions.net/api"
 
 # for Development
 # APP_DOMAIN = "http://localhost:3000"
 # API_DOMAIN = "http://localhost:4244"
 
-env_path = Path.home().joinpath(".peregrine")
+env_path = Path.home().joinpath(".platitude-ai")
 env_file_path = env_path.joinpath(".env")
 
 def envExists():
     return env_file_path.exists()
 
 def createNewEnv():
     Path.mkdir(env_path, exist_ok=True)
@@ -34,14 +35,18 @@
     writeDefaultEnv()
 
 
 def writeDefaultEnv():
     setModel(models.DEFAULT)              # write the default model, tier
     setTier(tier.NONE)    
     setUid("")
+    
+    # now = datetime.now()
+    # _writeNow = now.strftime("%m/%d/%y_%H:%M:%S")
+    # setTime()
 
     return {"TIER": tier.NONE, "MODEL": models.DEFAULT, "UID": ""}
 
 def getEnv():
     model = getModel()
     tier = getTier()
     uid = getUid()
```

### Comparing `PlatitudeTerminal-1.0.2/pyproject.toml` & `PlatitudeTerminal-1.0.3/pyproject.toml`

 * *Files identical despite different names*

