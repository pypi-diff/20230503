# Comparing `tmp/trakt.py-4.4.0.tar.gz` & `tmp/trakt.py-5.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trakt.py-4.4.0.tar", last modified: Fri Mar 19 04:19:48 2021, max compression
+gzip compressed data, was "trakt.py-5.0.0.0rc1.tar", last modified: Wed May  3 14:47:47 2023, max compression
```

## Comparing `trakt.py-4.4.0.tar` & `trakt.py-5.0.0.0rc1.tar`

### file list

```diff
@@ -1,565 +1,570 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2021-03-19 04:18:39.000000 trakt.py-4.4.0/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      893 2021-03-19 04:18:39.000000 trakt.py-4.4.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2021-03-19 04:19:48.000000 trakt.py-4.4.0/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)    17327 2021-03-19 04:18:39.000000 trakt.py-4.4.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2021-03-19 04:18:39.000000 trakt.py-4.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1113 2021-03-19 04:18:39.000000 trakt.py-4.4.0/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2021-03-19 04:18:39.000000 trakt.py-4.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5110 2021-03-19 04:19:48.000000 trakt.py-4.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2021-03-19 04:18:39.000000 trakt.py-4.4.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      204 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/_templates/sidebar_header.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/_templates/sidebar_index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/changes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    15618 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/license.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/docs/sourcecode/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1014 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/interfaces.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/objects.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/docs/sourcecode/trakt/
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.client.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.configuration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.context_collection.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.context_stack.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.emitter.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.errors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.exceptions.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.helpers.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.http.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.pagination.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.request.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.core.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.helpers.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      185 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.auth.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.base.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.calendars.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.movies.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.oauth.device.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.oauth.pin.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.oauth.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.scrobble.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.search.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.shows.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      264 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.collection.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.core.mixins.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.core.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.playback.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.ratings.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      197 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.watched.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      278 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.sync.watchlist.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.following.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.friends.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.lists.list_.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.lists.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.ratings.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.settings.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.interfaces.users.watchlist.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.comment.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.core.base.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.core.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.list.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.list_item.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.progress.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.search.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.summary.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.sync.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.mapper.user.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.comment.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.core.helpers.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.core.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.episode.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.list.base.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.list.custom.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.media.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.movie.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.person.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.progress.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.rating.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.season.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.show.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.user.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.objects.video.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2021-03-19 04:18:39.000000 trakt.py-4.4.0/docs/sourcecode/trakt/trakt.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/examples/authentication/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4156 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/authentication/device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2249 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/authentication/pin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2527 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1259 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/lists.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1103 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/media_center.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1585 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/scrobbler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1610 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2021-03-19 04:18:39.000000 trakt.py-4.4.0/examples/trending.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-03-19 04:18:39.000000 trakt.py-4.4.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1105 2021-03-19 04:19:48.000000 trakt.py-4.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      435 2021-03-19 04:18:39.000000 trakt.py-4.4.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-03-19 04:18:39.000000 trakt.py-4.4.0/test-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3034 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/core/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11876 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/core/mock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      994 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/core/semaphore.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/dvd.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/movies.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows/
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows/new.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows/premieres.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2185 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/dvd.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/movies.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows/
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows/new.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1061 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows/premieres.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2185 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/genres/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/genres/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2562 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/genres/shows.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/lists/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/lists/popular.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1523 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/lists/trending.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9179 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    44491 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/people.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16759 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/related.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/releases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    38459 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    14560 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/anticipated.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16760 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/boxoffice.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18407 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/collected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19152 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/played.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16943 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/popular.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/recommended/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18436 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/recommended/monthly.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18426 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/recommended.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18405 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/trending.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9179 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    44491 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/people.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16759 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/related.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/releases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    38459 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9179 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    44491 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/people.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16759 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/related.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/releases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    38459 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1710 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1089 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/updates.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19152 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/watched.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737/
--rw-rw-r--   0 travis    (2000) travis    (2000)    90101 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18566 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston/
--rw-rw-r--   0 travis    (2000) travis    (2000)    90101 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18566 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505/
--rw-rw-r--   0 travis    (2000) travis    (2000)    90101 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18566 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1053 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/episode/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/episode/#query/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7171 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/episode/#query/Breaking Bad.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1968 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/full.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2271 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/full.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3834 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/full.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/movie/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/movie/#query/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3542 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/movie/#query/The Avengers.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/show/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/show/#query/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4000 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/show/#query/Breaking Bad.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9117 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/last_episode.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7860 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    13411 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/people.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/progress/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/progress/collection.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1943 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/progress/watched.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19020 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/related.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5799 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/comments.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6563 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8574 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      130 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    22537 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1213 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7465 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7867 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16442 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    31704 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41662 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41168 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1765 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15287 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/anticipated.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    25282 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/collected.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9117 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/last_episode.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7860 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    13411 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/people.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/collection.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1813 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/watched.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19020 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/related.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5799 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/comments.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6563 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8574 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      130 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    22537 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      602 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7465 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7867 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16442 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    31704 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41626 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    40555 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1765 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    24000 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/played.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    20312 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/popular.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/recommended/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23515 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/recommended/monthly.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    23508 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/recommended.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    23487 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/trending.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/aliases.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9117 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/last_episode.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7860 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    13411 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/people.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1638 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/collection.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19020 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/related.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5799 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/comments.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6563 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/comments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8574 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      130 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    22537 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      602 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1292 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7465 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/ratings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7247 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16442 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    31704 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/stats.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41626 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/translations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41978 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/watching.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1765 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6323 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/updates.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    24081 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/watched.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/collection/
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/collection/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2865 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/collection/shows.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8084 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15202 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5213 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback/episodes.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      617 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3283 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/episodes.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/movies/
--rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/movies/8.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      611 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      930 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/seasons.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1674 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watched/
--rw-rw-r--   0 travis    (2000) travis    (2000)      904 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watched/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9497 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watched/shows.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watchlist/
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watchlist/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1607 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watchlist.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/likes.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/following.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      493 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/friends.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/history.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/movies/
--rw-rw-r--   0 travis    (2000) travis    (2000)      547 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/movies/items.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/movies.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/people/
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/people/items.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/people.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/shows/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/shows/items.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    10877 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/ratings.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watched/
--rw-rw-r--   0 travis    (2000) travis    (2000)      666 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watched/movies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2112 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watched/shows.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watchlist.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/55/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2015 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/55/items.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      774 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/55.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2015 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/items.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      774 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3739 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/fixtures/download.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/oauth/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/oauth/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1316 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/oauth/test_device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/oauth/test_device_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5552 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/oauth/test_oauth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/oauth/test_pin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/objects/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/objects/test_list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/collection/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/collection/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/collection/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2424 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/collection/test_shows.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/history/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/history/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      370 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/history/test_invalid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/history/test_mixed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      732 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/history/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      731 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/history/test_shows.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/playback/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/playback/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/playback/test_delete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1455 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/playback/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/playback/test_shows.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/ratings/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/ratings/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1291 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/ratings/test_mixed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2506 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/ratings/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2671 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/ratings/test_shows.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/watched/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watched/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      352 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watched/test_invalid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2030 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watched/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1509 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watched/test_shows.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/sync/watchlist/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watchlist/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5667 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watchlist/test_mixed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1263 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/sync/watchlist/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11176 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_calendars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1395 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_context_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      519 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1112 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6069 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_lists.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1464 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_pagination.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_popular.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6427 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_progress.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_recommended.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_scrobble.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5270 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4758 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_summary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1257 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_trending.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1086 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/test_user.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/users/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/users/lists/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/tests/users/lists/items/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/items/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1726 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/items/test_movies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/items/test_people.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1921 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/items/test_shows.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/test_actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      837 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/test_create.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/test_get.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      965 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/lists/test_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_following.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      772 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_friends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_ratings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10281 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_watched.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      611 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tests/users/test_watchlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2021-03-19 04:18:39.000000 trakt.py-4.4.0/tox.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1523 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5013 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/context_collection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      634 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/context_stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6297 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/emitter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3281 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10816 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      588 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/keylock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4190 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/pagination.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4288 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/core/request.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      713 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/hooks.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2427 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/auth.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3543 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5257 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/calendars.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/lists/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/lists/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/movies/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3015 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/movies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/oauth/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3390 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/oauth/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5234 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/oauth/device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/oauth/pin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11832 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/scrobble.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/search.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/shows/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5998 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/shows/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/sync/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      734 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/collection.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/sync/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/core/mixins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2373 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      549 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/playback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/ratings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      673 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/watched.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1880 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/sync/watchlist.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/users/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2902 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      966 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/following.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      960 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/friends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3409 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/history.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/interfaces/users/lists/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3559 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/lists/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5294 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/lists/list_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/profile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2947 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/ratings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2286 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/watched.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2781 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/interfaces/users/watchlist.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/mapper/
--rw-rw-r--   0 travis    (2000) travis    (2000)      602 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/comment.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/mapper/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/core/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2142 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4027 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/list_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      625 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/progress.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3893 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3894 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/summary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7788 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      804 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/mapper/user.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3241 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/comment.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/objects/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/core/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4887 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/episode.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/objects/list/
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/list/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5889 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/list/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2156 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/list/custom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      973 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/list/public.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6300 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/media.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6122 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/movie.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/person.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8497 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/progress.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/rating.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/season.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7238 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/show.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/user.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2549 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/objects/video.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2777 2021-03-19 04:18:39.000000 trakt.py-4.4.0/trakt/sphinxext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5110 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    20176 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-19 04:19:25.000000 trakt.py-4.4.0/trakt.py.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/pbr.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-03-19 04:19:48.000000 trakt.py-4.4.0/trakt.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.093031 trakt.py-5.0.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-03 14:47:47.157032 trakt.py-5.0.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/build-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.093031 trakt.py-5.0.0.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.093031 trakt.py-5.0.0.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/_templates/sidebar_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/_templates/sidebar_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.093031 trakt.py-5.0.0.0rc1/docs/sourcecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/objects.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.105031 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.context_collection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.context_stack.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.emitter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.pagination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.request.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.calendars.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.movies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.oauth.device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.oauth.pin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.scrobble.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.search.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.shows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.collection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.core.mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.playback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.ratings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.watched.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.sync.watchlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.following.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.friends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.lists.list_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.ratings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.interfaces.users.watchlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.comment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.core.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.list_item.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.progress.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.search.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.mapper.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.comment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.core.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.episode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.list.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.list.custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.media.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.movie.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.person.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.progress.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.rating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.season.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.show.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.objects.video.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/docs/sourcecode/trakt/trakt.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.105031 trakt.py-5.0.0.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.105031 trakt.py-5.0.0.0rc1/examples/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/authentication/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/authentication/pin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/media_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/scrobbler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/examples/trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 14:47:47.157032 trakt.py-5.0.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/core/semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.085031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/dvd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/movies.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows/new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows/premieres.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/dvd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/movies.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows/new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows/premieres.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/genres/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/genres/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/genres/shows.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.109031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/lists/popular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/lists/trending.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.113031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.113031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/people.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/related.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/releases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/anticipated.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/boxoffice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/collected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19152 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/played.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/popular.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.113031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/recommended/
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/recommended/monthly.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/recommended.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18405 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/trending.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.117031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/people.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/related.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/releases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.117031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44491 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/people.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/related.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/releases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38459 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19152 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/watched.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.117031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.117031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737/
+-rw-r--r--   0 runner    (1001) docker     (123)    90101 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.117031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston/
+-rw-r--r--   0 runner    (1001) docker     (123)    90101 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505/
+-rw-r--r--   0 runner    (1001) docker     (123)    90101 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.085031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/episode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/episode/#query/
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/episode/#query/Breaking Bad.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.081031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/movie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/movie/#query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/movie/#query/The Avengers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.085031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/show/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/show/#query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/show/#query/Breaking Bad.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.121031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/last_episode.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/people.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/progress/collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/progress/watched.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/related.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/comments.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.125032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31704 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons.json
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41662 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41168 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/anticipated.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/collected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/last_episode.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/people.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/watched.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/related.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/comments.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31704 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons.json
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40555 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/played.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/popular.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.129032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/recommended/
+-rw-r--r--   0 runner    (1001) docker     (123)    23515 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/recommended/monthly.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/recommended.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/trending.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/last_episode.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/people.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/related.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/comments.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/ratings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31704 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons.json
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41978 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/watching.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24081 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/watched.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.133032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/collection/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/collection/shows.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback/episodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/episodes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/movies/8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/seasons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watched/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watched/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watched/shows.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watchlist/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watchlist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/likes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/following.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/friends.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/history.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/movies/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/movies.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.137032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/people/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/people/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/people.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/shows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/shows/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists.json
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/ratings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watched/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watched/movies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watched/shows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watchlist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.085031 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/55/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/55/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/55.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/fixtures/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/oauth/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/oauth/test_device_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/oauth/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/oauth/test_pin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/objects/test_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/sync/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/collection/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/collection/test_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/sync/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/history/test_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/history/test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/history/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/history/test_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/sync/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/playback/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/playback/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/playback/test_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.141032 trakt.py-5.0.0.0rc1/tests/sync/ratings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/ratings/test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/ratings/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/ratings/test_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/tests/sync/watched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watched/test_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watched/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watched/test_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/tests/sync/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watchlist/test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/sync/watchlist/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_context_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_popular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_recommended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_scrobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/tests/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/tests/users/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/tests/users/lists/items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/items/test_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/items/test_people.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/items/test_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/lists/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_friends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_watched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tests/users/test_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/context_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/context_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/keylock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/calendars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/lists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/movies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/pin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/scrobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/shows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/shows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.149032 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/playback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/watched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/sync/watchlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/interfaces/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/following.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/friends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/interfaces/users/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/lists/list_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/watched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/interfaces/users/watchlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/mapper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/mapper/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/objects/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/episode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.153032 trakt.py-5.0.0.0rc1/trakt/objects/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/list/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/list/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/season.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/objects/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 14:47:29.000000 trakt.py-5.0.0.0rc1/trakt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:47:47.145032 trakt.py-5.0.0.0rc1/trakt.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:47:46.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 14:47:47.000000 trakt.py-5.0.0.0rc1/trakt.py.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trakt.py-4.4.0/.gitignore` & `trakt.py-5.0.0.0rc1/.gitignore`

 * *Files 23% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 .tox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 cover/
+*.lcov
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
@@ -65,10 +66,11 @@
 [Ll]ib
 [Ll]ocal
 [Ss]cripts
 pyvenv.cfg
 pip-selfcheck.json
 .venv*/
 
+
 /_html
 /.idea
 *.iml
```

### Comparing `trakt.py-4.4.0/CHANGES.rst` & `trakt.py-5.0.0.0rc1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/CONTRIBUTING.rst` & `trakt.py-5.0.0.0rc1/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,52 +37,76 @@
 
 Please detail your suggested enhancement and include any relevant information, for example:
 
 - Link to the relevant method in the `Trakt.tv API Specification`_
 - Current library functionality (on the latest official release)
 - Would this enhancement break compatibility? could this be resolved in any way (e.g. method proxies)?
 
-Pull Requests
--------------
+Development
+-----------
 
 **Please ensure:**
 
-- Your changes are based on the *develop* branch, before starting development checkout the correct branch:
+- Your changes should be based on the *develop* branch, before starting development checkout the correct branch:
 
   .. code-block:: shell
 
     git checkout develop
 
+- You have installed the development dependencies if you plan to work on the build system or run tests without using tox
+
+  - If you are using `pipenv`_
+
+    .. code-block:: shell
+
+      pipenv install
+
+  - Otherwise, you can install the 'test_requirements.txt' for running tests and 'build_requirements.txt' for building
+
+Building
+--------
+
+- To build a distribution, after you have installed the build requirements:
+
+  .. code-block:: shell
+
+    python -m build
+
+Pull Requests
+-------------
+
+**Please ensure:**
+
 - Tests pass, either:
 
   - Use `tox`_ to run tests against each version of Python and PyPy:
 
     .. code-block:: shell
 
       tox
 
   - Test against your current version of Python:
 
     .. code-block:: shell
 
-      python setup.py test
+      pytest
 
   - Create your pull request, and wait for the test results to be posted by Travis CI. *(this may take a few minutes)*
 
 - No issues are reported by `flake8`_, either:
 
   - Use `tox`_ to run `flake8`_:
 
     .. code-block:: shell
 
       tox flake8
 
   - Create your pull request, and wait for the test results to be posted by Travis CI. *(this may take a few minutes)*
 
-    **Note:** `flake8`_ results will be displayed under the "Python 3.6" job.
+    **Note:** `flake8`_ results will be displayed under the "Python 3.10" job.
 
 - Test coverage hasn't fallen *(lines added without tests)*
 
   - Use `tox`_ to run tests against each version of Python and PyPy:
 
     .. code-block:: shell
 
@@ -92,9 +116,10 @@
 
   - Create your pull request, and wait for the coverage details to be posted by Coveralls. *(this may take a few minutes)*
 
 If you aren't sure how to write tests or are confused about any of the above steps, just post the pull request anyway. I'll either let you
 know what needs to be changed, or can just cleanup your code and write the required tests (if requested).
 
 .. _flake8: http://flake8.pycqa.org
-.. _Trakt.tv API Specification: http://docs.trakt.apiary.io
+.. _Trakt.tv API Specification: http://trakt.docs.apiary.io
 .. _tox: https://tox.readthedocs.io
+.. _pipenv: https://pipenv.pypa.io/en/latest/index.html
```

### Comparing `trakt.py-4.4.0/LICENSE.rst` & `trakt.py-5.0.0.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/README.rst` & `trakt.py-5.0.0.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 trakt.py
 ========
 
 .. image:: https://img.shields.io/pypi/v/trakt.py.svg?style=flat-square
    :target: https://pypi.python.org/pypi/trakt.py
 
-.. image:: https://img.shields.io/travis/fuzeman/trakt.py.svg?style=flat-square
-   :target: https://travis-ci.org/fuzeman/trakt.py
+.. image:: https://github.com/fuzeman/trakt.py/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/fuzeman/trakt.py/actions/workflows/test.yml
 
 .. image:: https://img.shields.io/codeclimate/github/fuzeman/trakt.py.svg?style=flat-square
    :target: https://codeclimate.com/github/fuzeman/trakt.py
 
 .. image:: https://img.shields.io/coveralls/fuzeman/trakt.py.svg?style=flat-square
    :target: https://coveralls.io/r/fuzeman/trakt.py?branch=master
```

### Comparing `trakt.py-4.4.0/docs/conf.py` & `trakt.py-5.0.0.0rc1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
-from __future__ import print_function
 
 import inspect
 import os
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
```

### Comparing `trakt.py-4.4.0/docs/sourcecode/interfaces.rst` & `trakt.py-5.0.0.0rc1/docs/sourcecode/interfaces.rst`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/docs/sourcecode/modules.rst` & `trakt.py-5.0.0.0rc1/docs/sourcecode/modules.rst`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/examples/authentication/device.py` & `trakt.py-5.0.0.0rc1/examples/authentication/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt import Trakt
 
 from threading import Condition
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/authentication/pin.py` & `trakt.py-5.0.0.0rc1/examples/authentication/pin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt import Trakt
 
-from six.moves import input
 import logging
 import os
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Application(object):
```

### Comparing `trakt.py-4.4.0/examples/collection.py` & `trakt.py-5.0.0.0rc1/examples/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from examples.helpers import authenticate
 from trakt import Trakt
 from trakt.objects import Movie, Show
 
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/history.py` & `trakt.py-5.0.0.0rc1/examples/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from examples.helpers import authenticate
 from trakt import Trakt
 
 from datetime import datetime
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/lists.py` & `trakt.py-5.0.0.0rc1/examples/lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from examples.helpers import authenticate
 
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/media_center.py` & `trakt.py-5.0.0.0rc1/examples/media_center.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt import Trakt
 
 import logging
 import os
 
 logging.basicConfig(level=logging.DEBUG)
```

### Comparing `trakt.py-4.4.0/examples/scrobbler.py` & `trakt.py-5.0.0.0rc1/examples/scrobbler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from examples.helpers import authenticate
 from trakt import Trakt
 
 from pprint import pprint
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/search.py` & `trakt.py-5.0.0.0rc1/examples/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt import Trakt
 from trakt.objects import Episode
 
 import logging
 import os
```

### Comparing `trakt.py-4.4.0/examples/trending.py` & `trakt.py-5.0.0.0rc1/examples/trending.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt import Trakt
 
 import logging
 import os
 
 logging.basicConfig(level=logging.DEBUG)
```

### Comparing `trakt.py-4.4.0/setup.cfg` & `trakt.py-5.0.0.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [metadata]
 name = trakt.py
 author = Dean Gardiner
-author-email = me@dgardiner.net
+author_email = me@dgardiner.net
 summary = Python interface for the Trakt.tv API
-description-file = README.rst
+description_file = README.rst
 keywords = trakt.tv, api, client
 platforms = any
-home-page = https://github.com/fuzeman/trakt.py
+home_page = https://github.com/fuzeman/trakt.py
 license = MIT
-classifier = 
+classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries
 
 [pbr]
 skip_changelog = true
 
@@ -35,11 +34,10 @@
 [aliases]
 test = pytest
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
-post-hook.write_version = trakt.hooks.write_version
 tag_build = 
 tag_date = 0
```

### Comparing `trakt.py-4.4.0/tests/core/helpers.py` & `trakt.py-5.0.0.0rc1/tests/core/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 # flake8: noqa: E241
 
-from six.moves.urllib_parse import urlparse, parse_qsl
+from urllib.parse import urlparse, parse_qsl
 import json
 import math
 import os
 import pytest
-import six
 
-if six.PY2:
-    try:
-        from six import cStringIO as BufferIO
-    except ImportError:
-        from six import StringIO as BufferIO
-else:
-    from io import BytesIO as BufferIO
+from io import BytesIO as BufferIO
 
 TESTS_PATH = os.path.abspath(os.path.dirname(__file__) + os.path.sep + '..')
 
 
 def read(path, mode='rb'):
     if not os.path.isabs(path):
         path = os.path.join(TESTS_PATH, path)
```

### Comparing `trakt.py-4.4.0/tests/core/mock.py` & `trakt.py-5.0.0.0rc1/tests/core/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import try_convert
 
-from six.moves.urllib_parse import parse_qsl
 import functools
 import httmock
 import itertools
 import json
 import math
 import os
+import urllib.parse as parse
+
 
 CURRENT_DIR = os.path.abspath(os.path.dirname(__file__))
 FIXTURES_DIR = os.path.abspath(os.path.join(CURRENT_DIR, '..', 'fixtures'))
 
 
 def authenticated(func):
     @functools.wraps(func)
@@ -38,15 +39,15 @@
     return (
         request.headers.get('trakt-user-login') == 'mock' and request.headers.get('trakt-user-token') == 'mock'
     )
 
 
 def get_content(netloc, path, query=None):
     components = path.strip('/').split('/') + list(itertools.chain.from_iterable([
-        ('#' + key, value) for key, value in sorted(parse_qsl(query or ''))
+        ('#' + key, value) for key, value in sorted(parse.parse_qsl(query or ''))
     ]))
     path = None
 
     # Search for matching fixture
     current = os.path.join(FIXTURES_DIR, netloc)
 
     for component in components:
@@ -86,15 +87,15 @@
             'Content-Type': 'application/json'
         },
         request=request
     )
 
 
 def paginate(url, request, content_type='application/json'):
-    parameters = dict(parse_qsl(url.query))
+    parameters = dict(parse.parse_qsl(url.query))
 
     page = try_convert(parameters.get('page'), int) or 1
     limit = try_convert(parameters.get('limit'), int) or 10
 
     # Retrieve items from fixture
     items = get_json(url.netloc, url.path, url.query)
 
@@ -243,15 +244,15 @@
 def likes_invalid_content_type(url, request):
     return likes(url, request, content_type='text/plain')
 
 
 @httmock.urlmatch(netloc='api.trakt.tv', path=r'/users/likes')
 @authenticated
 def likes_invalid_json(url, request):
-    parameters = dict(parse_qsl(url.query))
+    parameters = dict(parse.parse_qsl(url.query))
 
     page = try_convert(parameters.get('page'), int) or 1
 
     # Return invalid response for page #2
     if request.method == 'GET' and page == 2:
         return httmock.response(
             200, '<invalid-json-response>', {
@@ -263,15 +264,15 @@
     # Return page
     return likes(url, request)
 
 
 @httmock.urlmatch(netloc='api.trakt.tv', path=r'/users/likes')
 @authenticated
 def likes_request_failure(url, request):
-    parameters = dict(parse_qsl(url.query))
+    parameters = dict(parse.parse_qsl(url.query))
 
     page = try_convert(parameters.get('page'), int) or 1
 
     # Return invalid response for page #2
     if request.method == 'GET' and page == 2:
         return httmock.response(400, request=request)
```

### Comparing `trakt.py-4.4.0/tests/core/semaphore.py` & `trakt.py-5.0.0.0rc1/tests/core/semaphore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from threading import Condition, Lock
 
 
 class Semaphore(object):
     def __init__(self, value=1):
         if value < 0:
```

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/dvd.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/dvd.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows/new.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows/new.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows/premieres.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows/premieres.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/all/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/all/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/dvd.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/dvd.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows/new.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows/new.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows/premieres.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows/premieres.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/calendars/my/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/calendars/my/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/genres/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/genres/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/genres/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/genres/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/lists/popular.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/lists/popular.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/lists/trending.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/lists/trending.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/releases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/releases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/12601.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/12601.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/anticipated.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/anticipated.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/boxoffice.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/boxoffice.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/collected.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/collected.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/played.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/played.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/popular.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/popular.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/recommended/monthly.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/recommended/monthly.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/recommended.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/recommended.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/trending.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/trending.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/releases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/releases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tron-legacy-2010.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/releases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/releases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/tt1104001.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/tt1104001.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/updates.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/updates.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/movies/watched.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/movies/watched.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/297737.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/297737.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/bryan-cranston.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/bryan-cranston.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/people/nm0186505.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/people/nm0186505.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/episode/#query/Breaking Bad.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/episode/#query/Breaking Bad.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/full.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0848228/#extended/full.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/full.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0903747/#extended/full.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/full.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/imdb/tt0959621/#extended/full.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/movie/#query/The Avengers.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/movie/#query/The Avengers.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/search/show/#query/Breaking Bad.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/search/show/#query/Breaking Bad.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/last_episode.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/last_episode.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/progress/collection.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/progress/collection.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/progress/watched.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/progress/watched.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/episodes/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/seasons.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/seasons.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/1390.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/1390.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/anticipated.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/anticipated.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/collected.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/collected.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/last_episode.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/last_episode.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/collection.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/collection.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/watched.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/progress/watched.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/episodes/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/seasons.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/game-of-thrones.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/game-of-thrones.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/played.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/played.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/popular.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/popular.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/recommended/monthly.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/recommended/monthly.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/recommended.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/recommended.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/trending.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/trending.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/aliases.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/aliases.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/last_episode.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/last_episode.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/people.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/people.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/collection.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/progress/collection.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/related.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/related.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/comments.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/comments.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/episodes/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons/1.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/seasons.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/translations.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/translations.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947/watching.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947/watching.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/tt0944947.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/tt0944947.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/updates.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/updates.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/shows/watched.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/shows/watched.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/collection/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/collection/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/collection/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/collection/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/history.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/history.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback/episodes.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback/episodes.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/playback.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/playback.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/episodes.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/episodes.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/seasons.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/seasons.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/ratings.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/ratings.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watched/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watched/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watched/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watched/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/sync/watchlist.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/sync/watchlist.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/likes.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/likes.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/history.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/history.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/movies/items.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/movies/items.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/people/items.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/people/items.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists/shows/items.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists/shows/items.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/lists.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/lists.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/ratings.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/ratings.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watched/movies.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watched/movies.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watched/shows.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watched/shows.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/me/watchlist.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/me/watchlist.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/55/items.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/55/items.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/55.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/55.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/items.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order/items.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order.json` & `trakt.py-5.0.0.0rc1/tests/fixtures/api.trakt.tv/users/sean/lists/star-wars-in-machete-order.json`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/fixtures/download.py` & `trakt.py-5.0.0.0rc1/tests/fixtures/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # flake8: noqa: E241
 
 from datetime import datetime
-from six import string_types
-from six.moves.urllib_parse import ParseResult, parse_qsl, urlparse
+from urllib.parse import ParseResult, parse_qsl, urlparse
 import itertools
 import json
 import os
 import requests
 import sys
 import time
 
@@ -73,15 +72,15 @@
         )
 
     print('[%s] Done' % (url,))
     return True
 
 
 def build_destination_path(url):
-    if isinstance(url, string_types):
+    if isinstance(url, str):
         url = urlparse(url)
     elif not isinstance(url, ParseResult):
         raise ValueError('Invalid value provided for "url" parameter (expected string or urlparse result)')
 
     if not url.netloc or not url.path:
         print('[%s] Missing netloc or path' % (url,))
         return False
```

### Comparing `trakt.py-4.4.0/tests/oauth/test_device.py` & `trakt.py-5.0.0.0rc1/tests/oauth/test_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt, TraktClient
 
 from httmock import HTTMock
 import pytest
```

### Comparing `trakt.py-4.4.0/tests/oauth/test_device_poller.py` & `trakt.py-5.0.0.0rc1/tests/oauth/test_device_poller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 from threading import Event
 import httmock
@@ -140,12 +140,12 @@
         poller = Trakt['oauth/device'].poll('mock-device_code', 600, 5)
 
         # Start poller
         poller.start()
 
         try:
             # Ensure an exception is raised when attempting to start the poller again
-            with pytest.raises(Exception):
+            with pytest.raises(Exception, match='Poller already started'):
                 poller.start()
         finally:
             # Stop polling
             poller.stop()
```

### Comparing `trakt.py-4.4.0/tests/oauth/test_oauth.py` & `trakt.py-5.0.0.0rc1/tests/oauth/test_oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from tests.core.helpers import assert_url
 from trakt import Trakt, TraktClient
 
 from httmock import HTTMock
 from threading import Event
```

### Comparing `trakt.py-4.4.0/tests/objects/test_list.py` & `trakt.py-5.0.0.0rc1/tests/objects/test_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/sync/collection/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/collection/test_movies.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/collection/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/sync/collection/test_shows.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/history/test_mixed.py` & `trakt.py-5.0.0.0rc1/tests/sync/history/test_mixed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # flake8: noqa: F403, F405
 
 from tests.core import mock
 from trakt import Trakt
 
 from hamcrest import *
 from httmock import HTTMock
-from six.moves import xrange
 
 
 def test_basic():
     with HTTMock(mock.sync_history, mock.unknown):
         with Trakt.configuration.auth('mock', 'mock'):
             history = Trakt['sync/history'].get(pagination=True, per_page=5)
 
@@ -21,9 +20,9 @@
 
     # Ensure all items have been returned
     assert_that(items, has_length(3))
 
     # Verify item identifiers
     assert_that(
         [item.id for item in items],
-        equal_to(list(xrange(1, 4)))
+        equal_to(list(range(1, 4)))
     )
```

### Comparing `trakt.py-4.4.0/tests/sync/history/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/history/test_movies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # flake8: noqa: F403, F405
 
 from tests.core import mock
 from trakt import Trakt
 
 from hamcrest import *
 from httmock import HTTMock
-from six.moves import xrange
 
 
 def test_basic():
     with HTTMock(mock.sync_history, mock.unknown):
         with Trakt.configuration.auth('mock', 'mock'):
             history = Trakt['sync/history'].movies(pagination=True, per_page=5)
 
@@ -21,9 +20,9 @@
 
     # Ensure all items have been returned
     assert_that(items, has_length(25))
 
     # Verify item identifiers
     assert_that(
         [item.id for item in items],
-        equal_to(list(xrange(1, 26)))
+        equal_to(list(range(1, 26)))
     )
```

### Comparing `trakt.py-4.4.0/tests/sync/history/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/sync/history/test_shows.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # flake8: noqa: F403, F405
 
 from tests.core import mock
 from trakt import Trakt
 
 from hamcrest import *
 from httmock import HTTMock
-from six.moves import xrange
 
 
 def test_basic():
     with HTTMock(mock.sync_history, mock.unknown):
         with Trakt.configuration.auth('mock', 'mock'):
             history = Trakt['sync/history'].shows(pagination=True, per_page=5)
 
@@ -21,9 +20,9 @@
 
     # Ensure all items have been returned
     assert_that(items, has_length(25))
 
     # Verify item identifiers
     assert_that(
         [item.id for item in items],
-        equal_to(list(xrange(1, 26)))
+        equal_to(list(range(1, 26)))
     )
```

### Comparing `trakt.py-4.4.0/tests/sync/playback/test_delete.py` & `trakt.py-5.0.0.0rc1/tests/sync/playback/test_delete.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/playback/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/playback/test_movies.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/playback/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/sync/playback/test_shows.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/ratings/test_mixed.py` & `trakt.py-5.0.0.0rc1/tests/sync/ratings/test_mixed.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/ratings/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/ratings/test_movies.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/ratings/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/sync/ratings/test_shows.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/watched/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/watched/test_movies.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/watched/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/sync/watched/test_shows.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/sync/watchlist/test_mixed.py` & `trakt.py-5.0.0.0rc1/tests/sync/watchlist/test_mixed.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             # Ensure collection is valid
             assert_that(watchlist, not_none())
 
             # Resolve all pages
             items = list(watchlist)
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # TRON: Legacy (2010)
         all_of(
             instance_of(Movie),
             has_properties({
                 'pk': ('imdb', 'tt1104001'),
                 'title': 'TRON: Legacy',
                 'year': 2010,
@@ -116,15 +116,15 @@
             # Ensure collection is valid
             assert_that(watchlist, not_none())
 
             # Resolve iterator
             items = list(watchlist)
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # TRON: Legacy (2010)
         all_of(
             instance_of(Movie),
             has_properties({
                 'pk': ('imdb', 'tt1104001'),
                 'title': 'TRON: Legacy',
                 'year': 2010,
```

### Comparing `trakt.py-4.4.0/tests/sync/watchlist/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/sync/watchlist/test_movies.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # Ensure collection is valid
     assert_that(watchlist, not_none())
 
     # Retrieve values from dictionary
     items = watchlist.values()
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # TRON: Legacy (2010)
         all_of(
             instance_of(Movie),
             has_properties({
                 'pk': ('imdb', 'tt1104001'),
                 'title': 'TRON: Legacy',
                 'year': 2010,
```

### Comparing `trakt.py-4.4.0/tests/test_calendars.py` & `trakt.py-5.0.0.0rc1/tests/test_calendars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa: F403, F405
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 from trakt.interfaces.calendars import Base
 
 from datetime import date, datetime
 from dateutil.tz import tzutc
```

### Comparing `trakt.py-4.4.0/tests/test_configuration.py` & `trakt.py-5.0.0.0rc1/tests/test_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core.semaphore import Semaphore
 from trakt.core.configuration import ConfigurationManager
 
 from threading import Thread
 import threading
 import time
```

### Comparing `trakt.py-4.4.0/tests/test_context_collection.py` & `trakt.py-5.0.0.0rc1/tests/test_context_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.context_collection import ListCollection, ContextCollection
 
 
 def test_list_collection():
     m = ListCollection(
         lambda: [1, 2, 3],
```

### Comparing `trakt.py-4.4.0/tests/test_http.py` & `trakt.py-5.0.0.0rc1/tests/test_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 from requests.exceptions import ConnectionError
 from threading import Event
```

### Comparing `trakt.py-4.4.0/tests/test_interface.py` & `trakt.py-5.0.0.0rc1/tests/test_interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core import exceptions
 from trakt.interfaces.base import Interface
 
 from httmock import HTTMock
 import httmock
 import pytest
```

### Comparing `trakt.py-4.4.0/tests/test_lists.py` & `trakt.py-5.0.0.0rc1/tests/test_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa: F403, F405
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 from trakt.objects import PublicList, User
 
 from hamcrest import *
 from httmock import HTTMock
@@ -11,15 +11,15 @@
 
 def test_popular():
     with HTTMock(mock.fixtures, mock.unknown):
         items = Trakt['lists'].popular()
 
     assert_that(items, all_of(
         has_length(2),
-        contains(
+        contains_exactly(
             all_of(
                 instance_of(PublicList),
                 has_properties({
                     'pk': ('trakt', '1338'),
                     'name': 'Top Chihuahua Movies',
                     'description': 'So cute.',
                     'privacy': 'public',
@@ -104,15 +104,15 @@
 
 def test_trending():
     with HTTMock(mock.fixtures, mock.unknown):
         items = Trakt['lists'].trending()
 
     assert_that(items, all_of(
         has_length(2),
-        contains(
+        contains_exactly(
             all_of(
                 instance_of(PublicList),
                 has_properties({
                     'pk': ('trakt', '1337'),
                     'name': 'Incredible Thoughts',
                     'description': 'How could my brain conceive them?',
                     'privacy': 'public',
```

### Comparing `trakt.py-4.4.0/tests/test_pagination.py` & `trakt.py-5.0.0.0rc1/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/test_popular.py` & `trakt.py-5.0.0.0rc1/tests/test_popular.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/test_progress.py` & `trakt.py-5.0.0.0rc1/tests/test_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from hamcrest import assert_that, has_entries
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/test_recommended.py` & `trakt.py-5.0.0.0rc1/tests/test_recommended.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/test_scrobble.py` & `trakt.py-5.0.0.0rc1/tests/test_scrobble.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/test_search.py` & `trakt.py-5.0.0.0rc1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/test_summary.py` & `trakt.py-5.0.0.0rc1/tests/test_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/test_trending.py` & `trakt.py-5.0.0.0rc1/tests/test_trending.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/test_user.py` & `trakt.py-5.0.0.0rc1/tests/test_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 import pytest
```

### Comparing `trakt.py-4.4.0/tests/users/lists/items/test_movies.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/items/test_movies.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         with Trakt.configuration.auth('mock', 'mock'):
             items = Trakt['users/me/lists/movies'].items()
 
     # Ensure collection is valid
     assert_that(items, not_none())
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # Mad Max: Fury Road
         all_of(
             instance_of(Movie),
             has_properties({
                 'pk': ('imdb', 'tt1392190'),
                 'title': 'Mad Max: Fury Road',
                 'year': 2015,
```

### Comparing `trakt.py-4.4.0/tests/users/lists/items/test_people.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/items/test_people.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         with Trakt.configuration.auth('mock', 'mock'):
             items = Trakt['users/me/lists/people'].items()
 
     # Ensure collection is valid
     assert_that(items, not_none())
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # Bryan Cranston
         all_of(
             instance_of(Person),
             has_properties({
                 'pk': ('tmdb', '17419'),
                 'name': 'Bryan Cranston',
```

### Comparing `trakt.py-4.4.0/tests/users/lists/items/test_shows.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/items/test_shows.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             items = Trakt['users/me/lists/shows'].items()
 
     # Ensure collection is valid
     assert_that(items, not_none())
     assert_that(items, has_length(3))
 
     # Validate items
-    assert_that(items, contains(
+    assert_that(items, contains_exactly(
         # Game of Thrones (2011)
         all_of(
             instance_of(Show),
             has_properties({
                 'pk': ('tvdb', '121361'),
                 'title': 'Game of Thrones',
                 'year': 2011,
```

### Comparing `trakt.py-4.4.0/tests/users/lists/test_actions.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/test_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/users/lists/test_create.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/test_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from datetime import datetime
 from dateutil.tz import tzutc
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/users/lists/test_get.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/test_get.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/tests/users/lists/test_list.py` & `trakt.py-5.0.0.0rc1/tests/users/lists/test_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from datetime import datetime
 from dateutil.tz import tzutc
 from httmock import HTTMock
```

### Comparing `trakt.py-4.4.0/tests/users/test_friends.py` & `trakt.py-5.0.0.0rc1/tests/users/test_friends.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 import datetime
```

### Comparing `trakt.py-4.4.0/tests/users/test_history.py` & `trakt.py-5.0.0.0rc1/tests/users/test_history.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 import datetime
```

### Comparing `trakt.py-4.4.0/tests/users/test_ratings.py` & `trakt.py-5.0.0.0rc1/tests/users/test_ratings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 import datetime
```

### Comparing `trakt.py-4.4.0/tests/users/test_watched.py` & `trakt.py-5.0.0.0rc1/tests/users/test_watched.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa: F403, F405
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 from trakt.objects import Movie, Show, Season, Episode
 
 from datetime import datetime
 from dateutil.tz import tzutc
@@ -19,15 +19,15 @@
 
             assert items is not None
 
             items = list(items)
 
     assert_that(items, all_of(
         has_length(2),
-        contains(
+        contains_exactly(
             all_of(
                 instance_of(Show),
                 has_properties({
                     'title': 'Breaking Bad',
                     'year': 2008,
 
                     'plays': 56,
@@ -217,15 +217,15 @@
 
             assert items is not None
 
             items = list(items)
 
     assert_that(items, all_of(
         has_length(2),
-        contains(
+        contains_exactly(
             all_of(
                 instance_of(Movie),
                 has_properties({
                     'pk': ('imdb', 'tt0372784'),
                     'title': 'Batman Begins',
                     'year': 2005,
```

### Comparing `trakt.py-4.4.0/tests/users/test_watchlist.py` & `trakt.py-5.0.0.0rc1/tests/users/test_watchlist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from tests.core import mock
 from trakt import Trakt
 
 from httmock import HTTMock
 import datetime
```

### Comparing `trakt.py-4.4.0/tox.ini` & `trakt.py-5.0.0.0rc1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 [tox]
-envlist = clean,py27,py35,py36,py37,py38,pypy,stats,flake8
-minversion = 1.6
+requires = 
+  tox>=4
+env_list = clean, py{37,38,39,310,311}, pypy, stats, lint
 skipsdist = True
 
-[travis]
+[gh-actions]
 python =
-  3.7: py37, flake8
+  3.7: py37
+  3.8: py38
+  3.9: py39
+  3.10: py310
+  3.11: py311
+  pypy-3.7: pypy
 
 [testenv]
+description = run unit tests
 deps =
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
-
-  pytest-cov>=2.1.0, <3.0.0
+  pytest-cov>=4.0.0
 commands =
-  py.test --cov-config .coveragerc --cov-append --cov=trakt
+  pytest --cov-config .coveragerc --cov-append --cov=trakt
 
 [testenv:clean]
 skip_install = true
 deps =
   coverage
 commands =
   coverage erase
 
 [testenv:docs]
 commands = sphinx-build -a -b html docs build/sphinx
 
-[testenv:flake8]
-basepython = python3.7
+[testenv:lint]
+basepython = python3.10
 skip_install = true
 deps =
   flake8
   flake8-bugbear>=17.3.0
   flake8-docstrings>=0.2.7
-  flake8-future-import>=0.4.3
-  flake8-import-order>=0.9,<=0.16
-  flake8-import-order-fuzeman>=1.1.1
+  flake8-import-order>=0.18
+  flake8-import-order-fuzeman>=1.8.1
   flake8-quotes>=0.9.0
 commands =
   flake8
 
 [testenv:stats]
 skip_install = true
 deps =
   coverage
 commands =
   coverage report -m
   coverage html
+  coverage lcov
 
 [flake8]
 format=pylint
 statistics = True
 ignore =
   D100,
   D101,
```

### Comparing `trakt.py-4.4.0/trakt/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.client import TraktClient
 from trakt.core.errors import ERRORS
 from trakt.core.exceptions import RequestError, ClientError, ServerError
 from trakt.helpers import has_attribute
 from trakt.version import __version__  # NOQA
 
-from six import add_metaclass
 import logging
 
 
 __all__ = (
     'Trakt',
     'RequestError',
     'ClientError',
@@ -41,16 +40,15 @@
     def __getitem__(self, key):
         if self.client is None:
             self.construct()
 
         return self.client[key]
 
 
-@add_metaclass(TraktMeta)
-class Trakt(object):
+class Trakt(object, metaclass=TraktMeta):
     client = None
 
     @classmethod
     def construct(cls):
         cls.client = TraktClient()
```

### Comparing `trakt.py-4.4.0/trakt/client.py` & `trakt.py-5.0.0.0rc1/trakt/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.configuration import ConfigurationManager
 from trakt.core.emitter import Emitter
 from trakt.core.http import HttpClient
 from trakt.interfaces import construct_map
 from trakt.interfaces.base import InterfaceProxy
 from trakt.mapper.core.base import Mapper
```

### Comparing `trakt.py-4.4.0/trakt/core/configuration.py` & `trakt.py-5.0.0.0rc1/trakt/core/configuration.py`

 * *Files identical despite different names*

### Comparing `trakt.py-4.4.0/trakt/core/context_collection.py` & `trakt.py-5.0.0.0rc1/trakt/core/context_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import synchronized
 
-from six.moves import xrange
-from six.moves import _thread as thread
 from threading import RLock
+import _thread
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class ListCollection(object):
     def __init__(self, *lists):
@@ -67,15 +66,15 @@
         return list.pop(index)
 
     @synchronized(lambda self: self._lock)
     def __eq__(self, other):
         if len(self) != len(other):
             return False
 
-        for x in xrange(len(self)):
+        for x in range(len(self)):
             if self[x] != other[x]:
                 return False
 
         return True
 
     @synchronized(lambda self: self._lock)
     def __contains__(self, value):
@@ -130,27 +129,27 @@
         if ident not in self._threads:
             self._threads[ident] = ListCollection(lambda: self.base, [])
 
         return self._threads[ident]
 
     @property
     def current(self):
-        ident = thread.get_ident()
+        ident = _thread.get_ident()
 
         try:
             return self._threads[ident]
         except KeyError:
             return self.build(ident)
 
     def append(self, value):
         self.current.append(value)
 
     @synchronized(lambda self: self._lock)
     def clear(self):
-        ident = thread.get_ident()
+        ident = _thread.get_ident()
 
         if ident not in self._threads:
             return
 
         del self._threads[ident]
 
     def pop(self, index=None):
```

### Comparing `trakt.py-4.4.0/trakt/core/emitter.py` & `trakt.py-5.0.0.0rc1/trakt/core/emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 import logging
 
 # concurrent.futures is optional
 try:
     from concurrent.futures import ThreadPoolExecutor
 except ImportError:
@@ -45,15 +45,15 @@
         log.debug(
             ('[%s]:' % self.__name.ljust(34)) + str(message),
             *args, **kwargs
         )
 
     def __wrap(self, callback, *args, **kwargs):
         def wrap(func):
-            callback(func=func, *args, **kwargs)
+            callback(*args, func=func, **kwargs)
             return func
 
         return wrap
 
     def on(self, events, func=None, on_bound=None):
         if not func:
             # assume decorator, wrap
```

### Comparing `trakt.py-4.4.0/trakt/core/errors.py` & `trakt.py-5.0.0.0rc1/trakt/core/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa: E241
 
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 
 ERRORS = {
     400: ("Bad Request",            "Request couldn't be parsed"),
     401: ("Unauthorized",           "OAuth must be provided"),
     403: ("Forbidden",              "Invalid API key or unapproved app"),
     404: ("Not Found",              "Method exists, but no record found"),
```

### Comparing `trakt.py-4.4.0/trakt/core/exceptions.py` & `trakt.py-5.0.0.0rc1/trakt/core/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.errors import ERRORS
 
 
 class RequestFailedError(Exception):
     pass
```

### Comparing `trakt.py-4.4.0/trakt/core/helpers.py` & `trakt.py-5.0.0.0rc1/trakt/core/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from __future__ import absolute_import, division, print_function
 
-from six import string_types
+
 import functools
 import logging
 import warnings
 
 try:
     import arrow
 except ImportError:
@@ -52,15 +51,15 @@
 
     return result
 
 
 def synchronized(f_lock, mode='full'):
     if mode == 'full':
         mode = ['acquire', 'release']
-    elif isinstance(mode, string_types):
+    elif isinstance(mode, str):
         mode = [mode]
 
     def wrap(func):
         @functools.wraps(func)
         def wrapped(self, *args, **kwargs):
             lock = f_lock(self)
 
@@ -97,18 +96,29 @@
 def try_convert(value, value_type, default=None):
     try:
         return value_type(value)
     except (ValueError, TypeError):
         return default
 
 
+def reraise(tp, value, tb=None):
+    try:
+        if value is None:
+            value = tp()
+        if value.__traceback__ is not tb:
+            raise value.with_traceback(tb)
+        raise value
+    finally:
+        value = None
+        tb = None
 #
 # Date/Time Conversion
 #
 
+
 @deprecated('`from_iso8601(value)` has been renamed to `from_iso8601_datetime(value)`')
 def from_iso8601(value):
     return from_iso8601_datetime(value)
 
 
 def from_iso8601_date(value):
     if value is None:
```

### Comparing `trakt.py-4.4.0/trakt/core/http.py` & `trakt.py-5.0.0.0rc1/trakt/core/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.configuration import DEFAULT_HTTP_RETRY, DEFAULT_HTTP_MAX_RETRIES, DEFAULT_HTTP_TIMEOUT, \
     DEFAULT_HTTP_RETRY_SLEEP
 from trakt.core.context_stack import ContextStack
-from trakt.core.helpers import synchronized
+from trakt.core.helpers import synchronized, reraise
 from trakt.core.keylock import KeyLock
 from trakt.core.pagination import PaginationIterator
 from trakt.core.request import TraktRequest
 
 from requests.adapters import DEFAULT_POOLBLOCK, HTTPAdapter
 from requests.exceptions import ConnectionError, SSLError
 from requests.packages.urllib3.exceptions import ReadTimeoutError
 from threading import RLock
 import calendar
 import datetime
 import logging
 import requests
-import six
 import socket
 import sys
 import time
 
 try:
     import ssl
 except ImportError:
@@ -169,15 +168,15 @@
 
             # Sleep until next request attempt
             if i < max_retries:
                 time.sleep(retry_sleep)
 
         # Raise last exception
         if exc_info:
-            six.reraise(*exc_info)
+            reraise(*exc_info)
 
         # Return last response
         return response
 
     def delete(self, path=None, params=None, data=None, **kwargs):
         return self.request('DELETE', path, params, data, **kwargs)
```

### Comparing `trakt.py-4.4.0/trakt/core/keylock.py` & `trakt.py-5.0.0.0rc1/trakt/core/keylock.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from threading import Lock
 
 
 class KeyLock(object):
     def __init__(self, lock=Lock):
         self._lock = lock
```

### Comparing `trakt.py-4.4.0/trakt/core/pagination.py` & `trakt.py-5.0.0.0rc1/trakt/core/pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.errors import log_request_error
 from trakt.core.exceptions import ServerError, ClientError, RequestFailedError
 from trakt.core.helpers import try_convert
 
-from six.moves.urllib.parse import urlsplit, urlunsplit, parse_qsl
 import logging
+import urllib.parse as parse
 
 log = logging.getLogger(__name__)
 
 
 class PaginationIterator(object):
     def __init__(self, client, request, exceptions=False):
         self.client = client
@@ -19,18 +19,18 @@
         self.per_page = None
         self.total_items = None
         self.total_pages = None
 
         self._mapper = None
 
         # Parse request url
-        scheme, netloc, path, query = urlsplit(self.request.url)[:4]
+        scheme, netloc, path, query = parse.urlsplit(self.request.url)[:4]
 
-        self.url = urlunsplit([scheme, netloc, path, '', ''])
-        self.query = dict(parse_qsl(query))
+        self.url = parse.urlunsplit([scheme, netloc, path, '', ''])
+        self.query = dict(parse.parse_qsl(query))
 
         # Resolve pagination details
         self.resolve()
 
     def get(self, page):
         request = self.request.copy()
```

### Comparing `trakt.py-4.4.0/trakt/core/request.py` & `trakt.py-5.0.0.0rc1/trakt/core/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from __future__ import absolute_import, division, print_function
+
 
 from requests import Request
-from six.moves.urllib_parse import urlencode
 import json
-import six
+import urllib.parse as parse
 
 
 class TraktRequest(object):
     def __init__(self, client, **kwargs):
         self.client = client
         self.configuration = client.configuration
         self.kwargs = kwargs
@@ -47,15 +46,15 @@
 
         if self.path.endswith('/'):
             self.path = self.path[:-1]
 
         # Transform `params` into list
         self.params = self.kwargs.get('params') or []
 
-        if isinstance(self.params, six.string_types):
+        if isinstance(self.params, str):
             self.params = [self.params]
 
         # Transform `query`
         self.query = self.kwargs.get('query') or {}
 
     def transform_method(self):
         self.method = self.kwargs.get('method')
@@ -118,15 +117,15 @@
         return url
 
     @classmethod
     def encode_query(cls, parameters):
         if not parameters:
             return ''
 
-        return urlencode([
+        return parse.urlencode([
             (key, cls.encode_query_parameter(value))
             for key, value in parameters.items()
             if value is not None
         ])
 
     @classmethod
     def encode_query_parameter(cls, value):
```

### Comparing `trakt.py-4.4.0/trakt/helpers.py` & `trakt.py-5.0.0.0rc1/trakt/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import absolute_import, division, print_function
 
-from six.moves.urllib_parse import urlencode
+
+import urllib.parse as parse
 
 
 def setdefault(d, defaults, func=None):
     for key, value in defaults.items():
         if func and not func(key, value):
             continue
 
@@ -24,9 +24,9 @@
         (key, value)
         for (key, value) in kwargs.items()
         if value
     ]
 
     return ''.join([
         '/'.join([str(x) for x in args]),
-        ('?' + urlencode(parameters)) if parameters else ''
+        ('?' + parse.urlencode(parameters)) if parameters else ''
     ])
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.interfaces import auth
 from trakt.interfaces import calendars
 from trakt.interfaces import lists
 from trakt.interfaces import movies
 from trakt.interfaces import oauth
 from trakt.interfaces import scrobble
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/auth.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.interfaces.base import Interface
 
 import requests
 
 
 class AuthInterface(Interface):
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/base/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.errors import log_request_error
 from trakt.core.exceptions import RequestFailedError, ServerError, ClientError
 from trakt.core.pagination import PaginationIterator
 from trakt.helpers import setdefault
 
 import functools
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/calendars.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/calendars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper.summary import SummaryMapper
 
 from datetime import datetime
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/lists/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/lists/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface
 from trakt.mapper import ListMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/movies/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/movies/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface
 from trakt.mapper.summary import SummaryMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/oauth/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import deprecated
 from trakt.helpers import build_url
 from trakt.interfaces.base import Interface
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/oauth/device.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/oauth/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.emitter import Emitter
 from trakt.interfaces.base import Interface
 
 from datetime import datetime, timedelta
 from threading import Thread
 import calendar
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/scrobble.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/scrobble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.interfaces.base import Interface, authenticated, application
 
 
 class ScrobbleInterface(Interface):
     path = 'scrobble'
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/search.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface
 from trakt.mapper.search import SearchMapper
 
 import requests
-import six
 import warnings
 
 
 class SearchInterface(Interface):
     path = 'search'
 
     def lookup(self, id, service=None, media=None, extended=None, page=None, per_page=None, **kwargs):
@@ -72,15 +71,15 @@
         # Build query
         query = {
             'extended': extended,
             'page': page,
             'limit': per_page
         }
 
-        if isinstance(media, six.string_types):
+        if isinstance(media, str):
             query['type'] = media
         elif isinstance(media, list):
             query['type'] = ','.join(media)
 
         # Send request
         response = self.http.get(
             params=[service, id],
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/shows/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/shows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper.progress import ProgressMapper
 from trakt.mapper.summary import SummaryMapper
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import deprecated, dictfilter
 from trakt.interfaces.base import Interface, authenticated
 from trakt.interfaces.sync.collection import SyncCollectionInterface
 from trakt.interfaces.sync.history import SyncHistoryInterface
 from trakt.interfaces.sync.playback import SyncPlaybackInterface
 from trakt.interfaces.sync.ratings import SyncRatingsInterface
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/collection.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.interfaces.sync.core.mixins import Get, Add, Remove
 
 
 class SyncCollectionInterface(Get, Add, Remove):
     path = 'sync/collection'
     flags = {'is_collected': True}
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/core/mixins.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper.sync import SyncMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/history.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import to_iso8601_datetime
 from trakt.interfaces.base import authenticated
 from trakt.interfaces.sync.core.mixins import Get, Add, Remove
 
 
 class SyncHistoryInterface(Get, Add, Remove):
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/ratings.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/ratings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.interfaces.base import authenticated
 from trakt.interfaces.sync.core.mixins import Get, Add, Remove
 
 
 class SyncRatingsInterface(Get, Add, Remove):
     path = 'sync/ratings'
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/sync/watchlist.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/sync/watchlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.interfaces.base import authenticated
 from trakt.interfaces.sync.core.mixins import Get, Add, Remove
 
 
 class SyncWatchlistInterface(Get, Add, Remove):
     path = 'sync/watchlist'
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.interfaces.users.following import UsersFollowingInterface
 from trakt.interfaces.users.friends import UsersFriendsInterface
 from trakt.interfaces.users.history import UsersHistoryInterface
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/following.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/following.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.interfaces.base import Interface
 from trakt.mapper import UserMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/friends.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/friends.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.interfaces.base import Interface
 from trakt.mapper import UserMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/history.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter, to_iso8601_datetime
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import SyncMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/lists/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/lists/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username
 from trakt.interfaces.base import Interface
 from trakt.mapper import ListMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/lists/list_.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/lists/list_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import ListMapper, ListItemMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/profile.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import UserMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/ratings.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/ratings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import SyncMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/watched.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/watched.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import SyncMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/interfaces/users/watchlist.py` & `trakt.py-5.0.0.0rc1/trakt/interfaces/users/watchlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import clean_username, dictfilter
 from trakt.core.pagination import PaginationIterator
 from trakt.interfaces.base import Interface, authenticated
 from trakt.mapper import SyncMapper
 
 import requests
```

### Comparing `trakt.py-4.4.0/trakt/mapper/__init__.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.comment import CommentMapper
 from trakt.mapper.list import ListMapper
 from trakt.mapper.list_item import ListItemMapper
 from trakt.mapper.progress import ProgressMapper
 from trakt.mapper.search import SearchMapper
 from trakt.mapper.summary import SummaryMapper
```

### Comparing `trakt.py-4.4.0/trakt/mapper/core/base.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/core/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.objects import User, Movie, Show, Episode, Season, CustomList, Comment, Person, PublicList,\
     WatchedProgress, CollectionProgress
 
 IDENTIFIERS = {
     'movie': [
         'imdb',
```

### Comparing `trakt.py-4.4.0/trakt/mapper/list.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 from trakt.mapper.user import UserMapper
 
 
 class ListMapper(Mapper):
     @classmethod
```

### Comparing `trakt.py-4.4.0/trakt/mapper/list_item.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/list_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 
 
 class ListItemMapper(Mapper):
     @classmethod
     def process(cls, client, item, media=None, **kwargs):
```

### Comparing `trakt.py-4.4.0/trakt/mapper/progress.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/progress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 
 
 class ProgressMapper(Mapper):
     @classmethod
     def progress(cls, client, progress_type, item, **kwargs):
```

### Comparing `trakt.py-4.4.0/trakt/mapper/search.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 
 import logging
 
 log = logging.getLogger(__name__)
```

### Comparing `trakt.py-4.4.0/trakt/mapper/summary.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 
 
 class SummaryMapper(Mapper):
     @classmethod
     def movies(cls, client, items, **kwargs):
```

### Comparing `trakt.py-4.4.0/trakt/mapper/sync.py` & `trakt.py-5.0.0.0rc1/trakt/mapper/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.mapper.core.base import Mapper
 
 import logging
 
 log = logging.getLogger(__name__)
```

### Comparing `trakt.py-4.4.0/trakt/objects/comment.py` & `trakt.py-5.0.0.0rc1/trakt/objects/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 
 
 class Comment(object):
     def __init__(self, client, keys):
```

### Comparing `trakt.py-4.4.0/trakt/objects/episode.py` & `trakt.py-5.0.0.0rc1/trakt/objects/episode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime, to_iso8601_datetime, deprecated
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.video import Video
 
 
 class Episode(Video):
```

### Comparing `trakt.py-4.4.0/trakt/objects/list/base.py` & `trakt.py-5.0.0.0rc1/trakt/objects/list/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 
 
 class List(object):
     def __init__(self, client, keys, user):
```

### Comparing `trakt.py-4.4.0/trakt/objects/list/custom.py` & `trakt.py-5.0.0.0rc1/trakt/objects/list/custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.objects.list.base import List
 
 
 class CustomList(List):
     @classmethod
     def _construct(cls, client, keys, info, user):
```

### Comparing `trakt.py-4.4.0/trakt/objects/media.py` & `trakt.py-5.0.0.0rc1/trakt/objects/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.rating import Rating
 
 
 class Media(object):
```

### Comparing `trakt.py-4.4.0/trakt/objects/movie.py` & `trakt.py-5.0.0.0rc1/trakt/objects/movie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime, to_iso8601_datetime,\
     from_iso8601_date, to_iso8601_date, deprecated
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.video import Video
```

### Comparing `trakt.py-4.4.0/trakt/objects/person.py` & `trakt.py-5.0.0.0rc1/trakt/objects/person.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 
 
 class Person(object):
     def __init__(self, client, keys=None, index=None):
```

### Comparing `trakt.py-4.4.0/trakt/objects/progress.py` & `trakt.py-5.0.0.0rc1/trakt/objects/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import dictfilter, from_iso8601_datetime, to_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 
 LABELS = {
     'last_progress_change': {
         'watched': 'last_watched_at',
```

### Comparing `trakt.py-4.4.0/trakt/objects/rating.py` & `trakt.py-5.0.0.0rc1/trakt/objects/rating.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 
 
 class Rating(object):
     def __init__(self, client, value=None, timestamp=None, votes=None):
         self._client = client
```

### Comparing `trakt.py-4.4.0/trakt/objects/season.py` & `trakt.py-5.0.0.0rc1/trakt/objects/season.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import to_iso8601_datetime, from_iso8601_datetime, deprecated
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.media import Media
 
 
 class Season(Media):
```

### Comparing `trakt.py-4.4.0/trakt/objects/show.py` & `trakt.py-5.0.0.0rc1/trakt/objects/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime, to_iso8601_datetime, deprecated
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.media import Media
 
-from six import iteritems
-
 
 class Show(Media):
     def __init__(self, client, keys, index=None):
         super(Show, self).__init__(client, keys, index)
 
         self.title = None
         """
@@ -146,17 +144,17 @@
     def episodes(self):
         """Return a flat episode iterator.
 
         :returns: Iterator :code:`((season_num, episode_num), Episode)`
         :rtype: iterator
         """
 
-        for sk, season in iteritems(self.seasons):
+        for sk, season in self.seasons.iteritems():
             # Yield each episode in season
-            for ek, episode in iteritems(season.episodes):
+            for ek, episode in season.episodes.iteritems():
                 yield (sk, ek), episode
 
     def to_identifier(self):
         """Return the show identifier which is compatible with requests that require show definitions.
 
         :return: Show identifier/definition
         :rtype: :class:`~python:dict`
```

### Comparing `trakt.py-4.4.0/trakt/objects/user.py` & `trakt.py-5.0.0.0rc1/trakt/objects/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 
 
 class User(object):
     def __init__(self, client, keys):
```

### Comparing `trakt.py-4.4.0/trakt/objects/video.py` & `trakt.py-5.0.0.0rc1/trakt/objects/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+
 
 from trakt.core.helpers import from_iso8601_datetime
 from trakt.objects.core.helpers import update_attributes
 from trakt.objects.media import Media
 
 
 class Video(Media):
```

### Comparing `trakt.py-4.4.0/trakt/sphinxext.py` & `trakt.py-5.0.0.0rc1/trakt/sphinxext.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 from trakt import interfaces
 import trakt  # noqa: I902
 
 from docutils import nodes
 from docutils.parsers import rst
 from docutils.parsers.rst import directives
 from docutils.statemachine import ViewList
 from sphinx.util.nodes import nested_parse_with_titles
 import collections
 import inspect
-import six
 
 
 def _get_methods(obj):
     for (name, _) in inspect.getmembers(obj, predicate=inspect.ismethod):
         if name.startswith('_'):
             continue
 
@@ -24,16 +21,16 @@
 def _format_apis(apis):
 
     output = []
 
     def make_path(path_dict, api_path):
 
         sorted_paths = collections.OrderedDict(
-            sorted(six.iteritems(path_dict)))
-        for k, v in six.iteritems(sorted_paths):
+            sorted(path_dict.iteritems()))
+        for k, v in sorted_paths.iteritems():
             if k is None:
                 k = ''
             api_path.append(k)
 
             if isinstance(v, dict):
                 api_path = make_path(v, api_path)
             else:
```

### Comparing `trakt.py-4.4.0/trakt.py.egg-info/SOURCES.txt` & `trakt.py-5.0.0.0rc1/trakt.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 .gitignore
 AUTHORS
 CHANGES.rst
 CONTRIBUTING.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
+build-requirements.txt
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
+.github/workflows/publish.yml
+.github/workflows/test.yml
 docs/changes.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
 docs/_templates/sidebar_header.html
 docs/_templates/sidebar_index.html
 docs/sourcecode/interfaces.rst
@@ -365,15 +369,14 @@
 tests/users/lists/items/__init__.py
 tests/users/lists/items/test_movies.py
 tests/users/lists/items/test_people.py
 tests/users/lists/items/test_shows.py
 trakt/__init__.py
 trakt/client.py
 trakt/helpers.py
-trakt/hooks.py
 trakt/sphinxext.py
 trakt/version.py
 trakt.py.egg-info/PKG-INFO
 trakt.py.egg-info/SOURCES.txt
 trakt.py.egg-info/dependency_links.txt
 trakt.py.egg-info/not-zip-safe
 trakt.py.egg-info/pbr.json
```

