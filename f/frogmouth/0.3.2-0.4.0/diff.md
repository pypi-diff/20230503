# Comparing `tmp/frogmouth-0.3.2.tar.gz` & `tmp/frogmouth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.3.2.tar", max compression
+gzip compressed data, was "frogmouth-0.4.0.tar", max compression
```

## Comparing `frogmouth-0.3.2.tar` & `frogmouth-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.3.2/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.3.2/README.md
--rw-r--r--   0        0        0      283 2023-04-30 11:12:52.375078 frogmouth-0.3.2/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.3.2/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.3.2/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.3.2/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.3.2/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.3.2/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.3.2/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.3.2/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.3.2/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.3.2/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.3.2/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.3.2/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.3.2/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.3.2/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.3.2/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.3.2/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.3.2/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    18984 2023-04-30 11:10:42.376816 frogmouth-0.3.2/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.3.2/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.3.2/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.3.2/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.3.2/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.3.2/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.3.2/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.3.2/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.3.2/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1468 2023-04-30 11:13:02.337061 frogmouth-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.4.0/README.md
+-rw-r--r--   0        0        0      283 2023-05-03 09:31:33.035349 frogmouth-0.4.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.4.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.4.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.4.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.4.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.4.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.4.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.4.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.4.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.4.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.4.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.4.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.4.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     2717 2023-05-03 09:31:33.036023 frogmouth-0.4.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.4.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.4.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.4.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    18746 2023-05-03 09:31:33.036343 frogmouth-0.4.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.4.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.4.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.4.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.4.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.4.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-03 09:31:33.037070 frogmouth-0.4.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.4.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    11675 2023-05-03 09:31:33.038042 frogmouth-0.4.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0    10129 2023-05-01 07:06:00.079325 frogmouth-0.4.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1468 2023-05-03 09:31:33.038167 frogmouth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.4.0/PKG-INFO
```

### Comparing `frogmouth-0.3.2/LICENSE` & `frogmouth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/README.md` & `frogmouth-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/app/app.py` & `frogmouth-0.4.0/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/data/bookmarks.py` & `frogmouth-0.4.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/data/config.py` & `frogmouth-0.4.0/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/data/data_directory.py` & `frogmouth-0.4.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/data/history.py` & `frogmouth-0.4.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/dialogs/error.py` & `frogmouth-0.4.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.4.0/frogmouth/dialogs/help_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.4.0/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/screens/main.py` & `frogmouth-0.4.0/frogmouth/screens/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The main screen for the application."""
 
 from __future__ import annotations
 
+from functools import partial
 from pathlib import Path
 from typing import Awaitable, Callable
 from webbrowser import open as open_url
 
 from httpx import URL
 from textual.app import ComposeResult
 from textual.binding import Binding
@@ -83,15 +84,15 @@
         border-bottom: heavy $accent !important;
         border-left: heavy $accent !important;
     }
 
     """
 
     BINDINGS = [
-        Binding("/", "omnibox", "Omnibox", show=False),
+        Binding("/,:", "omnibox", "Omnibox", show=False),
         Binding("ctrl+b", "bookmarks", "", show=False),
         Binding("ctrl+d", "bookmark_this", "", show=False),
         Binding("ctrl+l", "local_files", "", show=False),
         Binding("ctrl+left", "backward", "", show=False),
         Binding("ctrl+right", "forward", "", show=False),
         Binding("ctrl+t", "table_of_contents", "", show=False),
         Binding("ctrl+y", "history", "", show=False),
@@ -467,14 +468,23 @@
                 f"Built with [@click=app.visit('{TEXTUAL_URL}')]Textual[/] "
                 f"by [@click=app.visit('{ORGANISATION_URL}')]{ORGANISATION_TITLE}[/].\n\n"
                 f"[@click=app.visit('https://github.com/{ORGANISATION_NAME}/{PACKAGE_NAME}')]"
                 f"https://github.com/{ORGANISATION_NAME}/{PACKAGE_NAME}[/]",
             )
         )
 
+    def add_bookmark(self, location: Path | URL, bookmark: str) -> None:
+        """Handle adding the bookmark.
+
+        Args:
+            location: The location to bookmark.
+            bookmark: The bookmark to add.
+        """
+        self.query_one(Navigation).bookmarks.add_bookmark(bookmark, location)
+
     def action_bookmark_this(self) -> None:
         """Add a bookmark for the currently-viewed file."""
 
         location = self.query_one(Viewer).location
 
         # Only allow bookmarking if we're actually viewing something that
         # can be bookmarked.
@@ -489,31 +499,18 @@
 
         # To make a bookmark, we need a title and a location. We've got a
         # location; let's make the filename the default title.
         title = (location if isinstance(location, Path) else Path(location.path)).name
 
         # Give the user a chance to edit the title.
         self.app.push_screen(
-            InputDialog(self, "Bookmark title:", title, location, id="add_bookmark")
+            InputDialog("Bookmark title:", title),
+            partial(self.add_bookmark, location),
         )
 
-    def on_input_dialog_result(self, event: InputDialog.Result) -> None:
-        """Handle a result coming back from an input dialog.
-
-        Args:
-            event: The input dialog result event.
-        """
-        # Handle the correct source dialog.
-        if event.sender_id == "add_bookmark":
-            # The cargo value for the result should be the location, which
-            # should be a path or a URL.
-            assert isinstance(event.cargo, (Path, URL))
-            # Save the bookmark.
-            self.query_one(Navigation).bookmarks.add_bookmark(event.value, event.cargo)
-
     def action_toggle_theme(self) -> None:
         """Toggle the light/dark mode theme."""
         config = load_config()
         config.light_mode = not config.light_mode
         save_config(config)
         # pylint:disable=attribute-defined-outside-init
         self.app.dark = not config.light_mode
```

### Comparing `frogmouth-0.3.2/frogmouth/utility/advertising.py` & `frogmouth-0.4.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/utility/forge.py` & `frogmouth-0.4.0/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/utility/type_tests.py` & `frogmouth-0.4.0/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Vertical
 from textual.reactive import var
 from textual.widgets import TabbedContent, Tabs
 from typing_extensions import Self
 
-from .navigation_panes.navigation_pane import NavigationPane
 from .navigation_panes.bookmarks import Bookmarks
 from .navigation_panes.history import History
 from .navigation_panes.local_files import LocalFiles
+from .navigation_panes.navigation_pane import NavigationPane
 from .navigation_panes.table_of_contents import TableOfContents
 
 
 class Navigation(Vertical, can_focus=False, can_focus_children=True):
     """A navigation panel widget."""
 
     DEFAULT_CSS = """
```

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provides the bookmarks navigation pane."""
 
 from __future__ import annotations
 
+from functools import partial
 from pathlib import Path
 
 from httpx import URL
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.message import Message
@@ -119,54 +120,51 @@
         Args:
             event: The event to handle.
         """
         event.stop()
         assert isinstance(event.option, Entry)
         self.post_message(self.Goto(event.option.bookmark))
 
+    def delete_bookmark(self, bookmark: int, delete_it: bool) -> None:
+        """Delete a given bookmark.
+
+        Args:
+            bookmark: The bookmark to delete.
+            delete_it: Should it be deleted?
+        """
+        if delete_it:
+            del self._bookmarks[bookmark]
+            self._bookmarks_updated()
+
     def action_delete(self) -> None:
         """Delete the highlighted bookmark."""
-        if self.query_one(OptionList).highlighted is not None:
+        if (bookmark := self.query_one(OptionList).highlighted) is not None:
             self.app.push_screen(
                 YesNoDialog(
-                    self,
                     "Delete bookmark",
                     "Are you sure you want to delete the bookmark?",
-                    id="delete",
-                )
+                ),
+                partial(self.delete_bookmark, bookmark),
             )
 
-    def on_yes_no_dialog_positive_reply(self, event: YesNoDialog.PositiveReply) -> None:
-        """Handle a yes/no dialog giving a positive reply.
+    def rename_bookmark(self, bookmark: int, new_name: str) -> None:
+        """Rename the current bookmark.
 
         Args:
-            event: The event to handle.
+            bookmark: The location of the bookmark to rename.
+            new_name: The input dialog result that is the new name.
         """
-        bookmarks = self.query_one(OptionList)
-        if event.sender_id == "delete" and bookmarks.highlighted is not None:
-            del self._bookmarks[bookmarks.highlighted]
-            self._bookmarks_updated()
+        self._bookmarks[bookmark] = Bookmark(
+            new_name, self._bookmarks[bookmark].location
+        )
+        self._bookmarks_updated()
 
     def action_rename(self) -> None:
         """Rename the highlighted bookmark."""
         if (bookmark := self.query_one(OptionList).highlighted) is not None:
             self.app.push_screen(
                 InputDialog(
-                    self,
                     "Bookmark title:",
                     self._bookmarks[bookmark].title,
-                    bookmark,
-                    id="edit_title",
-                )
+                ),
+                partial(self.rename_bookmark, bookmark),
             )
-
-    def on_input_dialog_result(self, event: InputDialog.Result) -> None:
-        """Handle an input dialog result being passed to us."""
-        if event.sender_id == "edit_title":
-            # The cargo value for the result should be the index of the
-            # bookmark we're changing.
-            assert isinstance(event.cargo, int)
-            # Everything looks good, update the bookmarks.
-            self._bookmarks[event.cargo] = Bookmark(
-                event.value, self._bookmarks[event.cargo].location
-            )
-            self._bookmarks_updated()
```

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Provides a base class for all navigation panes."""
 
-from typing_extensions import Self
-
-
 from textual.widgets import TabbedContent, TabPane
+from typing_extensions import Self
 
 
 class NavigationPane(TabPane):
     """Base class for panes within the navigation sidebar."""
 
     def set_focus_within(self) -> None:
         """Set the focus on the correct child within the navigation pane."""
```

### Comparing `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.4.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.2/frogmouth/widgets/omnibox.py` & `frogmouth-0.4.0/frogmouth/widgets/omnibox.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
     _SPECIFIC_BRANCH = compile_regexp(
         r"^(?P<owner>[^/ ]+)[/ ](?P<repo>[^ :]+):(?P<branch>[^ ]+)(?: +(?P<file>[^ ]+))?$"
     )
     """Regular expression for matching a repo and file where the branch is also given."""
 
     class ForgeCommand(Message):
-        """The base git force quick load command."""
+        """The base git forge quick load command."""
 
         def __init__(
             self,
             owner: str,
             repository: str,
             branch: str | None = None,
             desired_file: str | None = None,
```

### Comparing `frogmouth-0.3.2/frogmouth/widgets/viewer.py` & `frogmouth-0.4.0/frogmouth/widgets/viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from typing import Callable
 from webbrowser import open as open_url
 
 from httpx import URL, AsyncClient, HTTPStatusError, RequestError
 from textual import work
 from textual.app import ComposeResult
+from textual.binding import Binding
 from textual.containers import VerticalScroll
 from textual.message import Message
 from textual.reactive import var
 from textual.widgets import Markdown
 from typing_extensions import Final
 
 from .. import __version__
@@ -98,14 +99,22 @@
     DEFAULT_CSS = """
     Viewer {
         width: 1fr;
         scrollbar-gutter: stable;
     }
     """
 
+    BINDINGS = [
+        Binding("w,k", "scroll_up", "", show=False),
+        Binding("s,j", "scroll_down", "", show=False),
+        Binding("space", "page_down", "", show=False),
+        Binding("b", "page_up", "", show=False),
+    ]
+    """Bindings for the Markdown viewer widget."""
+
     history: var[History] = var(History)
     """The browsing history."""
 
     viewing_location: var[bool] = var(False)
     """Is an actual location being viewed?"""
 
     class ViewerMessage(Message):
```

### Comparing `frogmouth-0.3.2/pyproject.toml` & `frogmouth-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.3.2"
+version = "0.4.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `frogmouth-0.3.2/PKG-INFO` & `frogmouth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.3.2 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.4.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
```

