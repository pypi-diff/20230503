# Comparing `tmp/shikithon-2.4.2.tar.gz` & `tmp/shikithon-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shikithon-2.4.2.tar", max compression
+gzip compressed data, was "shikithon-2.5.tar", max compression
```

## Comparing `shikithon-2.4.2.tar` & `shikithon-2.5.tar`

### file list

```diff
@@ -1,131 +1,135 @@
--rw-r--r--   0        0        0     1070 2023-04-15 16:01:18.885165 shikithon-2.4.2/LICENSE
--rw-r--r--   0        0        0    12407 2023-04-15 16:01:18.885165 shikithon-2.4.2/README.md
--rw-r--r--   0        0        0     1188 2023-04-15 16:01:18.885165 shikithon-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      262 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/__init__.py
--rw-r--r--   0        0        0     3903 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/api.py
--rw-r--r--   0        0        0    22001 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/base_client.py
--rw-r--r--   0        0        0      189 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/__init__.py
--rw-r--r--   0        0        0     2074 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/exceptions_handler.py
--rw-r--r--   0        0        0     1616 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/decorators/method_endpoint.py
--rw-r--r--   0        0        0    34606 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/endpoints.py
--rw-r--r--   0        0        0     1648 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/__init__.py
--rw-r--r--   0        0        0     2705 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/anime.py
--rw-r--r--   0        0        0      895 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/club.py
--rw-r--r--   0        0        0      632 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/comment.py
--rw-r--r--   0        0        0      310 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/enhanced_enum.py
--rw-r--r--   0        0        0      289 2023-04-15 16:01:18.885165 shikithon-2.4.2/shikithon/enums/favorite.py
--rw-r--r--   0        0        0      222 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/history.py
--rw-r--r--   0        0        0     1961 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/manga.py
--rw-r--r--   0        0        0      286 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/message.py
--rw-r--r--   0        0        0      466 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/person.py
--rw-r--r--   0        0        0     1522 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/ranobe.py
--rw-r--r--   0        0        0      240 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/request.py
--rw-r--r--   0        0        0      218 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/response.py
--rw-r--r--   0        0        0      198 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/style.py
--rw-r--r--   0        0        0     1999 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/topic.py
--rw-r--r--   0        0        0      685 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/user_rate.py
--rw-r--r--   0        0        0      380 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/enums/video.py
--rw-r--r--   0        0        0      657 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/__init__.py
--rw-r--r--   0        0        0      276 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/already_running_client.py
--rw-r--r--   0        0        0      329 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/invalid_content_type.py
--rw-r--r--   0        0        0      732 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/missing_app_variable.py
--rw-r--r--   0        0        0      231 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/retry_later.py
--rw-r--r--   0        0        0      358 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/shikimori_api_response_error.py
--rw-r--r--   0        0        0      240 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/shikithon_exception.py
--rw-r--r--   0        0        0      234 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/exceptions/store_exception.py
--rw-r--r--   0        0        0     1689 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/__init__.py
--rw-r--r--   0        0        0      230 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/abuse_response.py
--rw-r--r--   0        0        0      303 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/achievement.py
--rw-r--r--   0        0        0      190 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/activity.py
--rw-r--r--   0        0        0     1735 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/anime.py
--rw-r--r--   0        0        0      410 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/ban.py
--rw-r--r--   0        0        0      270 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/birthday.py
--rw-r--r--   0        0        0      331 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/calendar_event.py
--rw-r--r--   0        0        0      796 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/character.py
--rw-r--r--   0        0        0      789 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/club.py
--rw-r--r--   0        0        0      290 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/club_image.py
--rw-r--r--   0        0        0      488 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/comment.py
--rw-r--r--   0        0        0      688 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/constants.py
--rw-r--r--   0        0        0      207 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/created_user_image.py
--rw-r--r--   0        0        0      218 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/dialog.py
--rw-r--r--   0        0        0      243 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/favourite.py
--rw-r--r--   0        0        0      452 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/favourites.py
--rw-r--r--   0        0        0      195 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/forum.py
--rw-r--r--   0        0        0      327 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/franchise_tree.py
--rw-r--r--   0        0        0      186 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/genre.py
--rw-r--r--   0        0        0      401 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/history.py
--rw-r--r--   0        0        0      196 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/image.py
--rw-r--r--   0        0        0      414 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/link.py
--rw-r--r--   0        0        0      492 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/linked_topic.py
--rw-r--r--   0        0        0      199 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/logo.py
--rw-r--r--   0        0        0     1645 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/manga.py
--rw-r--r--   0        0        0      564 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/message.py
--rw-r--r--   0        0        0      956 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/person.py
--rw-r--r--   0        0        0      158 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/publisher.py
--rw-r--r--   0        0        0     1572 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/ranobe.py
--rw-r--r--   0        0        0      161 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/rating.py
--rw-r--r--   0        0        0      277 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/rating_list.py
--rw-r--r--   0        0        0      379 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/relation.py
--rw-r--r--   0        0        0      356 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/role.py
--rw-r--r--   0        0        0      271 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/roles.py
--rw-r--r--   0        0        0      158 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/score.py
--rw-r--r--   0        0        0      241 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/score_list.py
--rw-r--r--   0        0        0      171 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/screenshot.py
--rw-r--r--   0        0        0      234 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/seyu.py
--rw-r--r--   0        0        0      857 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/stats.py
--rw-r--r--   0        0        0      206 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/status.py
--rw-r--r--   0        0        0      246 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/status_list.py
--rw-r--r--   0        0        0      249 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/studio.py
--rw-r--r--   0        0        0      388 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/style.py
--rw-r--r--   0        0        0      808 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/topic.py
--rw-r--r--   0        0        0      252 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/tree_link.py
--rw-r--r--   0        0        0      301 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/tree_node.py
--rw-r--r--   0        0        0      155 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/type.py
--rw-r--r--   0        0        0      235 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/type_list.py
--rw-r--r--   0        0        0      243 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/unread_messages.py
--rw-r--r--   0        0        0      853 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user.py
--rw-r--r--   0        0        0      229 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_image.py
--rw-r--r--   0        0        0      703 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_list.py
--rw-r--r--   0        0        0      538 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate.py
--rw-r--r--   0        0        0      167 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate_score.py
--rw-r--r--   0        0        0      169 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/user_rate_status.py
--rw-r--r--   0        0        0      287 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/video.py
--rw-r--r--   0        0        0      328 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/models/works.py
--rw-r--r--   0        0        0        0 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/py.typed
--rw-r--r--   0        0        0     1294 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/abuse_requests.py
--rw-r--r--   0        0        0     1173 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/achievements.py
--rw-r--r--   0        0        0    14250 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/animes.py
--rw-r--r--   0        0        0     1157 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/appears.py
--rw-r--r--   0        0        0     1316 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/bans.py
--rw-r--r--   0        0        0      162 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/base_resource.py
--rw-r--r--   0        0        0     1291 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/calendars.py
--rw-r--r--   0        0        0     1813 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/characters.py
--rw-r--r--   0        0        0    12292 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/clubs.py
--rw-r--r--   0        0        0     6300 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/comments.py
--rw-r--r--   0        0        0     3222 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/constants.py
--rw-r--r--   0        0        0     2437 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/dialogs.py
--rw-r--r--   0        0        0     3682 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/favorites.py
--rw-r--r--   0        0        0      909 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/forums.py
--rw-r--r--   0        0        0     1480 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/friends.py
--rw-r--r--   0        0        0      908 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/genres.py
--rw-r--r--   0        0        0     9698 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/mangas.py
--rw-r--r--   0        0        0     6548 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/messages.py
--rw-r--r--   0        0        0     2005 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/people.py
--rw-r--r--   0        0        0      952 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/publishers.py
--rw-r--r--   0        0        0     9513 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/ranobes.py
--rw-r--r--   0        0        0      748 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/stats.py
--rw-r--r--   0        0        0      919 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/studios.py
--rw-r--r--   0        0        0     4178 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/styles.py
--rw-r--r--   0        0        0     9881 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/topics.py
--rw-r--r--   0        0        0     1533 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/user_images.py
--rw-r--r--   0        0        0    10984 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/user_rates.py
--rw-r--r--   0        0        0    15779 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/resources/users.py
--rw-r--r--   0        0        0      217 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/__init__.py
--rw-r--r--   0        0        0     4117 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/base.py
--rw-r--r--   0        0        0     3143 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/json.py
--rw-r--r--   0        0        0     4428 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/memory.py
--rw-r--r--   0        0        0     1190 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/store/null.py
--rw-r--r--   0        0        0       82 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/utils/__init__.py
--rw-r--r--   0        0        0    12419 2023-04-15 16:01:18.889165 shikithon-2.4.2/shikithon/utils/utils.py
--rw-r--r--   0        0        0    13547 1970-01-01 00:00:00.000000 shikithon-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-03 12:49:40.722659 shikithon-2.5/LICENSE
+-rw-r--r--   0        0        0    12299 2023-05-03 12:49:40.722659 shikithon-2.5/README.md
+-rw-r--r--   0        0        0     1220 2023-05-03 12:49:40.722659 shikithon-2.5/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/__init__.py
+-rw-r--r--   0        0        0     3958 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/api.py
+-rw-r--r--   0        0        0    22018 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/base_client.py
+-rw-r--r--   0        0        0      189 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/exceptions_handler.py
+-rw-r--r--   0        0        0     1617 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/decorators/method_endpoint.py
+-rw-r--r--   0        0        0    35815 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/endpoints.py
+-rw-r--r--   0        0        0     1699 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/__init__.py
+-rw-r--r--   0        0        0     2707 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/anime.py
+-rw-r--r--   0        0        0      897 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/club.py
+-rw-r--r--   0        0        0      634 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/comment.py
+-rw-r--r--   0        0        0      312 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/enhanced_enum.py
+-rw-r--r--   0        0        0      291 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/favorite.py
+-rw-r--r--   0        0        0      225 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/history.py
+-rw-r--r--   0        0        0     1963 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/manga.py
+-rw-r--r--   0        0        0      289 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/message.py
+-rw-r--r--   0        0        0      470 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/person.py
+-rw-r--r--   0        0        0     1524 2023-05-03 12:49:40.722659 shikithon-2.5/shikithon/enums/ranobe.py
+-rw-r--r--   0        0        0      240 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/request.py
+-rw-r--r--   0        0        0      218 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/response.py
+-rw-r--r--   0        0        0      247 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/review.py
+-rw-r--r--   0        0        0      200 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/style.py
+-rw-r--r--   0        0        0     2001 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/topic.py
+-rw-r--r--   0        0        0      712 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/user_rate.py
+-rw-r--r--   0        0        0      382 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/enums/video.py
+-rw-r--r--   0        0        0      657 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/already_running_client.py
+-rw-r--r--   0        0        0      329 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/invalid_content_type.py
+-rw-r--r--   0        0        0      732 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/missing_app_variable.py
+-rw-r--r--   0        0        0      231 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/retry_later.py
+-rw-r--r--   0        0        0      358 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/shikimori_api_response_error.py
+-rw-r--r--   0        0        0      240 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/shikithon_exception.py
+-rw-r--r--   0        0        0      235 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/exceptions/store_exception.py
+-rw-r--r--   0        0        0     2167 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/abuse_response.py
+-rw-r--r--   0        0        0      306 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/achievement.py
+-rw-r--r--   0        0        0      193 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/activity.py
+-rw-r--r--   0        0        0     1676 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/anime.py
+-rw-r--r--   0        0        0      433 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/ban.py
+-rw-r--r--   0        0        0      342 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/calendar_event.py
+-rw-r--r--   0        0        0      855 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/character.py
+-rw-r--r--   0        0        0      803 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/club.py
+-rw-r--r--   0        0        0      293 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/club_image.py
+-rw-r--r--   0        0        0      590 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/comment.py
+-rw-r--r--   0        0        0     1579 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/constants.py
+-rw-r--r--   0        0        0      210 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/created_user_image.py
+-rw-r--r--   0        0        0      727 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/critique.py
+-rw-r--r--   0        0        0      276 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/date.py
+-rw-r--r--   0        0        0      238 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/dialog.py
+-rw-r--r--   0        0        0      246 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/favourite.py
+-rw-r--r--   0        0        0      455 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/favourites.py
+-rw-r--r--   0        0        0      199 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/forum.py
+-rw-r--r--   0        0        0      330 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/franchise_tree.py
+-rw-r--r--   0        0        0      228 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/genre.py
+-rw-r--r--   0        0        0      428 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/history.py
+-rw-r--r--   0        0        0      196 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/image.py
+-rw-r--r--   0        0        0      417 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/link.py
+-rw-r--r--   0        0        0      613 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/linked_topic.py
+-rw-r--r--   0        0        0      202 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/logo.py
+-rw-r--r--   0        0        0     1751 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/manga.py
+-rw-r--r--   0        0        0      647 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/message.py
+-rw-r--r--   0        0        0     1008 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/person.py
+-rw-r--r--   0        0        0      161 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/publisher.py
+-rw-r--r--   0        0        0     1663 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/ranobe.py
+-rw-r--r--   0        0        0      164 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/rating.py
+-rw-r--r--   0        0        0      280 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/rating_list.py
+-rw-r--r--   0        0        0      406 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/relation.py
+-rw-r--r--   0        0        0      578 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/review.py
+-rw-r--r--   0        0        0      376 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/role.py
+-rw-r--r--   0        0        0      290 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/roles.py
+-rw-r--r--   0        0        0      161 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/score.py
+-rw-r--r--   0        0        0      244 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/score_list.py
+-rw-r--r--   0        0        0      174 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/screenshot.py
+-rw-r--r--   0        0        0      237 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/seyu.py
+-rw-r--r--   0        0        0      860 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/stats.py
+-rw-r--r--   0        0        0      209 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/status.py
+-rw-r--r--   0        0        0      249 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/status_list.py
+-rw-r--r--   0        0        0      252 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/studio.py
+-rw-r--r--   0        0        0      500 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/style.py
+-rw-r--r--   0        0        0     1600 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/topic.py
+-rw-r--r--   0        0        0      255 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/tree_link.py
+-rw-r--r--   0        0        0      304 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/tree_node.py
+-rw-r--r--   0        0        0      158 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/type.py
+-rw-r--r--   0        0        0      238 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/type_list.py
+-rw-r--r--   0        0        0      247 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/unread_messages.py
+-rw-r--r--   0        0        0      903 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user.py
+-rw-r--r--   0        0        0      232 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_image.py
+-rw-r--r--   0        0        0      726 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_list.py
+-rw-r--r--   0        0        0      543 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate.py
+-rw-r--r--   0        0        0      170 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate_score.py
+-rw-r--r--   0        0        0      172 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/user_rate_status.py
+-rw-r--r--   0        0        0      290 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/video.py
+-rw-r--r--   0        0        0      355 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/models/works.py
+-rw-r--r--   0        0        0        0 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/py.typed
+-rw-r--r--   0        0        0     1338 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/__init__.py
+-rw-r--r--   0        0        0     4706 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/abuse_requests.py
+-rw-r--r--   0        0        0     1176 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/achievements.py
+-rw-r--r--   0        0        0    14269 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/animes.py
+-rw-r--r--   0        0        0     1160 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/appears.py
+-rw-r--r--   0        0        0     1319 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/bans.py
+-rw-r--r--   0        0        0      162 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/base_resource.py
+-rw-r--r--   0        0        0     1294 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/calendars.py
+-rw-r--r--   0        0        0     1839 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/characters.py
+-rw-r--r--   0        0        0    13716 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/clubs.py
+-rw-r--r--   0        0        0     6302 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/comments.py
+-rw-r--r--   0        0        0     3218 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/constants.py
+-rw-r--r--   0        0        0     2440 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/dialogs.py
+-rw-r--r--   0        0        0     3684 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/favorites.py
+-rw-r--r--   0        0        0      912 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/forums.py
+-rw-r--r--   0        0        0     1483 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/friends.py
+-rw-r--r--   0        0        0      911 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/genres.py
+-rw-r--r--   0        0        0     9732 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/mangas.py
+-rw-r--r--   0        0        0     6578 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/messages.py
+-rw-r--r--   0        0        0     2028 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/people.py
+-rw-r--r--   0        0        0      955 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/publishers.py
+-rw-r--r--   0        0        0     9542 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/ranobes.py
+-rw-r--r--   0        0        0     4380 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/reviews.py
+-rw-r--r--   0        0        0      751 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/stats.py
+-rw-r--r--   0        0        0      922 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/studios.py
+-rw-r--r--   0        0        0     4153 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/styles.py
+-rw-r--r--   0        0        0     9901 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/topics.py
+-rw-r--r--   0        0        0     1536 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/user_images.py
+-rw-r--r--   0        0        0    10959 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/user_rates.py
+-rw-r--r--   0        0        0    15848 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/resources/users.py
+-rw-r--r--   0        0        0      217 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/base.py
+-rw-r--r--   0        0        0     3142 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/json.py
+-rw-r--r--   0        0        0     4427 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/memory.py
+-rw-r--r--   0        0        0     1189 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/store/null.py
+-rw-r--r--   0        0        0       82 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/utils/__init__.py
+-rw-r--r--   0        0        0    13234 2023-05-03 12:49:40.726659 shikithon-2.5/shikithon/utils/utils.py
+-rw-r--r--   0        0        0    13437 1970-01-01 00:00:00.000000 shikithon-2.5/PKG-INFO
```

### Comparing `shikithon-2.4.2/LICENSE` & `shikithon-2.5/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 SecondThundeR
+Copyright (c) 2022-2023 SecondThundeR
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `shikithon-2.4.2/README.md` & `shikithon-2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,31 @@
 > На данный момент, библиотека находится в статусе поддержки (новые функции будут добавляться только по необходимости)
 >
 > Начиная с версии 2.0.0, библиотека поддерживает асинхронные запросы, отдельные пути к ресурсам API и многое другое
 > _[(Инструкция по миграции с версии 1.x.x)](https://github.com/SecondThundeR/shikithon/wiki/%D0%9C%D0%B8%D0%B3%D1%80%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%81-v1-%D0%BD%D0%B0-v2)_
 
 ## Описание
 
-Данный враппер предоставляет абстракцию, которая позволяет удобнее работать с методами API и их ответами.
+Данный враппер предоставляет абстракцию, которая позволяет удобнее работать с методами API и их ответами
 
-Для каждого эндпоинта API существует свой объект с методами, которые благодаря библиотеке Pydantic,
-возвращают удобную модель данных.
-
-Все данные, возвращаемые API Shikimori, валидируются и парсятся в модели, со всеми необходимыми полями,
+Для каждого эндпоинта API существует свой объект с методами, и все данные, возвращаемые API Shikimori, валидируются и парсятся в модели, со всеми необходимыми полями,
 а также дополнительными, которые могут вернуть некоторые методы API _(Например /users/whoami и /users/:id/info возвращают разные поля)_.
-Это позволяет не задумываться об обработке очередного ответа от сервера и сосредоточиться над реализацией своей идеи.
+Это позволяет не задумываться об обработке очередного ответа от сервера и сосредоточиться над реализацией своей идеи
 
-Также благодаря многочисленным проверкам при взамодействии с запросами, библиотека старается добиться максимально
-безопасной работы с API: все ошибки API, переданных параметров, данных и т.д. обратываются и логируются и
-возвращаются значения по умолчанию
+Также благодаря множеству проверок при взаимодействии с запросами, библиотека старается добиться максимально
+безопасной работы с API: все ошибки API, переданных параметров, данных и т.д. обратываются, логируются и
+пользователю возвращаются значения по умолчанию
 
 > Данная библиотека начинает свою поддержку с Python 3.8.10.
 
 ## Установка
 
- ```pip install shikithon```
+```shell
+pip install shikithon
+```
 
 ## Пример использования
 
 ```py
 import asyncio
 
 from typing import Dict
@@ -63,15 +62,15 @@
 
 # Или же прочитать его из внешнего файла
 with open("config.json", "r", encoding="utf-8") as config_file:
     config_2: Dict[str, str] = loads(config_file.read())
 
 # Инициализируем API объект с необходимыми опциями
 # В данном примере используется JSONStore и отключено логирование
-api = ShikimoriAPI(app_name=config['app_name'], store=JSONStore(), logging=False)
+api = ShikimoriAPI(app_name=config['app_name'], store=JSONStore())
 
 async def main():
     # Используем объект без авторизации
     async with api:
         lycoris = await api.animes.get(50709)
         print(lycoris)
         # >> id=50709 name='Lycoris Recoil' russian='Ликорис Рикоил' ...
@@ -82,15 +81,15 @@
     # Вариант 1
     async with api.auth(
         client_id=config["client_id"],
         client_secret=config["client_secret"],
         auth_code=config["auth_code"],
     ):
         print(await api.users.current())
-        # >> User(id=723052, nickname='SecondThundeR', ...
+        # >> UserBrief(id=723052, nickname='SecondThundeR', ...
 
     # Вариант 2
 
     # Создаем новый объект API
     # (По умолчанию используется NullStore в качестве хранилища)
     api_2 = ShikimoriAPI(app_name="...")
 
@@ -129,17 +128,17 @@
             api.characters.search("Тисато Нисикиги"),
             api.ranobes.get_all(search="Ликорис"),
         ])
         print(chainsaw)
         print(lycoris_chisato[:1])
         print(lycoris_ranobe)
 
-# [Anime(id=44511, name='Chainsaw Man', russian='Человек-бензопила', ...]
-# [Character(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
-# [Ranobe(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
+# [AnimeInfo(id=44511, name='Chainsaw Man', russian='Человек-бензопила', ...]
+# [CharacterInfo(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
+# [RanobeInfo(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
 ```
 
 Также, если хочется узнать как использовать встроенные хранилища конфигов или хочется создать свой,
 посмотрите [этот гайд](https://github.com/SecondThundeR/shikithon/wiki/%D0%93%D0%B0%D0%B9%D0%B4-%D0%BF%D0%BE-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B0%D0%BC-%D0%BA%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D0%B8)
 
 ### Пара уточнений по использованию
 
@@ -195,13 +194,13 @@
 
 ## Лицензия проекта
 
 Данный проект имеет MIT лицензию.
 Ознакомиться с ее содержанием можно [здесь](https://github.com/SecondThundeR/shikithon/blob/main/LICENSE)
 
 Проект использует логотип сайта [Shikimori](https://shikimori.org) для логотипа в этом README.md.
-Все права принадлежат правообладателям и используются по принципу _fair use_.
+Все права принадлежат правообладателям и используются по принципу _fair use_
 
 ## Благодарности
 
 - [shiki4py](https://github.com/ren3104/Shiki4py) - взяты некоторые идеи по рефакторингу и добавлению поддержки асинхронных запросов
 [(Лицензия)](https://github.com/ren3104/Shiki4py/blob/main/LICENSE)
```

### Comparing `shikithon-2.4.2/pyproject.toml` & `shikithon-2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shikithon"
-version = "2.4.2"
+version = "2.5"
 description = "Yet another Python wrapper for Shikimori API"
 authors = [
     "SecondThundeR <awayfromgalaxy@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SecondThundeR/shikithon"
@@ -26,25 +26,28 @@
 generate-setup-file = false
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 check_untyped_defs = true
 warn_redundant_casts = true
+plugins = [
+    "pydantic.mypy"
+]
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
 pydantic = "^1.10.7"
 loguru = "^0.7.0"
 validators ="^0.20.0"
 aiohttp = "^3.8.4"
 pyrate-limiter = "^2.10.0"
 backoff = "^2.2.1"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.2.2"
+pre-commit = "^3.3.1"
 mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shikithon-2.4.2/shikithon/api.py` & `shikithon-2.5/shikithon/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Shikithon API Module.
 
 This is main module with a class
-for interacting with the Shikimori API.
+for interacting with the Shikimori API
 """
 import sys
 from typing import Optional, TypeVar
 
 from loguru import logger
 
 from .base_client import Client
 from .resources import (AbuseRequests, Achievements, Animes, Appears, Bans,
                         Calendars, Characters, Clubs, Comments, Constants,
                         Dialogs, Favorites, Forums, Friends, Genres, Mangas,
-                        Messages, People, Publishers, Ranobes, Stats, Studios,
-                        Styles, Topics, UserImages, UserRates, Users)
+                        Messages, People, Publishers, Ranobes, Reviews, Stats,
+                        Studios, Styles, Topics, UserImages, UserRates, Users)
 from .store import NullStore, Store
 
 RT = TypeVar('RT')
 
 
 class ShikimoriAPI(Client):
     """Main class for interacting with the API.
 
     Current API class uses base client for interacting with API.
-    Also, all API methods splitted up to resources for convinient usage.
+    Also, all API methods splitted up to resources for convinient usage
     """
 
     __slots__ = ('achievements', 'animes', 'appears', 'bans', 'calendars',
                  'characters', 'clubs', 'comments', 'constants', 'dialogs',
                  'favorites', 'forums', 'friends', 'genres', 'mangas',
-                 'messages', 'people', 'publishers', 'ranobes', 'stats',
-                 'studios', 'styles', 'topics', 'user_images', 'user_rates',
-                 'users', 'abuse_requests')
+                 'messages', 'people', 'publishers', 'ranobes', 'reviews',
+                 'stats', 'studios', 'styles', 'topics', 'user_images',
+                 'user_rates', 'users', 'abuse_requests')
 
     def __init__(self,
                  app_name: str = 'Api Test',
                  store: Store = NullStore(),
                  auto_close_store: bool = True,
                  logging: Optional[bool] = False):
         """Shikimori API class initialization.
@@ -95,14 +95,15 @@
         self.friends = Friends(self)
         self.genres = Genres(self)
         self.mangas = Mangas(self)
         self.messages = Messages(self)
         self.people = People(self)
         self.publishers = Publishers(self)
         self.ranobes = Ranobes(self)
+        self.reviews = Reviews(self)
         self.stats = Stats(self)
         self.studios = Studios(self)
         self.styles = Styles(self)
         self.topics = Topics(self)
         self.user_images = UserImages(self)
         self.user_rates = UserRates(self)
         self.users = Users(self)
```

### Comparing `shikithon-2.4.2/shikithon/base_client.py` & `shikithon-2.5/shikithon/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 request_limiter = Limiter(second_rate, minute_rate)
 
 
 class Client:
     """Base client class for shikithon API class.
 
     Contains logic and methods for making requests to the shikimori API
-    as well as validating config and etc.
+    as well as validating config and etc
     """
 
     __slots__ = ('endpoints', '_app_name', '_store', '_auto_close_store',
                  '_session', '_config')
 
     def __init__(self,
                  app_name: str = 'Api Test',
@@ -142,41 +142,41 @@
 
     authorization_header = property(fset=_set_authorization_header)
 
     @property
     def config(self) -> Optional[ClientConfig]:
         """Returns current config.
 
-        If config is not availble, returns None.
+        If config is not availble, returns None
 
         :return: Current config
         :rtype: Optional[ClientConfig]
         """
         return self._config
 
     @config.setter
     def config(self, config: Optional[ClientConfig]):
         """Sets new config.
 
-        If passed config isn't valid, raises Exception.
+        If passed config isn't valid, raises Exception
 
         :param config: New config data
         :type config: Optional[ClientConfig]
         """
         if config is None:
             return None
 
         self.validate_config(config)
 
         self._config = config
 
     def validate_config(self, config: ClientConfig):
         """Validates passed config.
 
-        Method checks config for required dict keys.
+        Method checks config for required dict keys
 
         :param config: Config to validate
         :type config: ClientConfig
 
         :return: True if config is valid, False otherwise
         :rtype: bool
 
@@ -404,19 +404,15 @@
         logger.debug('Checking if token is expired')
 
         token_expiration_status = int(time()) > token_expire_at
 
         logger.debug(f'Token expire status: {token_expiration_status}')
         return token_expiration_status
 
-    @backoff.on_exception(backoff.expo,
-                          RetryLater,
-                          max_time=5,
-                          max_tries=10,
-                          jitter=None)
+    @backoff.on_exception(backoff.expo, RetryLater, max_time=10, max_tries=20)
     async def request(
         self,
         url: str,
         data: Optional[Union[Dict[str, Dict[str, str]], Dict[str, str]]] = None,
         form_data: Optional[FormData] = None,
         query: Optional[Dict[str, str]] = None,
         request_type: RequestType = RequestType.GET,
@@ -517,14 +513,18 @@
 
             logger.debug('Check if response has empty body')
             response_text = await response.text()
             if response_text == '':
                 logger.debug('Response has empty body. ' \
                     'Returning response status')
                 return response.status
+            elif response_text == 'null':
+                logger.debug('Response is "null". Returning None')
+                return None
+
 
             logger.debug('Response is not empty. ' \
                 'Trying to extract JSON from response')
             try:
                 json_response = await response.json()
             except ContentTypeError:
                 # Special case for such method, like
@@ -565,15 +565,15 @@
         return await asyncio.gather(*requests, return_exceptions=False)
 
     async def _refresh_and_save_tokens(self):
         """Refreshes current access token and saves it to the store.
 
         Due to some problems when trying to refresh with
         Authorization header, this method sets the header to None
-        before refreshing and then sets it back to the new token.
+        before refreshing and then sets it back to the new token
         """
         if self._config is None:
             return None
 
         self.authorization_header = None
 
         token_data = await self.refresh_access_token(
```

### Comparing `shikithon-2.4.2/shikithon/decorators/exceptions_handler.py` & `shikithon-2.5/shikithon/decorators/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.2/shikithon/decorators/method_endpoint.py` & `shikithon-2.5/shikithon/decorators/method_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :return: Decorated function
         :rtype: Callable[P, Awaitable[R]]
         """
 
         @wraps(function)
         async def endpoint_logger_wrapped(*args: P.args,
                                           **kwargs: P.kwargs) -> R:
-            """Decorator's wrapped function for logging endpoint of method
+            """Decorator's wrapped function for logging endpoint of method.
 
             :param args: Positional arguments
             :type args: P.args
 
             :param kwargs: Keyword arguments
             :type kwargs: P.kwargs
```

### Comparing `shikithon-2.4.2/shikithon/endpoints.py` & `shikithon-2.5/shikithon/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Shikimori API Endpoints.
 
 This module contains Endpoints class, which
 contains all endpoints for API and can form
-customized endpoints via input parameters.
+customized endpoints via input parameters
 """
 from typing import Optional, Union
 
 from .utils import Utils
 
 
 class Endpoints:
     """Contains endpoints for Shikimori API.
 
     This class allows to form customized endpoint depending
-    on input parameters.
+    on input parameters
     """
 
     def __init__(self, base_url: str, base_url_v2: str, oauth_url: str):
         """Initializing URLs for Shikimori's API/OAuth.
 
-        This constructor also has base_url_v2, which is
-        modified base_url that routes to new API methods
+        This constructor also has `base_url_v2`, which is
+        modified `base_url` that routes to new API methods
 
         :param base_url: URL for Shikimori API
         :type base_url: str
 
         :param base_url_v2: URL for Shikimori API (v.2)
         :type base_url_v2: str
 
@@ -33,78 +33,78 @@
         """
         self._base_url = base_url
         self._base_url_v2 = base_url_v2
         self._oauth_url = oauth_url
 
     @property
     def base_url(self) -> str:
-        """Returns base_url
+        """Returns `base_url`.
 
         :return: Link for Shikimori API
         :rtype: str
         """
         return self._base_url
 
     @base_url.setter
     def base_url(self, base_url: str):
-        """Sets base_url
+        """Sets `base_url`.
 
         :param base_url: Link for Shikimori API
         :type base_url: str
         """
         self._base_url = base_url
 
     @property
     def base_url_v2(self) -> str:
-        """Returns base_url_v2
+        """Returns `base_url_v2`.
 
         :return: Link for Shikimori API (v.2)
         :rtype: str
         """
         return self._base_url_v2
 
     @base_url_v2.setter
     def base_url_v2(self, base_url_v2: str):
-        """Sets base_url_v2
+        """Sets `base_url_v2`.
 
         :param base_url_v2: Link for Shikimori API (v.2)
         :type base_url_v2: str
         """
         self._base_url_v2 = base_url_v2
 
     @property
     def oauth_url(self) -> str:
-        """Returns oauth_url
+        """Returns `oauth_url`.
 
         :return: Link for Shikimori OAuth
         :rtype: str
         """
         return self._oauth_url
 
     @oauth_url.setter
     def oauth_url(self, oauth_url: str):
-        """Sets oauth_url
+        """Sets `oauth_url`.
 
         :param oauth_url: Link for Shikimori OAuth
         :type oauth_url: str
         """
         self._oauth_url = oauth_url
 
     @property
     def oauth_token(self) -> str:
-        """Returns endpoint for OAuth token
+        """Returns endpoint for OAuth token.
 
         :return: Link for Shikimori OAuth token endpoint
         :rtype: str
         """
         return f'{self.oauth_url}/token'
 
     @property
     def oauth_authorize(self) -> str:
-        """Returns endpoint for OAuth authorization
+        """Returns endpoint for OAuth authorization.
 
         :return: Link for Shikimori OAuth authorization endpoint
         :rtype: str
         """
         return f'{self.oauth_url}/authorize'
 
     def authorization_link(self, client_id: str, redirect_uri: str,
@@ -162,17 +162,14 @@
         """
         return f'{self.abuse_requests}/review'
 
     @property
     def abuse_violation(self) -> str:
         """Returns endpoint for creating request about violation of site rules.
 
-        In Shikimori API docs, this endpoint also named as
-        '/api/v2/abuse_requests/**abuse**'
-
         :return: Abuse violation endpoint link
         :rtype: str
         """
         return f'{self.abuse_requests}/abuse'
 
     @property
     def abuse_spoiler(self) -> str:
@@ -424,14 +421,36 @@
         :type club_id: int
 
         :return: Club characters endpoint link
         :rtype: str
         """
         return f'{self.club(club_id)}/characters'
 
+    def club_collections(self, club_id: int) -> str:
+        """Returns endpoint of a list of collections of a certain club.
+
+        :param club_id: Club ID for endpoint
+        :type club_id: int
+
+        :return: Club collections endpoint link
+        :rtype: str
+        """
+        return f'{self.club(club_id)}/collections'
+
+    def club_clubs(self, club_id: int) -> str:
+        """Returns endpoint of a list of clubs of a certain club.
+
+        :param club_id: Club ID for endpoint
+        :type club_id: int
+
+        :return: Club clubs endpoint link
+        :rtype: str
+        """
+        return f'{self.club(club_id)}/clubs'
+
     def club_members(self, club_id: int) -> str:
         """Returns endpoint of a list of members of a certain club.
 
         :param club_id: Club ID for endpoint
         :type club_id: int
 
         :return: Club members endpoint link
@@ -577,36 +596,36 @@
         :rtype: str
         """
         return f'{self.base_url_v2}/episode_notifications'
 
     def favorites_create(self, linked_type: str, linked_id: int,
                          kind: Optional[str]) -> str:
         """Returns endpoint for creating some type
-        of object as favorite
+        of object as favorite.
 
         :param linked_type: Type of object
         :type linked_type: str
 
         :param linked_id: ID of linked object
         :type linked_id: int
 
         :param kind: Kind of linked object
-            (Required when linked_type is 'Person')
+        (Required when linked_type is `Person`)
         :type kind: Optional[str]
 
         :return: Favorite create endpoint link
         :rtype: str
         """
         return f'{self.base_url}/favorites/' \
                f'{linked_type}/{linked_id}' \
                f'{"" if not kind else f"/{kind}"}'
 
     def favorites_destroy(self, linked_type: str, linked_id: int) -> str:
         """Returns endpoint for destroying some type
-        of object from favorites
+        of object from favorites.
 
         :param linked_type: Type of object
         :type linked_type: str
 
         :param linked_id: ID of linked object
         :type linked_id: int
 
@@ -633,15 +652,15 @@
 
         :return: Forums list endpoint link
         :rtype: str
         """
         return f'{self.base_url}/forums'
 
     def friend(self, friend_id: int) -> str:
-        """Returns endpoint for adding/deleting friend
+        """Returns endpoint for adding/deleting friend.
 
         :param friend_id: Friend ID for endpoint
         :type friend_id: int
 
         :return: Friend addition/deletion endpoint link
         :rtype: str
         """
@@ -912,16 +931,36 @@
 
         :return: Ranobe topics endpoint link
         :rtype: str
         """
         return f'{self.ranobe(ranobe_id)}/topics'
 
     @property
+    def reviews(self) -> str:
+        """Returns endpoint of the reviews.
+
+        :return: Reviews endpoint link
+        :rtype: str
+        """
+        return f'{self.base_url}/reviews'
+
+    def review(self, review_id: int) -> str:
+        """Returns endpoint of a specific review.
+
+        :param review_id: Review ID for endpoint
+        :type review_id: int
+
+        :return: Review endpoint link
+        :rtype: str
+        """
+        return f'{self.reviews}/{review_id}'
+
+    @property
     def active_users(self) -> str:
-        """Returns endpoints of a list of users,
+        """Returns endpoint of a list of users,
         having at least 1 completed animes and active during last month.
 
         :return: Active users list endpoint link
         :rtype: str
         """
         return f'{self.base_url}/stats/active_users'
 
@@ -932,30 +971,38 @@
         :return: Studios list endpoint link
         :rtype: str
         """
         return f'{self.base_url}/studios'
 
     @property
     def styles(self) -> str:
-        """Returns endpoint for creating/previewing style.
+        """Returns endpoint of the styles.
 
-        :return: Style create/preview endpoint link
+        This endpoint also used for styles creation
+
+        :return: Style create endpoint link
         :rtype: str
         """
         return f'{self.base_url}/styles'
 
     @property
     def style_preview(self) -> str:
+        """Returns endpoint for previwing style.
+
+        :return: Style preview endpoint link
+        :rtype: str
+        """
         return f'{self.styles}/preview'
 
     def style(self, style_id: int) -> str:
         """Returns endpoint of the style.
 
         :param style_id: Style ID for endpoint
         :type style_id: int
+
         :return: Style endpoint link
         :rtype: str
         """
         return f'{self.styles}/{style_id}'
 
     @property
     def topics(self) -> str:
@@ -1191,41 +1238,41 @@
 
         :return: User rate endpoint link
         :rtype: str
         """
         return f'{self.user_rates}/{user_rate_id}'
 
     def user_rate_increment(self, user_rate_id: int) -> str:
-        """Returns endpoint for incrementing episodes/chapters by 1
+        """Returns endpoint for incrementing episodes/chapters by 1.
 
         :param user_rate_id: User rate ID for increment endpoint
         :type user_rate_id: int
 
         :return: User rate increment endpoint link
         :rtype: str
         """
         return f'{self.user_rate(user_rate_id)}/increment'
 
     def user_rates_cleanup(self, user_rate_type: str) -> str:
         """Returns endpoint for cleanup user rates by type.
 
-        This endpoint is using API v.1
+        This endpoint is used by API v1
 
         :param user_rate_type: Type of an user rate
         :type user_rate_type: str
 
         :return: User rates cleanup endpoint link
         :rtype: str
         """
         return f'{self.base_url}/user_rates/{user_rate_type}/cleanup'
 
     def user_rates_reset(self, user_rate_type: str) -> str:
         """Returns endpoint for resetting user rates by type.
 
-        This endpoint is using API v.1
+        This endpoint is used by API v1
 
         :param user_rate_type: Type of an user rate
         :type user_rate_type: str
 
         :return: User rates reset endpoint link
         :rtype: str
         """
```

### Comparing `shikithon-2.4.2/shikithon/enums/__init__.py` & `shikithon-2.5/shikithon/enums/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 from .manga import (MangaCensorship, MangaKind, MangaList, MangaOrder,
                     MangaStatus)
 from .message import MessageType
 from .person import PersonKind, PersonSearchKind
 from .ranobe import RanobeCensorship, RanobeList, RanobeOrder, RanobeStatus
 from .request import RequestType
 from .response import ResponseCode
+from .review import ReviewOpinion
 from .style import StyleOwner
 from .topic import TopicForumType, TopicLinkedType, TopicType
 from .user_rate import UserRateStatus, UserRateTarget, UserRateType
 from .video import VideoKind
 
 __all__ = [
     'AnimeCensorship', 'AnimeDuration', 'AnimeKind', 'AnimeTopicKind',
     'AnimeList', 'AnimeOrder', 'AnimeRating', 'AnimeStatus', 'CommentPolicy',
     'ImageUploadPolicy', 'JoinPolicy', 'PagePolicy', 'TopicPolicy',
     'CommentableType', 'CommentableCreateType', 'HistoryTargetType',
     'FavoriteLinkedType', 'MangaCensorship', 'MangaKind', 'MangaList',
     'MangaOrder', 'MangaStatus', 'MessageType', 'PersonKind',
     'PersonSearchKind', 'RanobeCensorship', 'RanobeList', 'RanobeOrder',
-    'RanobeStatus', 'RequestType', 'ResponseCode', 'StyleOwner',
-    'TopicForumType', 'TopicLinkedType', 'TopicType', 'UserRateStatus',
-    'UserRateTarget', 'UserRateType', 'VideoKind'
+    'RanobeStatus', 'RequestType', 'ResponseCode', 'ReviewOpinion',
+    'StyleOwner', 'TopicForumType', 'TopicLinkedType', 'TopicType',
+    'UserRateStatus', 'UserRateTarget', 'UserRateType', 'VideoKind'
 ]
```

### Comparing `shikithon-2.4.2/shikithon/enums/anime.py` & `shikithon-2.5/shikithon/enums/anime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""Enums for /api/animes."""
+"""Enums for `/api/animes`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class AnimeOrder(EnhancedEnum):
     """Contains constants related for list ordering query."""
     ID = 'id'
     ID_DESC = 'id_desc'
     RANKED = 'ranked'
     KIND = 'kind'
     POPULARITY = 'popularity'
     NAME = 'name'
     AIRED_ON = 'aired_on'
     EPISODES = 'episodes'
     STATUS = 'status'
+    RANDOM = 'random'
     CREATED_AT = 'created_at'
     CREATED_AT_DESC = 'created_at_desc'
-    RANDOM = 'random'
 
 
 class AnimeKind(EnhancedEnum):
     """Contains constants related for getting certain kind of anime."""
     TV = 'tv'
     NOT_TV = '!tv'
     TV_13 = 'tv_13'
```

### Comparing `shikithon-2.4.2/shikithon/enums/club.py` & `shikithon-2.5/shikithon/enums/club.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/clubs."""
+"""Enums for `/api/clubs`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class JoinPolicy(EnhancedEnum):
     """Contains constants related for join policy setting."""
     FREE = 'free'
     MEMBER_INVITE = 'member_invite'
```

### Comparing `shikithon-2.4.2/shikithon/enums/comment.py` & `shikithon-2.5/shikithon/enums/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/comments."""
+"""Enums for `/api/comments`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class CommentableType(EnhancedEnum):
     """Contains constants related for commentable type
     of fetched comment."""
     TOPIC = 'Topic'
```

### Comparing `shikithon-2.4.2/shikithon/enums/manga.py` & `shikithon-2.5/shikithon/enums/manga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/mangas."""
+"""Enums for `/api/mangas`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class MangaOrder(EnhancedEnum):
     """Contains constants related for list ordering query."""
     ID = 'id'
     ID_DESC = 'id_desc'
```

### Comparing `shikithon-2.4.2/shikithon/enums/ranobe.py` & `shikithon-2.5/shikithon/enums/ranobe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/ranobe."""
+"""Enums for `/api/ranobe`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class RanobeOrder(EnhancedEnum):
     """Contains constants related for list ordering query."""
     ID = 'id'
     ID_DESC = 'id_desc'
```

### Comparing `shikithon-2.4.2/shikithon/enums/topic.py` & `shikithon-2.5/shikithon/enums/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/topics."""
+"""Enums for `/api/topics`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class TopicType(EnhancedEnum):
     """Contains constants related for getting certain type of topic."""
     REGULAR_TOPIC = 'Topic'
     CLUB_USER_TOPIC = 'Topics::ClubUserTopic'
```

### Comparing `shikithon-2.4.2/shikithon/enums/user_rate.py` & `shikithon-2.5/shikithon/enums/user_rate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Enums for /api/user_rates."""
+"""Enums for `/api/user_rates` and `/api/v2/user_rates`."""
 from .enhanced_enum import EnhancedEnum
 
 
 class UserRateType(EnhancedEnum):
     """Contains constants related for getting certain type of user rate."""
     ANIME = 'anime'
     MANGA = 'manga'
```

### Comparing `shikithon-2.4.2/shikithon/exceptions/__init__.py` & `shikithon-2.5/shikithon/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.2/shikithon/exceptions/missing_app_variable.py` & `shikithon-2.5/shikithon/exceptions/missing_app_variable.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.4.2/shikithon/models/__init__.py` & `shikithon-2.5/shikithon/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """Models for the Shikimori API."""
 
 from .abuse_response import AbuseResponse
 from .achievement import Achievement
-from .anime import Anime
+from .anime import AnimeInfo, Anime, CharacterAnime
 from .ban import Ban
 from .calendar_event import CalendarEvent
-from .character import Character
-from .club import Club
+from .character import CharacterInfo, Character
+from .club import ClubInfo, Club
 from .club_image import ClubImage
-from .comment import Comment
+from .comment import CommentInfo, Comment
 from .constants import (AnimeConstants, ClubConstants, MangaConstants,
-                        SmileyConstants, UserRateConstants)
+                        SmileyConstant, UserRateConstants)
 from .created_user_image import CreatedUserImage
+from .critique import Critique
 from .dialog import Dialog
 from .favourites import Favourites
 from .forum import Forum
 from .franchise_tree import FranchiseTree
 from .genre import Genre
 from .history import History
 from .link import Link
-from .manga import Manga
-from .message import Message
-from .person import Person
+from .manga import MangaInfo, Manga, CharacterManga
+from .message import MessageInfo, Message
+from .person import PersonInfo, Person
 from .publisher import Publisher
-from .ranobe import Ranobe
+from .ranobe import RanobeInfo, Ranobe, CharacterRanobe
 from .relation import Relation
+from .review import Review
 from .role import Role
 from .screenshot import Screenshot
 from .studio import Studio
 from .style import Style
-from .topic import Topic
+from .topic import Topic, TopicUpdate
 from .unread_messages import UnreadMessages
-from .user import User
+from .user import UserInfo, UserBrief, User
 from .user_list import UserList
 from .user_rate import UserRate
 from .video import Video
 
 __all__ = [
-    'AbuseResponse', 'Anime', 'Achievement', 'Ban', 'CalendarEvent',
-    'Character', 'Club', 'ClubImage', 'Comment', 'AnimeConstants',
-    'ClubConstants', 'MangaConstants', 'SmileyConstants', 'UserRateConstants',
-    'CreatedUserImage', 'Dialog', 'Favourites', 'Forum', 'FranchiseTree',
-    'Genre', 'History', 'Link', 'Manga', 'Message', 'Person', 'Publisher',
-    'Ranobe', 'Relation', 'Role', 'Screenshot', 'Studio', 'Style', 'Topic',
-    'UnreadMessages', 'User', 'UserList', 'UserRate', 'Video'
+    'AbuseResponse', 'AnimeInfo', 'Anime', 'CharacterAnime', 'Achievement',
+    'Ban', 'CalendarEvent', 'CharacterInfo', 'Character', 'ClubInfo', 'Club',
+    'ClubImage', 'CommentInfo', 'Comment', 'AnimeConstants', 'ClubConstants',
+    'MangaConstants', 'SmileyConstant', 'UserRateConstants', 'CreatedUserImage',
+    'Critique', 'Dialog', 'Favourites', 'Forum', 'FranchiseTree', 'Genre',
+    'History', 'Link', 'MangaInfo', 'Manga', 'CharacterManga', 'MessageInfo',
+    'Message', 'PersonInfo', 'Person', 'Publisher', 'RanobeInfo', 'Ranobe',
+    'CharacterRanobe', 'Relation', 'Review', 'Role', 'Screenshot', 'Studio',
+    'Style', 'Topic', 'TopicUpdate', 'UnreadMessages', 'UserInfo', 'UserBrief',
+    'User', 'UserList', 'UserRate', 'Video'
 ]
```

### Comparing `shikithon-2.4.2/shikithon/models/anime.py` & `shikithon-2.5/shikithon/models/anime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,68 @@
-"""Model for /api/animes"""
-from datetime import datetime
+"""Model for `/api/animes`."""
+from datetime import date, datetime
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from .genre import Genre
 from .image import Image
 from .screenshot import Screenshot
 from .studio import Studio
 from .user_rate import UserRate
 from .user_rate_score import UserRateScore
 from .user_rate_status import UserRateStatus
 from .video import Video
 
 
-class Anime(BaseModel):
-    """Represents an anime entity."""
+class AnimeInfo(BaseModel):
+    """Represents an anime info entity."""
     id: int
     name: str
     russian: str
     image: Image
     url: str
     kind: Optional[str]
     score: float
     status: str
     episodes: int
     episodes_aired: int
-    aired_on: Optional[str]
-    released_on: Optional[str]
-    rating: Optional[str]
-    english: Optional[List[Optional[str]]]
-    japanese: Optional[List[Optional[str]]]
-    synonyms: Optional[List[Optional[str]]]
+    aired_on: Optional[date]
+    released_on: Optional[date]
+
+
+class Anime(AnimeInfo):
+    """Represents an anime entity."""
+    rating: str
+    english: List[Optional[str]]
+    japanese: List[Optional[str]]
+    synonyms: List[str]
     license_name_ru: Optional[str]
-    duration: Optional[int]
+    duration: int
     description: Optional[str]
-    description_html: Optional[str]
+    description_html: str
     description_source: Optional[str]
     franchise: Optional[str]
-    favoured: Optional[bool]
-    anons: Optional[bool]
-    ongoing: Optional[bool]
+    favoured: bool
+    anons: bool
+    ongoing: bool
     thread_id: Optional[int]
     topic_id: Optional[int]
-    myanimelist_id: Optional[int]
-    rates_scores_stats: Optional[List[UserRateScore]]
-    rates_statuses_stats: Optional[List[UserRateStatus]]
-    updated_at: Optional[datetime]
+    myanimelist_id: int
+    rates_scores_stats: List[UserRateScore]
+    rates_statuses_stats: List[UserRateStatus]
+    updated_at: datetime
     next_episode_at: Optional[datetime]
-    fansubbers: Optional[List[str]]
-    fandubbers: Optional[List[str]]
-    licensors: Optional[List[str]]
-    genres: Optional[List[Genre]]
-    studios: Optional[List[Studio]]
-    videos: Optional[List[Video]]
-    screenshots: Optional[List[Screenshot]]
+    fansubbers: List[str]
+    fandubbers: List[str]
+    licensors: List[str]
+    genres: List[Genre]
+    studios: List[Studio]
+    videos: List[Video]
+    screenshots: List[Screenshot]
     user_rate: Optional[UserRate]
-    roles: Optional[List[str]]
-    role: Optional[str]
+
+
+class CharacterAnime(AnimeInfo):
+    """Represents a character anime info entity."""
+    roles: List[str]
+    role: str
```

### Comparing `shikithon-2.4.2/shikithon/models/character.py` & `shikithon-2.5/shikithon/models/user_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-"""Submodel for creator.py"""
+"""Model for `/api/users/:id/anime_rates|manga_rates`."""
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from pydantic import BaseModel
 
-from .anime import Anime
-from .image import Image
-from .manga import Manga
-from .ranobe import Ranobe
-from .seyu import Seyu
+from .anime import AnimeInfo
+from .manga import MangaInfo
+from .ranobe import RanobeInfo
+from .user import UserInfo
 
 
-class Character(BaseModel):
-    """Represents character entity."""
+class UserList(BaseModel):
+    """Represents user list entity.
+
+    Contains data of watched/read titles.
+    """
     id: int
-    name: str
-    russian: str
-    image: Image
-    url: str
-    altname: Optional[str]
-    japanese: Optional[str]
-    description: Optional[str]
-    description_html: Optional[str]
-    description_source: Optional[str]
-    favoured: Optional[bool]
-    thread_id: Optional[int]
-    topic_id: Optional[int]
-    updated_at: Optional[datetime]
-    seyu: Optional[List[Seyu]]
-    animes: Optional[List[Anime]]
-    mangas: Optional[List[Union[Manga, Ranobe]]]
+    score: int
+    status: str
+    text: Optional[str]
+    episodes: Optional[int]
+    chapters: Optional[int]
+    volumes: Optional[int]
+    text_html: str
+    rewatches: int
+    created_at: datetime
+    updated_at: datetime
+    user: UserInfo
+    anime: Optional[AnimeInfo]
+    manga: Optional[Union[MangaInfo, RanobeInfo]]
```

### Comparing `shikithon-2.4.2/shikithon/models/club.py` & `shikithon-2.5/shikithon/models/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-"""Model for /api/clubs"""
+"""Model for `/api/users`"""
+from datetime import datetime
 from typing import List, Optional
 
 from pydantic import BaseModel
 
-from .anime import Anime
-from .character import Character
-from .club_image import ClubImage
-from .logo import Logo
-from .manga import Manga
-from .user import User
+from .stats import Stats
+from .user_image import UserImage
 
 
-class Club(BaseModel):
-    """Represents a club entity."""
+class UserInfo(BaseModel):
+    """Represents user basic info entity."""
     id: int
-    name: str
-    logo: Logo
-    is_censored: bool
-    join_policy: str
-    comment_policy: str
-    description: Optional[str]
-    description_html: Optional[str]
-    mangas: Optional[List[Manga]]
-    characters: Optional[List[Character]]
-    thread_id: Optional[int]
-    topic_id: Optional[int]
-    user_role: Optional[str]
-    style_id: Optional[int]
-    members: Optional[List[User]]
-    animes: Optional[List[Anime]]
-    images: Optional[List[ClubImage]]
+    nickname: str
+    avatar: str
+    image: UserImage
+    last_online_at: datetime
+    url: str
+
+
+class UserBrief(UserInfo):
+    """Represents user brief info entity."""
+    name: Optional[str]
+    sex: Optional[str]
+    full_years: Optional[int]
+    locale: Optional[str]
+
+
+class User(UserBrief):
+    """Represents user full info entity."""
+    last_online: str
+    website: str
+    birth_on: Optional[datetime]
+    location: Optional[str]
+    banned: bool
+    about: str
+    about_html: str
+    common_info: List[str]
+    show_comments: bool
+    in_friends: Optional[bool]
+    is_ignored: bool
+    stats: Stats
+    style_id: int
```

### Comparing `shikithon-2.4.2/shikithon/models/ranobe.py` & `shikithon-2.5/shikithon/models/manga.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,74 @@
-"""Model for /api/ranobe"""
+"""Model for `/api/mangas`."""
+from datetime import date
 from typing import List, Optional
 
 from pydantic import BaseModel, validator
 
 from .genre import Genre
 from .image import Image
 from .publisher import Publisher
 from .user_rate import UserRate
 from .user_rate_score import UserRateScore
 from .user_rate_status import UserRateStatus
 
+MANGAS_KIND = (
+    'manga',
+    'manhwa',
+    'manhua',
+    'one_shot',
+    'doujin',
+)
 
-class Ranobe(BaseModel):
-    """Represents ranobe entity."""
+
+class MangaInfo(BaseModel):
+    """Represents manga info entity."""
     id: int
     name: str
     russian: str
     image: Image
     url: str
     kind: str
     score: float
     status: str
     volumes: int
     chapters: int
-    aired_on: Optional[str]
-    released_on: Optional[str]
-    english: Optional[List[Optional[str]]]
-    japanese: Optional[List[Optional[str]]]
-    synonyms: Optional[List[Optional[str]]]
+    aired_on: Optional[date]
+    released_on: Optional[date]
+
+    # pylint: disable=E0213
+    @validator('kind')
+    def kind_validator(cls, v):
+        if v not in MANGAS_KIND:
+            raise ValueError(f'Invalid manga kind. Got "{v}"'
+                             f' but expected one of {MANGAS_KIND}')
+        return v
+
+
+class Manga(MangaInfo):
+    """Represents manga entity."""
+    english: List[Optional[str]]
+    japanese: List[Optional[str]]
+    synonyms: List[str]
     license_name_ru: Optional[str]
     description: Optional[str]
-    description_html: Optional[str]
+    description_html: str
     description_source: Optional[str]
     franchise: Optional[str]
-    favoured: Optional[bool]
-    anons: Optional[bool]
-    ongoing: Optional[bool]
+    favoured: bool
+    anons: bool
+    ongoing: bool
     thread_id: Optional[int]
     topic_id: Optional[int]
-    myanimelist_id: Optional[int]
-    rates_scores_stats: Optional[List[UserRateScore]]
-    rates_statuses_stats: Optional[List[UserRateStatus]]
-    licensors: Optional[List[str]]
-    genres: Optional[List[Genre]]
-    publishers: Optional[List[Publisher]]
+    myanimelist_id: int
+    rates_scores_stats: List[UserRateScore]
+    rates_statuses_stats: List[UserRateStatus]
+    licensors: List[str]
+    genres: List[Genre]
+    publishers: List[Publisher]
     user_rate: Optional[UserRate]
 
-    # pylint: disable=E0213
-    @validator('kind')
-    def kind_validator(cls, v):
-        if 'novel' not in v:
-            raise ValueError(f'Invalid kind. Got {v}'
-                             f' but expected kind, containing "novel"')
-        return v
+
+class CharacterManga(MangaInfo):
+    """Represents a character manga info entity."""
+    roles: List[str]
+    role: str
```

### Comparing `shikithon-2.4.2/shikithon/models/stats.py` & `shikithon-2.5/shikithon/models/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Submodel for user.py"""
+"""Submodel for `user.py`."""
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field
 
 from .activity import Activity
 from .genre import Genre
 from .publisher import Publisher
```

### Comparing `shikithon-2.4.2/shikithon/models/topic.py` & `shikithon-2.5/shikithon/models/linked_topic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-"""Model for /api/animes/:id/topics"""
-from datetime import datetime
-from typing import Optional, Union
+"""Submodel for `message.py`."""
+from datetime import date
+from typing import Optional
 
 from pydantic import BaseModel
 
-from .anime import Anime
-from .club import Club
-from .forum import Forum
-from .manga import Manga
-from .user import User
+from .image import Image
 
 
-class Topic(BaseModel):
-    """Represents topic entity."""
+class LinkedTopic(BaseModel):
+    """Represents linked topic of message entity."""
     id: int
-    topic_title: Optional[str]
-    body: Optional[str]
-    html_body: Optional[str]
-    html_footer: Optional[str]
-    created_at: datetime
-    comments_count: Optional[int]
-    forum: Optional[Forum]
-    user: Optional[User]
-    type: Optional[str]
-    linked_id: Optional[int]
-    linked_type: Optional[str]
-    linked: Optional[Union[Club, Anime, Manga]]
-    viewed: Optional[bool]
-    last_comment_viewed: Optional[bool]
-    event: Optional[str]
-    episode: Optional[int]
+    topic_url: str
+    thread_id: int
+    topic_id: int
+    type: str
+    name: Optional[str]
+    russian: Optional[str]
+    image: Optional[Image]
+    url: Optional[str]
+    kind: Optional[str]
+    score: Optional[float]
+    status: Optional[str]
+    episodes: Optional[int]
+    episodes_aired: Optional[int]
+    aired_on: Optional[date]
+    released_on: Optional[date]
```

### Comparing `shikithon-2.4.2/shikithon/models/user_list.py` & `shikithon-2.5/shikithon/models/critique.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Model for /api/users/:id/anime_rates | manga_rates"""
+"""Submodel for `topic.py`."""
 from datetime import datetime
 from typing import Optional, Union
 
 from pydantic import BaseModel
 
-from .anime import Anime
-from .manga import Manga
-from .ranobe import Ranobe
-from .user import User
+from .anime import AnimeInfo
+from .manga import MangaInfo
+from .ranobe import RanobeInfo
+from .user import UserInfo
 
 
-class UserList(BaseModel):
-    """Represents user list entity.
+class Critique(BaseModel):
+    """Represents critique entity.
 
-    Contains data of watched/read titles.
+    Can be found in topics with type
+    `Topics::EntryTopics::CritiqueTopic`
     """
     id: int
-    score: int
-    status: str
-    text: Optional[str]
-    episodes: Optional[int]
-    chapters: Optional[int]
-    volumes: Optional[int]
-    text_html: str
-    rewatches: int
+    target: Optional[Union[AnimeInfo, MangaInfo, RanobeInfo]]
+    user: UserInfo
+    votes_count: int
+    votes_for: int
+    body: str
+    html_body: str
+    overall: Optional[int]
+    storyline: Optional[int]
+    music: Optional[int]
+    characters: Optional[int]
+    animation: Optional[int]
     created_at: datetime
-    updated_at: datetime
-    user: Optional[User]
-    anime: Optional[Anime]
-    manga: Optional[Union[Manga, Ranobe]]
```

### Comparing `shikithon-2.4.2/shikithon/models/user_rate.py` & `shikithon-2.5/shikithon/models/user_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Model for /api/user_rates and /api/v2/user_rates"""
+"""Model for `/api/user_rates` and `/api/v2/user_rates`."""
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 class UserRate(BaseModel):
```

### Comparing `shikithon-2.4.2/shikithon/resources/__init__.py` & `shikithon-2.5/shikithon/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .friends import Friends
 from .genres import Genres
 from .mangas import Mangas
 from .messages import Messages
 from .people import People
 from .publishers import Publishers
 from .ranobes import Ranobes
+from .reviews import Reviews
 from .stats import Stats
 from .studios import Studios
 from .styles import Styles
 from .topics import Topics
 from .user_images import UserImages
 from .user_rates import UserRates
 from .users import Users
@@ -44,14 +45,15 @@
     'Friends',
     'Genres',
     'Mangas',
     'Messages',
     'People',
     'Publishers',
     'Ranobes',
+    'Reviews',
     'Stats',
     'Studios',
     'Styles',
     'Topics',
     'UserImages',
     'UserRates',
     'Users',
```

### Comparing `shikithon-2.4.2/shikithon/resources/abuse_requests.py` & `shikithon-2.5/shikithon/resources/abuse_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/v2/abuse_requests resource."""
+"""Represents `/api/v2/abuse_requests` resource."""
 from typing import Any, Dict, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType, ResponseCode
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import AbuseResponse
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class AbuseRequests(BaseResource):
     """AbuseRequests resource class.
 
-    Used to represent /api/v2/abuse_requests resource.
+    Used to represent `/api/v2/abuse_requests` resource
     """
 
     @method_endpoint('/api/v2/abuse_requests/offtopic')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def offtopic(self, comment_id: int):
         """Marks comment as offtopic.
```

### Comparing `shikithon-2.4.2/shikithon/resources/achievements.py` & `shikithon-2.5/shikithon/resources/achievements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/achievements resource."""
+"""Represents `/api/achievements` resource."""
 
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Achievement
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Achievements(BaseResource):
     """Achievements resource class.
 
-    Used to represent /api/achievements resource.
+    Used to represent `/api/achievements` resource
     """
 
     @method_endpoint('/api/achievements')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self, user_id: int):
         """Returns list of user achievements.
```

### Comparing `shikithon-2.4.2/shikithon/resources/animes.py` & `shikithon-2.5/shikithon/resources/animes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Represents /api/animes and /api/animes/:anime_id/videos resource."""
+"""Represents `/api/animes` and `/api/animes/:anime_id/videos` resources."""
 from typing import Any, Dict, List, Optional, Union, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import (AnimeCensorship, AnimeDuration, AnimeKind, AnimeList,
                      AnimeOrder, AnimeRating, AnimeStatus, AnimeTopicKind,
                      RequestType, ResponseCode, VideoKind)
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import (Anime, FranchiseTree, Link, Relation, Role, Screenshot,
-                      Topic, Video)
+from ..models import (AnimeInfo, Anime, FranchiseTree, Link, Relation, Role,
+                      Screenshot, Topic, Video)
 from ..utils import Utils
 from .base_resource import BaseResource
 
-VIDEO_DICT_NAME = 'video'
+DICT_NAME = 'video'
 
 
 class Animes(BaseResource):
     """Anime resource class.
 
-    Used to represent /api/animes and
-    /api/animes/:anime_id/videos resource.
+    Used to represent `/api/animes` and
+    `/api/animes/:anime_id/videos` resources
     """
 
     @method_endpoint('/api/animes')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None,
@@ -36,16 +36,16 @@
                                                List[AnimeDuration]]] = None,
                       rating: Optional[Union[AnimeRating,
                                              List[AnimeRating]]] = None,
                       genre: Optional[Union[int, List[int]]] = None,
                       studio: Optional[Union[int, List[int]]] = None,
                       franchise: Optional[Union[int, List[int]]] = None,
                       censored: Optional[AnimeCensorship] = None,
-                      my_list: Optional[Union[AnimeList,
-                                              List[AnimeList]]] = None,
+                      mylist: Optional[Union[AnimeList,
+                                             List[AnimeList]]] = None,
                       ids: Optional[Union[int, List[int]]] = None,
                       exclude_ids: Optional[Union[int, List[int]]] = None,
                       search: Optional[str] = None):
         """Returns list of anime.
 
         :param page: Number of page
         :type page: Optional[int]
@@ -82,55 +82,55 @@
 
         :param franchise: Franchise(s) ID
         :type franchise: Optional[Union[int, List[int]]]
 
         :param censored: Type of anime censorship
         :type censored: Optional[AnimeCensorship]
 
-        :param my_list: Status(-es) of anime in current user list.
+        :param mylist: Status(-es) of anime in current user list.
             If app is in restricted mode,
             this parameter won't affect on response.
-        :type my_list: Optional[Union[AnimeList, List[AnimeList]]]
+        :type mylist: Optional[Union[AnimeList, List[AnimeList]]]
 
         :param ids: Anime(s) ID to include
         :type ids: Optional[Union[int, List[int]]]
 
         :param exclude_ids: Anime(s) ID to exclude
         :type exclude_ids: Optional[Union[int, List[int]]]
 
         :param search: Search phrase to filter animes by name
         :type search: Optional[str]
 
         :return: List of anime
-        :rtype: List[Anime]
+        :rtype: List[AnimeInfo]
         """
         query_dict = Utils.create_query_dict(page=page,
                                              limit=limit,
                                              order=order,
                                              kind=kind,
                                              status=status,
                                              season=season,
                                              score=score,
                                              duration=duration,
                                              rating=rating,
                                              genre=genre,
                                              studio=studio,
                                              franchise=franchise,
                                              censored=censored,
-                                             mylist=my_list,
+                                             mylist=mylist,
                                              ids=ids,
                                              exclude_ids=exclude_ids,
                                              search=search)
 
         response = await self._client.request(self._client.endpoints.animes,
                                               query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Anime)
+                                            data_model=AnimeInfo)
 
     @method_endpoint('/api/animes/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, anime_id: int):
         """Returns info about certain anime.
 
         :param anime_id: Anime ID to get info
@@ -168,22 +168,22 @@
     async def similar(self, anime_id: int):
         """Returns list of similar animes for certain anime.
 
         :param anime_id: Anime ID to get similar animes
         :type anime_id: int
 
         :return: List of similar animes
-        :rtype: List[Anime]
+        :rtype: List[AnimeInfo]
         """
         response = await self._client.request(
             self._client.endpoints.similar_animes(anime_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Anime)
+                                            data_model=AnimeInfo)
 
     @method_endpoint('/api/animes/:id/related')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def related(self, anime_id: int):
         """Returns list of relations of certain anime.
 
         :param anime_id: Anime ID to get relations
@@ -327,15 +327,15 @@
 
         :param url: URL of video
         :type url: str
 
         :return: Created video info
         :rtype: Optional[Video]
         """
-        data_dict = Utils.create_data_dict(dict_name=VIDEO_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            kind=kind,
                                            name=name,
                                            url=url)
 
         response = await self._client.request(
             self._client.endpoints.anime_videos(anime_id),
             data=data_dict,
```

### Comparing `shikithon-2.4.2/shikithon/resources/appears.py` & `shikithon-2.5/shikithon/resources/appears.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/appears resource."""
+"""Represents `/api/appears` resource."""
 from typing import cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType, ResponseCode
 from ..exceptions import ShikimoriAPIResponseError
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Appears(BaseResource):
     """Appears resource class.
 
-    Used to represent /api/appears resource.
+    Used to represent `/api/appears` resource
     """
 
     @method_endpoint('/api/appears')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=False)
     async def mark(self, *ids: str):
         """Marks comments or topics as read.
```

### Comparing `shikithon-2.4.2/shikithon/resources/bans.py` & `shikithon-2.5/shikithon/resources/bans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/bans resource."""
+"""Represents `/api/bans` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Ban
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Bans(BaseResource):
     """Bans resource class.
 
-    Used to represent /api/bans resource.
+    Used to represent `/api/bans` resource
     """
 
     @method_endpoint('/api/bans')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None):
```

### Comparing `shikithon-2.4.2/shikithon/resources/calendars.py` & `shikithon-2.5/shikithon/resources/calendars.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/calendar resource."""
+"""Represents `/api/calendar` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import AnimeCensorship
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import CalendarEvent
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Calendars(BaseResource):
     """Calendars resource class.
 
-    Used to represent /api/calendar resource.
+    Used to represent `/api/calendar` resource
     """
 
     @method_endpoint('/api/calendar')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self, censored: Optional[AnimeCensorship] = None):
         """Returns current calendar events.
```

### Comparing `shikithon-2.4.2/shikithon/resources/characters.py` & `shikithon-2.5/shikithon/resources/characters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/characters resource."""
+"""Represents `/api/characters` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Character
+from ..models import CharacterInfo, Character
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Characters(BaseResource):
     """Characters resource class.
 
-    Used to represent /api/characters resource.
+    Used to represent `/api/characters` resource
     """
 
     @method_endpoint('/api/characters/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, character_id: int):
         """Returns character info by ID.
 
@@ -36,17 +36,17 @@
     async def search(self, search: Optional[str] = None):
         """Returns list of found characters.
 
         :param search: Search query for characters
         :type search: Optional[str]
 
         :return: List of found characters
-        :rtype: List[Character]
+        :rtype: List[CharacterInfo]
         """
         query_dict = Utils.create_query_dict(search=search)
 
         response = await self._client.request(
             self._client.endpoints.character_search, query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Character)
+                                            data_model=CharacterInfo)
```

### Comparing `shikithon-2.4.2/shikithon/resources/clubs.py` & `shikithon-2.5/shikithon/resources/clubs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""Represents /api/clubs resource."""
+"""Represents `/api/clubs` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import (CommentPolicy, ImageUploadPolicy, JoinPolicy, PagePolicy,
                      RequestType, ResponseCode, TopicPolicy)
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Anime, Character, Club, ClubImage, Manga, Ranobe, User
+from ..models import AnimeInfo, CharacterInfo, ClubInfo, Club, ClubImage, MangaInfo, RanobeInfo, UserInfo, Topic
 from ..utils import Utils
 from .base_resource import BaseResource
 
 DICT_NAME = 'club'
 
 
 class Clubs(BaseResource):
     """Clubs resource class.
 
-    Used to represent /api/clubs resource.
+    Used to represent `/api/clubs` resource
     """
 
     @method_endpoint('/api/clubs')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None,
@@ -32,26 +32,26 @@
         :param limit: Number of results limit
         :type limit: Optional[int]
 
         :param search: Search phrase to filter clubs by name
         :type search: Optional[str]
 
         :return: Clubs list
-        :rtype: List[Club]
+        :rtype: List[ClubInfo]
         """
         query_dict = Utils.create_query_dict(page=page,
                                              limit=limit,
                                              search=search)
 
         response = await self._client.request(self._client.endpoints.clubs,
                                               query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Club)
+                                            data_model=ClubInfo)
 
     @method_endpoint('/api/clubs/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, club_id: int):
         """Returns info about club.
 
         :param club_id: Club ID to get info
@@ -191,94 +191,130 @@
     async def animes(self, club_id: int):
         """Returns anime list of club.
 
         :param club_id: Club ID to get anime list
         :type club_id: int
 
         :return: Club's anime list
-        :rtype: List[Anime]
+        :rtype: List[AnimeInfo]
         """
         response = await self._client.request(
             self._client.endpoints.club_animes(club_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Anime)
+                                            data_model=AnimeInfo)
 
     @method_endpoint('/api/clubs/:id/mangas')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def mangas(self, club_id: int):
         """Returns manga list of club.
 
         :param club_id: Club ID to get manga list
         :type club_id: int
 
         :return: Club's manga list
-        :rtype: List[Manga]
+        :rtype: List[MangaInfo]
         """
         response = await self._client.request(
             self._client.endpoints.club_mangas(club_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Manga)
+                                            data_model=MangaInfo)
 
     @method_endpoint('/api/clubs/:id/ranobe')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def ranobe(self, club_id: int):
         """Returns ranobe list of club.
 
         :param club_id: Club ID to get ranobe list
         :type club_id: int
 
         :return: Club's ranobe list
-        :rtype: List[Ranobe]
+        :rtype: List[RanobeInfo]
         """
         response = await self._client.request(
             self._client.endpoints.club_ranobe(club_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Ranobe)
+                                            data_model=RanobeInfo)
 
     @method_endpoint('/api/clubs/:id/characters')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def characters(self, club_id: int):
         """Returns character list of club.
 
         :param club_id: Club ID to get character list
         :type club_id: int
 
         :return: Club's character list
-        :rtype: List[Character]
+        :rtype: List[CharacterInfo]
         """
         response = await self._client.request(
             self._client.endpoints.club_characters(club_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Character)
+                                            data_model=CharacterInfo)
+
+    @method_endpoint('/api/clubs/:id/collections')
+    @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
+    async def collections(self, club_id: int):
+        """Returns collection list of club.
+
+        :param club_id: Club ID to get collection list
+        :type club_id: int
+
+        :return: Club's collection list
+        :rtype: List[Topic]
+        """
+        response = await self._client.request(
+            self._client.endpoints.club_collections(club_id))
+
+        return Utils.validate_response_data(cast(List[Dict[str, Any]],
+                                                 response),
+                                            data_model=Topic)
+
+    @method_endpoint('/api/clubs/:id/clubs')
+    @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
+    async def clubs(self, club_id: int):
+        """Returns clubs info list of club.
+
+        :param club_id: Club ID to get clubs info list
+        :type club_id: int
+
+        :return: Club's clubs info list
+        :rtype: List[ClubInfo]
+        """
+        response = await self._client.request(
+            self._client.endpoints.club_clubs(club_id))
+
+        return Utils.validate_response_data(cast(List[Dict[str, Any]],
+                                                 response),
+                                            data_model=ClubInfo)
 
     @method_endpoint('/api/clubs/:id/members')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def members(self, club_id: int):
         """Returns member list of club.
 
         :param club_id: Club ID to get member list
         :type club_id: int
 
         :return: Club's member list
-        :rtype: List[User]
+        :rtype: List[UserInfo]
         """
         response = await self._client.request(
             self._client.endpoints.club_members(club_id))
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=User)
+                                            data_model=UserInfo)
 
     @method_endpoint('/api/clubs/:id/images')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def images(self, club_id: int):
         """Returns images of club.
 
         :param club_id: Club ID to get images
```

### Comparing `shikithon-2.4.2/shikithon/resources/comments.py` & `shikithon-2.5/shikithon/resources/comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Represents /api/comments resource."""
+"""Represents `/api/comments` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from loguru import logger
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import CommentableCreateType, CommentableType, RequestType
 from ..exceptions import ShikimoriAPIResponseError
@@ -12,15 +12,15 @@
 
 DICT_NAME = 'comment'
 
 
 class Comments(BaseResource):
     """Comments resource class.
 
-    Used to represent /api/comments resource.
+    Used to represent `/api/comments` resource
     """
 
     @method_endpoint('/api/comments')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       commentable_id: int,
                       commentable_type: CommentableType,
@@ -84,15 +84,15 @@
                      commentable_id: int,
                      commentable_type: CommentableCreateType,
                      is_offtopic: Optional[bool] = None,
                      broadcast: Optional[bool] = None) -> Optional[Comment]:
         """Creates comment.
 
         When commentable_type set to other than Topic/User,
-        comment is attached to commentable main topic.
+        comment is attached to commentable main topic
 
         :param body: Body of comment
         :type body: str
 
         :param commentable_id: ID of entity to comment on
         :type commentable_id: int
```

### Comparing `shikithon-2.4.2/shikithon/resources/constants.py` & `shikithon-2.5/shikithon/resources/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/constants resource."""
+"""Represents `/api/constants` resource."""
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import (AnimeConstants, ClubConstants, MangaConstants,
-                      SmileyConstants, UserRateConstants)
+                      SmileyConstant, UserRateConstants)
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Constants(BaseResource):
     """Constants resource class.
 
-    Used to represent /api/constants resource.
+    Used to represent `/api/constants` resource
     """
 
     @method_endpoint('/api/constants/anime')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def anime(self):
         """Returns anime constants values.
 
@@ -70,18 +70,18 @@
 
         return Utils.validate_response_data(cast(Dict[str, Any], response),
                                             data_model=ClubConstants)
 
     @method_endpoint('/api/constants/smileys')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def smileys(self):
-        """Returns list of smileys constants values.
+        """Returns list of smiley constant values.
 
-        :return: List of smileys constants values
-        :rtype: List[SmileyConstants]
+        :return: List of smiley constant values
+        :rtype: List[SmileyConstant]
         """
         response = await self._client.request(
             self._client.endpoints.smileys_constants)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=SmileyConstants)
+                                            data_model=SmileyConstant)
```

### Comparing `shikithon-2.4.2/shikithon/resources/dialogs.py` & `shikithon-2.5/shikithon/resources/dialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Represents /api/dialogs resource."""
+"""Represents `/api/dialogs` resource."""
 from typing import Any, Dict, List, Union, cast
 
 from loguru import logger
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType
 from ..exceptions import ShikimoriAPIResponseError
@@ -10,15 +10,15 @@
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Dialogs(BaseResource):
     """Dialogs resource class.
 
-    Used to represent /api/dialogs resource.
+    Used to represent `/api/dialogs` resource
     """
 
     @method_endpoint('/api/dialogs')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self):
         """Returns list of current user's dialogs.
```

### Comparing `shikithon-2.4.2/shikithon/resources/favorites.py` & `shikithon-2.5/shikithon/resources/favorites.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/favorites resource."""
+"""Represents `/api/favorites` resource."""
 from typing import Any, Dict, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import FavoriteLinkedType, PersonKind, RequestType, ResponseCode
 from ..exceptions import ShikimoriAPIResponseError
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Favorites(BaseResource):
     """Favorites resource class.
 
-    Used to represent /api/favorites resource.
+    Used to represent `/api/favorites` resource
     """
 
     @method_endpoint('/api/favorites/:linked_type/:linked_id(/:kind)')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=False)
     async def create(self,
                      linked_type: FavoriteLinkedType,
                      linked_id: int,
@@ -70,15 +70,15 @@
 
     @method_endpoint('/api/favorites/:id/reorder')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=False)
     async def reorder(self, favorite_id: int, new_index: Optional[int] = None):
         """Reorders a favorite to the new index.
 
         This method requires a favorite ID,
-        which cannot be retrieved through the current API methods.
+        which cannot be retrieved through the current API methods
 
         To get the favorite ID, use DevTools on the favorites page
         See https://github.com/shikimori/shikimori/issues/2655
 
         :param favorite_id: ID of a favorite to reorder
         :type favorite_id: int
```

### Comparing `shikithon-2.4.2/shikithon/resources/forums.py` & `shikithon-2.5/shikithon/resources/studios.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Represents /api/forums resource."""
+"""Represents `/api/studios` resource."""
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Forum
+from ..models import Studio
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
-class Forums(BaseResource):
-    """Forums resource class.
+class Studios(BaseResource):
+    """Studios resource class.
 
-    Used to represent /api/forums resource.
+    Used to represent `/api/studios` resource
     """
 
-    @method_endpoint('/api/forums')
+    @method_endpoint('/api/studios')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self):
-        """Returns list of forums.
+        """Returns list of studios.
 
-        :returns: List of forums
-        :rtype: List[Forum]
+        :return: List of studios
+        :rtype: List[Studio]
         """
-        response = await self._client.request(self._client.endpoints.forums)
+        response = await self._client.request(self._client.endpoints.studios)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Forum)
+                                            data_model=Studio)
```

### Comparing `shikithon-2.4.2/shikithon/resources/friends.py` & `shikithon-2.5/shikithon/resources/friends.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Represents /api/friends resource."""
+"""Represents `/api/friends` resource."""
 from loguru import logger
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType
 from ..exceptions import ShikimoriAPIResponseError
 from .base_resource import BaseResource
 
 
 class Friends(BaseResource):
     """Friends resource class.
 
-    Used to represent /api/friends resource.
+    Used to represent `/api/friends` resource
     """
 
     @method_endpoint('/api/friends/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=False)
     async def create(self, user_id: int):
         """Creates (adds) new friend by ID.
```

### Comparing `shikithon-2.4.2/shikithon/resources/genres.py` & `shikithon-2.5/shikithon/resources/genres.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/genres resource."""
+"""Represents `/api/genres` resource."""
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Genre
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Genres(BaseResource):
     """Genres resource class.
 
-    Used to represent /api/genres resource.
+    Used to represent `/api/genres` resource
     """
 
     @method_endpoint('/api/genres')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self):
         """Returns list of genres.
```

### Comparing `shikithon-2.4.2/shikithon/resources/mangas.py` & `shikithon-2.5/shikithon/resources/mangas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Represents /api/mangas resource."""
+"""Represents `/api/mangas` resource."""
 from typing import Any, Dict, List, Optional, Union, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import (MangaCensorship, MangaKind, MangaList, MangaOrder,
                      MangaStatus)
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import FranchiseTree, Link, Manga, Relation, Role, Topic
+from ..models import FranchiseTree, Link, Manga, MangaInfo, RanobeInfo, Relation, Role, Topic
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Mangas(BaseResource):
     """Mangas resource class.
 
-    Used to represent /api/mangas resource.
+    Used to represent `/api/mangas` resource
     """
 
     @method_endpoint('/api/mangas')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None,
@@ -27,16 +27,16 @@
                                              List[MangaStatus]]] = None,
                       season: Optional[Union[str, List[str]]] = None,
                       score: Optional[int] = None,
                       genre: Optional[Union[int, List[int]]] = None,
                       publisher: Optional[Union[int, List[int]]] = None,
                       franchise: Optional[Union[int, List[int]]] = None,
                       censored: Optional[MangaCensorship] = None,
-                      my_list: Optional[Union[MangaList,
-                                              List[MangaList]]] = None,
+                      mylist: Optional[Union[MangaList,
+                                             List[MangaList]]] = None,
                       ids: Optional[Union[int, List[int]]] = None,
                       exclude_ids: Optional[Union[int, List[int]]] = None,
                       search: Optional[str] = None):
         """Returns mangas list.
 
         :param page: Number of page
         :type page: Optional[int]
@@ -67,53 +67,53 @@
 
         :param franchise: Franchise(s) ID
         :type franchise: Optional[Union[int, List[int]]
 
         :param censored: Type of manga censorship
         :type censored: Optional[MangaCensorship]
 
-        :param my_list: Status(-es) of manga in current user list.
+        :param mylist: Status(-es) of manga in current user list.
             If app is in restricted mode,
             this parameter won't affect on response.
-        :type my_list: Optional[Union[MangaList, List[MangaList]]]
+        :type mylist: Optional[Union[MangaList, List[MangaList]]]
 
         :param ids: Manga(s) ID to include
         :type ids: Optional[Union[int, List[int]]
 
         :param exclude_ids: Manga(s) ID to exclude
         :type exclude_ids: Optional[Union[int, List[int]]
 
         :param search: Search phrase to filter mangas by name
         :type search: Optional[str]
 
         :return: List of Mangas
-        :rtype: List[Manga]
+        :rtype: List[MangaInfo]
         """
         query_dict = Utils.create_query_dict(page=page,
                                              limit=limit,
                                              order=order,
                                              kind=kind,
                                              status=status,
                                              season=season,
                                              score=score,
                                              genre=genre,
                                              publisher=publisher,
                                              franchise=franchise,
                                              censored=censored,
-                                             mylist=my_list,
+                                             mylist=mylist,
                                              ids=ids,
                                              exclude_ids=exclude_ids,
                                              search=search)
 
         response = await self._client.request(self._client.endpoints.mangas,
                                               query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Manga)
+                                            data_model=MangaInfo)
 
     @method_endpoint('/api/mangas/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, manga_id: int):
         """Returns info about certain manga.
 
         :param manga_id: Manga ID to get info
@@ -145,28 +145,27 @@
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
                                             data_model=Role)
 
     @method_endpoint('/api/mangas/:id/similar')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def similar(self, manga_id: int):
-        """Returns list of similar mangas for certain manga.
+        """Returns list of similar mangas or ranobe for certain manga.
 
-        :param manga_id: Manga ID to get similar mangas
+        :param manga_id: Manga ID to get similar mangas/ranobe
         :type manga_id: int
 
-        :return: List of similar mangas
-        :rtype: List[Manga]
+        :return: List of similar mangas/ranobe
+        :rtype: List[Union[MangaInfo, RanobeInfo]]
         """
         response = await self._client.request(
             self._client.endpoints.similar_mangas(manga_id))
 
-        return Utils.validate_response_data(cast(List[Dict[str, Any]],
-                                                 response),
-                                            data_model=Manga)
+        return Utils.parse_mixed_response(response, List[Union[MangaInfo,
+                                                               RanobeInfo]])
 
     @method_endpoint('/api/mangas/:id/related')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def related(self, manga_id: int):
         """Returns list of related content of certain manga.
 
         :param manga_id: Manga ID to get related content
```

### Comparing `shikithon-2.4.2/shikithon/resources/messages.py` & `shikithon-2.5/shikithon/resources/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Represents /api/messages resource."""
+"""Represents `/api/messages` resource."""
 from typing import Any, Dict, List, Optional, Union, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import MessageType, RequestType, ResponseCode
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Message
 from ..utils import Utils
@@ -11,15 +11,15 @@
 DICT_NAME = 'message'
 PRIVATE_DM = 'Private'
 
 
 class Messages(BaseResource):
     """Messages resource class.
 
-    Used to represent /api/messages resource.
+    Used to represent `/api/messages` resource
     """
 
     @method_endpoint('/api/messages/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, message_id: int):
         """Returns message info.
 
@@ -37,15 +37,15 @@
 
     @method_endpoint('/api/messages')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def create(self, body: str, from_id: int,
                      to_id: int) -> Optional[Message]:
         """Creates message.
 
-        :param body: Body of message
+        :param body: Body of message (Need to have length >= 2)
         :type body: str
 
         :param from_id: Sender ID
         :type from_id: int
 
         :param to_id: Reciver ID
         :type to_id: int
```

### Comparing `shikithon-2.4.2/shikithon/resources/people.py` & `shikithon-2.5/shikithon/resources/people.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/people resource."""
+"""Represents `/api/people` resource."""
 from typing import Any, Dict, List, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import PersonSearchKind
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Person
+from ..models import PersonInfo, Person
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class People(BaseResource):
     """People resource class.
 
-    Used to represent /api/people resource.
+    Used to represent `/api/people` resource
     """
 
     @method_endpoint('/api/people/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, people_id: int):
         """Returns info about a person.
 
@@ -42,17 +42,17 @@
         :param search: Search query for persons
         :type search: Optional[str]
 
         :param people_kind: Kind of person for searching
         :type people_kind: Optional[PersonSearchKind]
 
         :return: List of found persons
-        :rtype: List[Person]
+        :rtype: List[PersonInfo]
         """
         query_dict = Utils.create_query_dict(search=search, kind=people_kind)
 
         response = await self._client.request(
             self._client.endpoints.people_search, query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Person)
+                                            data_model=PersonInfo)
```

### Comparing `shikithon-2.4.2/shikithon/resources/publishers.py` & `shikithon-2.5/shikithon/resources/publishers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Represents /api/publishers resource."""
+"""Represents `/api/publishers` resource."""
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Publisher
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Publishers(BaseResource):
     """Publishers resource class.
 
-    Used to represent /api/publishers resource.
+    Used to represent `/api/publishers` resource
     """
 
     @method_endpoint('/api/publishers')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self):
         """Returns list of publishers.
```

### Comparing `shikithon-2.4.2/shikithon/resources/ranobes.py` & `shikithon-2.5/shikithon/resources/ranobes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/ranobes resource."""
+"""Represents `/api/ranobes` resource."""
 from typing import Any, Dict, List, Optional, Union, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RanobeCensorship, RanobeList, RanobeOrder, RanobeStatus
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import FranchiseTree, Link, Ranobe, Relation, Role, Topic
+from ..models import FranchiseTree, Link, RanobeInfo, MangaInfo, Ranobe, Relation, Role, Topic
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Ranobes(BaseResource):
     """Ranobes resource class.
 
-    Used to represent /api/ranobes resource.
+    Used to represent `/api/ranobes` resource
     """
 
     @method_endpoint('/api/ranobe')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None,
@@ -25,16 +25,16 @@
                                              List[RanobeStatus]]] = None,
                       season: Optional[Union[str, List[str]]] = None,
                       score: Optional[int] = None,
                       genre: Optional[Union[int, List[int]]] = None,
                       publisher: Optional[Union[int, List[int]]] = None,
                       franchise: Optional[Union[int, List[int]]] = None,
                       censored: Optional[RanobeCensorship] = None,
-                      my_list: Optional[Union[RanobeList,
-                                              List[RanobeList]]] = None,
+                      mylist: Optional[Union[RanobeList,
+                                             List[RanobeList]]] = None,
                       ids: Optional[Union[int, List[int]]] = None,
                       exclude_ids: Optional[Union[int, List[int]]] = None,
                       search: Optional[str] = None):
         """Returns ranobe list.
 
         :param page: Number of page
         :type page: Optional[int]
@@ -62,52 +62,52 @@
 
         :param franchise: Franchise(s) ID
         :type franchise: Optional[Union[int, List[int]]
 
         :param censored: Type of ranobe censorship
         :type censored: Optional[RanobeCensorship]
 
-        :param my_list: Status(-es) of ranobe in current user list.
+        :param mylist: Status(-es) of ranobe in current user list.
             If app is in restricted mode,
             this parameter won't affect on response.
-        :type my_list: Optional[Union[RanobeList, List[RanobeList]]]
+        :type mylist: Optional[Union[RanobeList, List[RanobeList]]]
 
         :param ids: Ranobe(s) ID to include
         :type ids: Optional[Union[int, List[int]]
 
         :param exclude_ids: Ranobe(s) ID to exclude
         :type exclude_ids: Optional[Union[int, List[int]]
 
         :param search: Search phrase to filter ranobe by name
         :type search: Optional[str]
 
         :return: List of Ranobe
-        :rtype: List[Ranobe]
+        :rtype: List[RanobeInfo]
         """
         query_dict = Utils.create_query_dict(page=page,
                                              limit=limit,
                                              order=order,
                                              status=status,
                                              season=season,
                                              score=score,
                                              genre=genre,
                                              publisher=publisher,
                                              franchise=franchise,
                                              censored=censored,
-                                             mylist=my_list,
+                                             mylist=mylist,
                                              ids=ids,
                                              exclude_ids=exclude_ids,
                                              search=search)
 
         response = await self._client.request(self._client.endpoints.ranobes,
                                               query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Ranobe)
+                                            data_model=RanobeInfo)
 
     @method_endpoint('/api/ranobe/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, ranobe_id: int):
         """Returns info about certain ranobe.
 
         :param ranobe_id: Ranobe ID to get info
@@ -139,28 +139,27 @@
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
                                             data_model=Role)
 
     @method_endpoint('/api/ranobe/:id/similar')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def similar(self, ranobe_id: int):
-        """Returns list of similar ranobes for certain ranobe.
+        """Returns list of similar mangas or ranobe for certain ranobe.
 
-        :param ranobe_id: Ranobe ID to get similar ranobes
+        :param ranobe_id: Ranobe ID to get similar mangas/ranobe
         :type ranobe_id: int
 
-        :return: List of similar ranobes
-        :rtype: List[Ranobe]
+        :return: List of similar mangas/ranobe
+        :rtype: List[Union[MangaInfo, RanobeInfo]]
         """
         response = await self._client.request(
             self._client.endpoints.similar_ranobes(ranobe_id))
 
-        return Utils.validate_response_data(cast(List[Dict[str, Any]],
-                                                 response),
-                                            data_model=Ranobe)
+        return Utils.parse_mixed_response(response, List[Union[MangaInfo,
+                                                               RanobeInfo]])
 
     @method_endpoint('/api/ranobe/:id/related')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def related(self, ranobe_id: int):
         """Returns list of related content of certain ranobe.
 
         :param ranobe_id: Ranobe ID to get related content
```

### Comparing `shikithon-2.4.2/shikithon/resources/stats.py` & `shikithon-2.5/shikithon/resources/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Represents /api/stats resource."""
+"""Represents `/api/stats` resource."""
 from typing import List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
 from .base_resource import BaseResource
 
 
 class Stats(BaseResource):
     """Stats resource class.
 
-    Used to represent /api/stats resource.
+    Used to represent `/api/stats` resource
     """
 
     @method_endpoint('/api/stats/active_users')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def active_users(self):
         """Returns list of IDs of active users.
```

### Comparing `shikithon-2.4.2/shikithon/resources/studios.py` & `shikithon-2.5/shikithon/resources/forums.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Represents /api/studios resource."""
+"""Represents `/api/forums` resource."""
 from typing import Any, Dict, List, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Studio
+from ..models import Forum
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
-class Studios(BaseResource):
-    """Studios resource class.
+class Forums(BaseResource):
+    """Forums resource class.
 
-    Used to represent /api/studios resource.
+    Used to represent `/api/forums` resource
     """
 
-    @method_endpoint('/api/studios')
+    @method_endpoint('/api/forums')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self):
-        """Returns list of studios.
+        """Returns list of forums.
 
-        :return: List of studios
-        :rtype: List[Studio]
+        :returns: List of forums
+        :rtype: List[Forum]
         """
-        response = await self._client.request(self._client.endpoints.studios)
+        response = await self._client.request(self._client.endpoints.forums)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Studio)
+                                            data_model=Forum)
```

### Comparing `shikithon-2.4.2/shikithon/resources/styles.py` & `shikithon-2.5/shikithon/resources/styles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Represents /api/styles resource."""
+"""Represents `/api/styles` resource."""
 from typing import Any, Dict, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType, StyleOwner
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import Style
 from ..utils import Utils
 from .base_resource import BaseResource
 
-STYLES_DICT_NAME = 'style'
+DICT_NAME = 'style'
 
 
 class Styles(BaseResource):
     """Styles resource class.
 
-    Used to represent /api/styles resource.
+    Used to represent `/api/styles` resource
     """
 
     @method_endpoint('/api/styles/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, style_id: int):
         """Returns info about style.
 
@@ -41,15 +41,15 @@
 
         :param css: CSS code to preview
         :type css: str
 
         :return: Info about previewed style
         :rtype: Optional[Style]
         """
-        data_dict = Utils.create_data_dict(dict_name=STYLES_DICT_NAME, css=css)
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME, css=css)
 
         response = await self._client.request(
             self._client.endpoints.style_preview,
             data=data_dict,
             request_type=RequestType.POST)
 
         return Utils.validate_response_data(cast(Dict[str, Any], response),
@@ -72,15 +72,15 @@
 
         :param owner_type: Type of owner
         :type owner_type: StyleOwner
 
         :return: Info about previewed style
         :rtype: Optional[Style]
         """
-        data_dict = Utils.create_data_dict(dict_name=STYLES_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            css=css,
                                            name=name,
                                            owner_id=owner_id,
                                            owner_type=owner_type)
 
         response = await self._client.request(self._client.endpoints.styles,
                                               data=data_dict,
@@ -105,15 +105,15 @@
 
         :param name: New style name
         :type name: Optional[str]
 
         :return: Info about updated style
         :rtype: Optional[Style]
         """
-        data_dict = Utils.create_data_dict(dict_name=STYLES_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            css=css,
                                            name=name)
 
         response = await self._client.request(
             self._client.endpoints.style(style_id),
             data=data_dict,
             request_type=RequestType.PATCH)
```

### Comparing `shikithon-2.4.2/shikithon/resources/topics.py` & `shikithon-2.5/shikithon/resources/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Represents /api/topics and /api/v2/topics resource."""
+"""Represents `/api/topics` and `/api/v2/topics` resources."""
 from typing import Any, Dict, List, Optional, cast
 
 from loguru import logger
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType, TopicForumType, TopicLinkedType, TopicType
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import Topic
+from ..models import Topic, TopicUpdate
 from ..utils import Utils
 from .base_resource import BaseResource
 
-TOPICS_DICT_NAME = 'topic'
+DICT_NAME = 'topic'
 
 
 class Topics(BaseResource):
     """Topics resource class.
 
-    Used to represent /api/topics and /api/v2/topics resource.
+    Used to represent `/api/topics` and `/api/v2/topics` resources
     """
 
     @method_endpoint('/api/topics')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None,
@@ -74,25 +74,25 @@
 
         :param page: Number of page
         :type page: Optional[int]
 
         :param limit: Number of results limit
         :type limit: Optional[int]
 
-        :return: List of topics
-        :rtype: List[Topic]
+        :return: List of topic updates
+        :rtype: List[TopicUpdate]
         """
         query_dict = Utils.create_query_dict(page=page, limit=limit)
 
         response = await self._client.request(
             self._client.endpoints.updates_topics, query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Topic)
+                                            data_model=TopicUpdate)
 
     @method_endpoint('/api/topics/hot')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def hot(self, limit: Optional[int] = None):
         """Returns list of hot topics.
 
         :param limit: Number of results limit
@@ -155,15 +155,15 @@
 
         :param linked_type: Type of linked topic (Used together with linked_id)
         :type linked_type: Optional[TopicLinkedType]
 
         :return: Created topic info
         :rtype: Optional[Topic]
         """
-        data_dict = Utils.create_data_dict(dict_name=TOPICS_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            body=body,
                                            forum_id=forum_id,
                                            linked_id=linked_id,
                                            linked_type=linked_type,
                                            title=title,
                                            type=TopicType.REGULAR_TOPIC,
                                            user_id=user_id)
@@ -199,15 +199,15 @@
 
         :param linked_type: Type of linked topic (Used together with linked_id)
         :type linked_type: Optional[TopicLinkedType]
 
         :return: Updated topic info
         :rtype: Optional[Topic]
         """
-        data_dict = Utils.create_data_dict(dict_name=TOPICS_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            body=body,
                                            linked_id=linked_id,
                                            linked_type=linked_type,
                                            title=title)
 
         response = await self._client.request(
             self._client.endpoints.topic(topic_id),
```

### Comparing `shikithon-2.4.2/shikithon/resources/user_images.py` & `shikithon-2.5/shikithon/resources/user_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Represents /api/user_images resource."""
+"""Represents `/api/user_images` resource."""
 from typing import Any, Dict, Optional, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import RequestType
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import CreatedUserImage
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class UserImages(BaseResource):
     """UserImages resource class.
 
-    Used to represent /api/user_images resource.
+    Used to represent `/api/user_images` resource
     """
 
     @method_endpoint('/api/user_images')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def create(self, image_path: str, linked_type: Optional[str] = None):
         """Creates an user image.
```

### Comparing `shikithon-2.4.2/shikithon/resources/user_rates.py` & `shikithon-2.5/shikithon/resources/user_rates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""Represents /api/user_rates and /api/v2/user_rates resource."""
+"""Represents `/api/user_rates` and `/api/v2/user_rates` resources."""
 from typing import Any, Dict, List, Optional, cast
 
 from loguru import logger
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import (RequestType, ResponseCode, UserRateStatus, UserRateTarget,
                      UserRateType)
 from ..exceptions import ShikimoriAPIResponseError
 from ..models import UserRate
 from ..utils import Utils
 from .base_resource import BaseResource
 
-USER_RATES_DICT_NAME = 'user_rate'
+DICT_NAME = 'user_rate'
 
 
 class UserRates(BaseResource):
     """UserRates resource class.
 
-    Used to represent /api/user_rates and /api/v2/user_rates resource.
+    Used to represent `/api/user_rates` and `/api/v2/user_rates` resources
     """
 
     @method_endpoint('/api/v2/user_rates')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       user_id: int,
                       target_id: Optional[int] = None,
                       target_type: Optional[UserRateTarget] = None,
                       status: Optional[UserRateStatus] = None,
                       page: Optional[int] = None,
                       limit: Optional[int] = None):
         """Returns list of user rates.
 
-        When passing target_id, target_type is required.
+        When passing target_id, target_type is required
 
         Also there is a strange API behavior, so when pass nothing,
         endpoint not working.
         However, docs shows that page/limit ignored when user_id is set (bruh)
 
         :param user_id: ID of user to get rates for
         :type user_id: int
@@ -135,15 +135,15 @@
 
         :param text: Text note for user rate
         :type text: Optional[str]
 
         :return: Info about new user rate
         :rtype: Optional[UserRate]
         """
-        data_dict = Utils.create_data_dict(dict_name=USER_RATES_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            user_id=user_id,
                                            target_id=target_id,
                                            target_type=target_type,
                                            status=status,
                                            score=score,
                                            chapters=chapters,
                                            episodes=episodes,
@@ -194,15 +194,15 @@
 
         :param text: Text note for user rate
         :type text: Optional[str]
 
         :return: Info about new user rate
         :rtype: Optional[UserRate]
         """
-        data_dict = Utils.create_data_dict(dict_name=USER_RATES_DICT_NAME,
+        data_dict = Utils.create_data_dict(dict_name=DICT_NAME,
                                            status=status,
                                            score=score,
                                            chapters=chapters,
                                            episodes=episodes,
                                            volumes=volumes,
                                            rewatches=rewatches,
                                            text=text)
```

### Comparing `shikithon-2.4.2/shikithon/resources/users.py` & `shikithon-2.5/shikithon/resources/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""Represents /api/users and /api/v2/users resource."""
+"""Represents `/api/users` and `/api/v2/users` resources."""
 from typing import Any, Dict, List, Optional, Union, cast
 
 from ..decorators import exceptions_handler, method_endpoint
 from ..enums import (AnimeCensorship, AnimeList, HistoryTargetType, MessageType,
                      RequestType)
 from ..exceptions import ShikimoriAPIResponseError
-from ..models import (Ban, Club, Favourites, History, Message, UnreadMessages,
-                      User, UserList)
+from ..models import (Ban, ClubInfo, Favourites, History, Message,
+                      UnreadMessages, User, UserInfo, UserBrief, UserList)
 from ..utils import Utils
 from .base_resource import BaseResource
 
 
 class Users(BaseResource):
     """Users resource class.
 
-    Used to represent /api/users and /api/v2/users resource.
+    Used to represent `/api/users` and `/api/v2/users` resources
     """
 
     @method_endpoint('/api/users')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def get_all(self,
                       page: Optional[int] = None,
                       limit: Optional[int] = None):
@@ -27,24 +27,24 @@
         :param page: Number of page
         :type page: Optional[int]
 
         :param limit: Number of results limit
         :type limit: Optional[int]
 
         :return: List of users
-        :rtype: List[User]
+        :rtype: List[UserInfo]
         """
         query_dict = Utils.create_query_dict(page=page, limit=limit)
 
         response = await self._client.request(self._client.endpoints.users,
                                               query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=User)
+                                            data_model=UserInfo)
 
     @method_endpoint('/api/users/:id')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def get(self, user_id: Union[str, int]):
         """Returns info about user.
 
         :param user_id: User ID/Nickname to get info
@@ -67,45 +67,44 @@
     async def info(self, user_id: Union[str, int]):
         """Returns user's brief info.
 
         :param user_id: User ID/Nickname to get brief info
         :type user_id: Union[int, str]
 
         :return: User's brief info
-        :rtype: Optional[User]
+        :rtype: Optional[UserBrief]
         """
         is_nickname = True if isinstance(user_id, str) else None
         query_dict = Utils.create_query_dict(is_nickname=is_nickname)
 
         response = await self._client.request(
             self._client.endpoints.user_info(user_id), query=query_dict)
 
         return Utils.validate_response_data(cast(Dict[str, Any], response),
-                                            data_model=User)
+                                            data_model=UserBrief)
 
     @method_endpoint('/api/users/whoami')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=None)
     async def current(self):
         """Returns brief info about current user.
 
         Current user evaluated depending on authorization code.
 
         :return: Current user brief info
-        :rtype: Optional[User]
+        :rtype: Optional[UserBrief]
         """
         response = await self._client.request(self._client.endpoints.whoami)
 
         return Utils.validate_response_data(cast(Dict[str, Any], response),
-                                            data_model=User)
+                                            data_model=UserBrief)
 
     @method_endpoint('/api/users/sign_out')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=False)
     async def sign_out(self):
-        """
-        Sends sign out request to API.
+        """Sends sign out request to API.
 
         :return: True if request was successful, False otherwise
         :rtype: bool
         """
         response = await self._client.request(self._client.endpoints.sign_out)
 
         return cast(str, response) == 'signed out'
@@ -115,46 +114,46 @@
     async def friends(self, user_id: Union[str, int]):
         """Returns user's friends.
 
         :param user_id: User ID/Nickname to get friends
         :type user_id: Union[int, str]
 
         :return: List of user's friends
-        :rtype: List[User]
+        :rtype: List[UserInfo]
         """
         is_nickname = True if isinstance(user_id, str) else None
         query_dict = Utils.create_query_dict(is_nickname=is_nickname)
 
         response = await self._client.request(
             self._client.endpoints.user_friends(user_id), query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=User)
+                                            data_model=UserInfo)
 
     @method_endpoint('/api/users/:id/clubs')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def clubs(self, user_id: Union[int, str]):
         """Returns user's clubs.
 
         :param user_id: User ID/Nickname to get clubs
         :type user_id: Union[int, str]
 
         :return: List of user's clubs
-        :rtype: List[Club]
+        :rtype: List[ClubInfo]
         """
         is_nickname = True if isinstance(user_id, str) else None
         query_dict = Utils.create_query_dict(is_nickname=is_nickname)
 
         response = await self._client.request(
             self._client.endpoints.user_clubs(user_id), query=query_dict)
 
         return Utils.validate_response_data(cast(List[Dict[str, Any]],
                                                  response),
-                                            data_model=Club)
+                                            data_model=ClubInfo)
 
     @method_endpoint('/api/users/:id/anime_rates')
     @exceptions_handler(ShikimoriAPIResponseError, fallback=[])
     async def anime_rates(self,
                           user_id: Union[int, str],
                           page: Optional[int] = None,
                           limit: Optional[int] = None,
```

### Comparing `shikithon-2.4.2/shikithon/store/base.py` & `shikithon-2.5/shikithon/store/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ConfigsDict = Dict[str, Config]
 
 
 class Store:
     """Abstract class for config store.
 
-    This class is used to create custom stores by overriding abstract methods.
+    This class is used to create custom stores by overriding abstract methods
     """
 
     __slots__ = ('_closed',)
 
     def __init__(self):
         self._closed = True
```

### Comparing `shikithon-2.4.2/shikithon/store/json.py` & `shikithon-2.5/shikithon/store/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .base import ConfigsDict, Store
 from .memory import MemoryStore
 
 
 class JSONStore(Store):
     """JSON config store class.
 
-    This class is used for storing configs in JSON file.
+    This class is used for storing configs in JSON file
     """
 
     __slots__ = ('_file_path',)
 
     def __init__(self, file_path: str = '.shikithon'):
         super().__init__()
         self._file_path = file_path
```

### Comparing `shikithon-2.4.2/shikithon/store/memory.py` & `shikithon-2.5/shikithon/store/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..exceptions import StoreException
 from .base import ConfigsDict, ReturnConfig, Store, Token
 
 
 class MemoryStore(Store):
     """Memory config store class.
 
-    This class is used for storing configs in RAM for faster access.
+    This class is used for storing configs in RAM for faster access
     """
 
     __slots__ = ('_configs',)
 
     def __init__(self, configs: Optional[ConfigsDict] = None):
         super().__init__()
         self._configs: ConfigsDict = configs or {}
```

### Comparing `shikithon-2.4.2/shikithon/store/null.py` & `shikithon-2.5/shikithon/store/null.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .base import ReturnConfig, Store
 
 
 class NullStore(Store):
     """Dummy store with an empty implementation of an abstract store class.
 
-    This store is used when no store is provided to the client.
+    This store is used when no store is provided to the client
     """
 
     async def save_config(self,
                           app_name: str,
                           client_id: str,
                           client_secret: str,
                           redirect_uri: str,
```

### Comparing `shikithon-2.4.2/shikithon/utils/utils.py` & `shikithon-2.5/shikithon/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-"""
-Set of utility methods for the shikithon library.
+"""Set of utility methods for the shikithon library.
 
 This file contains the Utils class
 with all the necessary utility methods
 to work with the library
 """
 
 import imghdr
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union, overload
 
 from aiohttp import ClientResponse, ClientSession, FormData
 from loguru import logger
-from pydantic import BaseModel
+from pydantic import BaseModel, parse_obj_as
 from validators import url
 
 from ..enums import ResponseCode
 
 LOWER_LIMIT_NUMBER = 1
 M = TypeVar('M', bound=BaseModel)
 
+R = TypeVar('R')
+T = TypeVar('T')
+
 
 class Utils:
-    """
-    Utils class.
+    """Utils class.
 
     Contains all the necessary utility methods
     to work with the library
     """
 
     @staticmethod
     def convert_to_query_string(query_dict: Optional[Dict[str, str]]):
         """Converts query dict to query string for endpoint link.
 
-        If query_dict is None or empty, returns empty string.
+        If query_dict is None or empty, returns empty string
 
         :param query_dict: Query dictionary
         :type query_dict: Dict[str, str]
 
         :return: Query string
         :rtype: str
         """
@@ -55,15 +56,15 @@
         logger.debug(f'Formed string: "{query_string}"')
         return query_string
 
     @staticmethod
     async def get_image_data(image_path: Optional[str]):
         """Extracts image data from image path.
 
-        If image_path is a link, fetch the image data from the link.
+        If image_path is a link, fetch the image data from the link
 
         :param image_path: Path to image
         :type image_path: str
 
         :return: Image data
         :rtype: Optional[bytes]
         """
@@ -121,15 +122,15 @@
             logger.debug('Successfully extracted image data')
             return await image_response.read()
 
     @staticmethod
     def create_query_dict(**params_data: Optional[Any]):
         """Creates query dictionary for API request.
 
-        This methods checks for data types and converts to valid one.
+        This methods checks for data types and converts to valid one
 
         :param params_data: Parameters data for API request
         :type params_data: Optional[Any]
 
         :return: Query dictionary
         :rtype: Dict[str, str]
         """
@@ -149,19 +150,19 @@
         logger.debug(f'Generated query dictionary: {query_dict=}')
         return query_dict
 
     @staticmethod
     def create_data_dict(**dict_data: Optional[Any]):
         """Creates data dictionary for API request.
 
-        This methods checks for data types and converts to valid one.
+        This methods checks for data types and converts to valid one
 
         If dict_data doesn't contain "dict_name" key,
         generated dictionary will have "temp" as root dictionary name,
-        which will be removed on return.
+        which will be removed on return
 
         :param dict_data: Body data for API request
         :type dict_data: Optional[Any]
 
         :return: Data dictionary
         :rtype: Union[Dict[str, Dict[str, str]], Dict[str, str]]
         """
@@ -192,15 +193,15 @@
         return new_data_dict
 
     @staticmethod
     def _convert_dictionary_value(dict_value: Any, data_dict: bool = False):
         """Converts dictionary value to string.
 
         If data_dict is False, converts list values to comma-separated string.
-        Otherwise, returns list value as is.
+        Otherwise, returns list value as is
 
         :param dict_value: Dictionary value
         :type dict_value: Any
 
         :param data_dict: Flag if checking value for data dictionary
         :type data_dict: bool
 
@@ -282,27 +283,46 @@
         """
         logger.debug('Validating and parsing response data '\
                     f'using "{data_model.__name__}" data model')
         logger.debug(f'Passed response data: {response_data}')
 
         if not response_data:
             logger.debug('Response data is empty. Returning')
-            if isinstance(response_data, dict):
-                return None
-            return []
+            return [] if isinstance(response_data, list) else None
 
         return [data_model(**item) for item in response_data] if isinstance(
             response_data, list) else data_model(**response_data)
 
     @staticmethod
+    def parse_mixed_response(response: Any, parse_type: Type[T]):
+        """Parses response, mixed with other entities,
+        that can't be parsed with validation utility.
+
+        Due to fact, that every Manga and Ranobe can have both models as
+        similar, this utility method helps parse response correctly
+
+        :param response: Passed response data
+        :type response: Any
+
+        :param parse_type: Type for parsing response to
+        :type parse_type: Type[T]
+
+        :return: Parsed response to passed type
+        :rtype: T
+        """
+        logger.info('Parsing response with mixed models')
+        logger.info(f'Parsing using type: {parse_type}')
+        return parse_obj_as(parse_type, response)
+
+    @staticmethod
     def create_form_data(raw_data: Dict[str, Any]):
         """Creates form data for API request.
 
         Method converts dictionary with data to
-        FormData object for API request.
+        FormData object for API request
 
         :param raw_data: Raw data for API request
         :type raw_data: Dict[str, Any]
 
         :return: Form data
         :rtype: Optional[FormData]
         """
@@ -364,13 +384,15 @@
         logger.debug('Successfully generated FormData object')
         return form_data
 
     @staticmethod
     async def log_response_info(response: ClientResponse):
         """Logs response info.
 
+        This method extracts response status, headers and data
+
         :param response: Response object
         :type response: ClientResponse
         """
         logger.debug(f'Response status: {response.status}')
         logger.debug(f'Response headers: {response.headers}')
         logger.debug(f'Response data: {await response.text()}')
```

### Comparing `shikithon-2.4.2/PKG-INFO` & `shikithon-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shikithon
-Version: 2.4.2
+Version: 2.5
 Summary: Yet another Python wrapper for Shikimori API
 Home-page: https://github.com/SecondThundeR/shikithon
 License: MIT
 Keywords: Python,Shikimori,API
 Author: SecondThundeR
 Author-email: awayfromgalaxy@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
@@ -40,32 +40,31 @@
 > На данный момент, библиотека находится в статусе поддержки (новые функции будут добавляться только по необходимости)
 >
 > Начиная с версии 2.0.0, библиотека поддерживает асинхронные запросы, отдельные пути к ресурсам API и многое другое
 > _[(Инструкция по миграции с версии 1.x.x)](https://github.com/SecondThundeR/shikithon/wiki/%D0%9C%D0%B8%D0%B3%D1%80%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%81-v1-%D0%BD%D0%B0-v2)_
 
 ## Описание
 
-Данный враппер предоставляет абстракцию, которая позволяет удобнее работать с методами API и их ответами.
+Данный враппер предоставляет абстракцию, которая позволяет удобнее работать с методами API и их ответами
 
-Для каждого эндпоинта API существует свой объект с методами, которые благодаря библиотеке Pydantic,
-возвращают удобную модель данных.
-
-Все данные, возвращаемые API Shikimori, валидируются и парсятся в модели, со всеми необходимыми полями,
+Для каждого эндпоинта API существует свой объект с методами, и все данные, возвращаемые API Shikimori, валидируются и парсятся в модели, со всеми необходимыми полями,
 а также дополнительными, которые могут вернуть некоторые методы API _(Например /users/whoami и /users/:id/info возвращают разные поля)_.
-Это позволяет не задумываться об обработке очередного ответа от сервера и сосредоточиться над реализацией своей идеи.
+Это позволяет не задумываться об обработке очередного ответа от сервера и сосредоточиться над реализацией своей идеи
 
-Также благодаря многочисленным проверкам при взамодействии с запросами, библиотека старается добиться максимально
-безопасной работы с API: все ошибки API, переданных параметров, данных и т.д. обратываются и логируются и
-возвращаются значения по умолчанию
+Также благодаря множеству проверок при взаимодействии с запросами, библиотека старается добиться максимально
+безопасной работы с API: все ошибки API, переданных параметров, данных и т.д. обратываются, логируются и
+пользователю возвращаются значения по умолчанию
 
 > Данная библиотека начинает свою поддержку с Python 3.8.10.
 
 ## Установка
 
- ```pip install shikithon```
+```shell
+pip install shikithon
+```
 
 ## Пример использования
 
 ```py
 import asyncio
 
 from typing import Dict
@@ -91,15 +90,15 @@
 
 # Или же прочитать его из внешнего файла
 with open("config.json", "r", encoding="utf-8") as config_file:
     config_2: Dict[str, str] = loads(config_file.read())
 
 # Инициализируем API объект с необходимыми опциями
 # В данном примере используется JSONStore и отключено логирование
-api = ShikimoriAPI(app_name=config['app_name'], store=JSONStore(), logging=False)
+api = ShikimoriAPI(app_name=config['app_name'], store=JSONStore())
 
 async def main():
     # Используем объект без авторизации
     async with api:
         lycoris = await api.animes.get(50709)
         print(lycoris)
         # >> id=50709 name='Lycoris Recoil' russian='Ликорис Рикоил' ...
@@ -110,15 +109,15 @@
     # Вариант 1
     async with api.auth(
         client_id=config["client_id"],
         client_secret=config["client_secret"],
         auth_code=config["auth_code"],
     ):
         print(await api.users.current())
-        # >> User(id=723052, nickname='SecondThundeR', ...
+        # >> UserBrief(id=723052, nickname='SecondThundeR', ...
 
     # Вариант 2
 
     # Создаем новый объект API
     # (По умолчанию используется NullStore в качестве хранилища)
     api_2 = ShikimoriAPI(app_name="...")
 
@@ -157,17 +156,17 @@
             api.characters.search("Тисато Нисикиги"),
             api.ranobes.get_all(search="Ликорис"),
         ])
         print(chainsaw)
         print(lycoris_chisato[:1])
         print(lycoris_ranobe)
 
-# [Anime(id=44511, name='Chainsaw Man', russian='Человек-бензопила', ...]
-# [Character(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
-# [Ranobe(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
+# [AnimeInfo(id=44511, name='Chainsaw Man', russian='Человек-бензопила', ...]
+# [CharacterInfo(id=204621, name='Chisato Nishikigi', russian='Тисато Нисикиги', ...]
+# [RanobeInfo(id=151431, name='Lycoris Recoil: Ordinary Days', russian='Ликорис Рикоил: Повседневность', ...]
 ```
 
 Также, если хочется узнать как использовать встроенные хранилища конфигов или хочется создать свой,
 посмотрите [этот гайд](https://github.com/SecondThundeR/shikithon/wiki/%D0%93%D0%B0%D0%B9%D0%B4-%D0%BF%D0%BE-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B0%D0%BC-%D0%BA%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D0%B8)
 
 ### Пара уточнений по использованию
 
@@ -223,14 +222,14 @@
 
 ## Лицензия проекта
 
 Данный проект имеет MIT лицензию.
 Ознакомиться с ее содержанием можно [здесь](https://github.com/SecondThundeR/shikithon/blob/main/LICENSE)
 
 Проект использует логотип сайта [Shikimori](https://shikimori.org) для логотипа в этом README.md.
-Все права принадлежат правообладателям и используются по принципу _fair use_.
+Все права принадлежат правообладателям и используются по принципу _fair use_
 
 ## Благодарности
 
 - [shiki4py](https://github.com/ren3104/Shiki4py) - взяты некоторые идеи по рефакторингу и добавлению поддержки асинхронных запросов
 [(Лицензия)](https://github.com/ren3104/Shiki4py/blob/main/LICENSE)
```

