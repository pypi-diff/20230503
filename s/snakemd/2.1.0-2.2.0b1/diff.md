# Comparing `tmp/snakemd-2.1.0.tar.gz` & `tmp/snakemd-2.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemd-2.1.0.tar", max compression
+gzip compressed data, was "snakemd-2.2.0b1.tar", max compression
```

## Comparing `snakemd-2.1.0.tar` & `snakemd-2.2.0b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-29 18:06:06.129025 snakemd-2.1.0/LICENSE
--rw-r--r--   0        0        0     7060 2023-04-29 18:06:06.129025 snakemd-2.1.0/README.md
--rw-r--r--   0        0        0     1414 2023-04-29 18:06:06.133025 snakemd-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      594 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/__init__.py
--rw-r--r--   0        0        0    13530 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/document.py
--rw-r--r--   0        0        0    40086 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/elements.py
--rw-r--r--   0        0        0     3319 2023-04-29 18:06:06.133025 snakemd-2.1.0/snakemd/templates.py
--rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 snakemd-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/LICENSE
+-rw-r--r--   0        0        0     6958 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/README.md
+-rw-r--r--   0        0        0     2196 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0      930 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/snakemd/__init__.py
+-rw-r--r--   0        0        0    15776 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/snakemd/document.py
+-rw-r--r--   0        0        0    47325 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/snakemd/elements.py
+-rw-r--r--   0        0        0     4726 2023-05-03 02:22:02.039395 snakemd-2.2.0b1/snakemd/templates.py
+-rw-r--r--   0        0        0     8113 1970-01-01 00:00:00.000000 snakemd-2.2.0b1/PKG-INFO
```

### Comparing `snakemd-2.1.0/LICENSE` & `snakemd-2.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemd-2.1.0/README.md` & `snakemd-2.2.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,19 @@
 
 Links are targets to files or web pages and can be embedded in paragraphs in a variety of ways, such as with the insert_link() method.
 
 _SnakeMD Source_
 
 ```py
 def _insert_link(doc: Document):
-    doc.add_paragraph("Learn to program with The Renegade Coder (@RenegadeCoder94).") \
-        .insert_link("The Renegade Coder", "https://therenegadecoder.com") \
-        .insert_link("@RenegadeCoder94", "https://twitter.com/RenegadeCoder94")
+    doc.add_paragraph(
+        "Learn to program with The Renegade Coder (@RenegadeCoder94)."
+    ).insert_link("The Renegade Coder", "https://therenegadecoder.com").insert_link(
+        "@RenegadeCoder94", "https://twitter.com/RenegadeCoder94"
+    )
 ```
 
 _Markdown Source_
 
 ```markdown
 Learn to program with [The Renegade Coder](https://therenegadecoder.com) ([@RenegadeCoder94](https://twitter.com/RenegadeCoder94)).
 ```
@@ -158,21 +160,15 @@
 
 Checklists are lists in which the items themselves can be checked on and off. This feature is new as of v0.10.0.
 
 _SnakeMD Source_
 
 ```py
 def _checklist(doc: Document):
-    doc.add_checklist(
-        [
-            "Pass the puck",
-            "Shoot the puck",
-            "Score a goal"
-        ]
-    )
+    doc.add_checklist(["Pass the puck", "Shoot the puck", "Score a goal"])
 ```
 
 _Markdown Source_
 
 ```markdown
 - [ ] Pass the puck
 - [ ] Shoot the puck
@@ -190,23 +186,22 @@
 Nested lists are complex lists that contain lists. Currently, SnakeMD does not support any convenience methods to generate nested lists, but they can be created manually using the MDList object.
 
 _SnakeMD Source_
 
 ```py
 def _nested_list(doc: Document):
     doc.add_block(
-        MDList([
-            "Apples",
-            Inline("Onions", bold=True),
-            MDList([
-                "Sweet",
-                "Red"
-            ]),
-            Paragraph(["This is the end of the list!"])
-        ])
+        MDList(
+            [
+                "Apples",
+                Inline("Onions", bold=True),
+                MDList(["Sweet", "Red"]),
+                Paragraph(["This is the end of the list!"]),
+            ]
+        )
     )
 ```
 
 _Markdown Source_
 
 ```markdown
 - Apples
@@ -230,21 +225,17 @@
 
 _SnakeMD Source_
 
 ```py
 def _table(doc: Document):
     doc.add_table(
         ["Height (cm)", "Weight (kg)", "Age (y)"],
-        [
-            ['150', '70', '21'],
-            ['164', '75', '19'],
-            ['181', '87', '40']
-        ],
+        [["150", "70", "21"], ["164", "75", "19"], ["181", "87", "40"]],
         [Table.Align.LEFT, Table.Align.CENTER, Table.Align.RIGHT],
-        0
+        0,
     )
 ```
 
 _Markdown Source_
 
 ```markdown
 | Height (cm) | Weight (kg) | Age (y) |
```

### Comparing `snakemd-2.1.0/snakemd/document.py` & `snakemd-2.2.0b1/snakemd/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,396 +1,492 @@
+"""
+The document module houses the Document class, a tool for
+generating markdown documents.
+"""
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 import random
 from typing import Iterable
 
-from .elements import *
-from .templates import *
+from .elements import (
+    Block,
+    Code,
+    Element,
+    Heading,
+    HorizontalRule,
+    Inline,
+    MDList,
+    Paragraph,
+    Quote,
+    Raw,
+    Table,
+)
+from .templates import TableOfContents, Template
 
 logger = logging.getLogger(__name__)
 
 
 class Document:
     """
     A document represents a markdown file. Documents store
-    a collection of blocks which are appended with new lines
+    a collection of elements which are appended with new lines
     between to generate the markdown document. Document methods
     are intended to provided convenience when generating a
     markdown file. However, the functionality is not exhaustive.
     To get the full range of markdown functionality, you can
     take advantage of the :func:`add_block` function to provide
     custom markdown blocks.
 
     .. testsetup:: document
-    
+
         import snakemd
-        
+
     .. testcleanup:: document
-    
+
         import os
         os.remove("README.md")
+
+    :param list[Element] elements:
+        an optional list of elements that make up a markdown document
+
+        .. versionadded:: 2.2
+            Included to make __repr__ more useful
     """
 
-    def __init__(self) -> None:
-        self._contents: list[Block] = list()
-        logger.debug("New document initialized")
+    def __init__(self, elements: list[Element] = None) -> None:
+        self._elements: list[Element] = elements or []
+        logger.info("Created new document: %r", self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
-        Renders the markdown document from a list of blocks.
+        Renders the markdown document from a list of elements.
+
+        .. doctest:: document
 
-        :return: 
+            >>> doc = snakemd.new_doc()
+            >>> doc.add_heading("First")
+            Heading(text=[...], level=1)
+            >>> print(doc)
+            # First
+
+        :return:
             the document as a markdown string
         """
-        return "\n\n".join(str(block) for block in self._contents)
+        # load templates
+        for block in self._elements:
+            if isinstance(block, Template):
+                block.load(self._elements)
+        # render all
+        document = "\n\n".join(str(block) for block in self._elements)
+        logger.info("Rendered document: %r", document)
+        return document
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        .. doctest:: document
+
+            >>> doc = snakemd.new_doc()
+            >>> repr(doc)
+            'Document(elements=[])'
+
+        :return:
+            the MDList object as a development string
+        """
+        return f"Document(elements={self._elements!r})"
+
+    def get_elements(self) -> list[Element]:
+        """
+        A getter method which allows the user to retrieve
+        the underlying document structure of elements
+        as a list. The return value is directly aliased
+        to the underlying representation, so any changes
+        to this object will change the document.
+
+        The primary use of this method is to share an
+        alias to the underlying document structure to
+        other useful components like TableOfContents
+        without creating circular references.
+
+        .. versionadded:: 2.2
+            Included as a part of the TableOfContents rework
+
+        :return:
+            the list of block comprising this document
+        """
+        return self._elements
 
     def add_block(self, block: Block) -> Block:
         """
         A generic function for appending blocks to the document.
         Use this function when you want a little more control over
         what the output looks like.
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
-            >>> doc.add_block(snakemd.Heading("Python is Cool!", 2)) 
-            <snakemd.elements.Heading object at ...>
-            >>> str(doc)
-            '## Python is Cool!'
+            >>> doc.add_block(snakemd.Heading("Python is Cool!", 2))
+            Heading(text=[Inline(text='Python is Cool!',...)], level=2)
+            >>> print(doc)
+            ## Python is Cool!
 
-        :param Block block: 
+        :param Block block:
             a markdown block (e.g., Table, Heading, etc.)
-        :return: 
+        :return:
             the :class:`Block` added to this Document
         """
-        self._contents.append(block)
-        logger.debug(f"Added custom block to document\n{block}")
+        self._elements.append(block)
+        logger.info("Added custom block to document: %r", block)
         return block
 
     def add_raw(self, text: str) -> Raw:
         """
         A convenience method which adds text as-is to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_raw("X: 5\\nY: 4\\nZ: 3")
-            <snakemd.elements.Raw object at ...>
-            >>> str(doc)
-            'X: 5\\nY: 4\\nZ: 3'
-
-        :param str text: 
-            some text 
-        :return: 
+            Raw(text='X: 5\\nY: 4\\nZ: 3')
+            >>> print(doc)
+            X: 5
+            Y: 4
+            Z: 3
+
+        :param str text:
+            some text
+        :return:
             the :class:`Raw` block added to this Document
         """
         raw = Raw(text)
-        self._contents.append(raw)
-        logger.debug(f"Added raw block to document\n{text}")
+        self._elements.append(raw)
+        logger.info("Added raw block to document: %r", text)
         return raw
 
     def add_heading(self, text: str, level: int = 1) -> Heading:
         """
         A convenience method which adds a heading to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_heading("Welcome to SnakeMD!")
-            <snakemd.elements.Heading object at ...>
-            >>> str(doc)
-            '# Welcome to SnakeMD!'
+            Heading(text=[Inline(text='Welcome to SnakeMD!',...)], level=1)
+            >>> print(doc)
+            # Welcome to SnakeMD!
 
-        .. code-block:: Python
-
-            doc.add_heading("Welcome to SnakeMD!")
-
-        :param str text: 
+        :param str text:
             the text for the heading
-        :param int level: 
+        :param int level:
             the level of the heading from 1 to 6
-        :return: 
+        :return:
             the :class:`Heading` added to this Document
         """
         heading = Heading(Inline(text), level)
-        self._contents.append(heading)
-        logger.debug(f"Added heading to document\n{heading}")
+        self._elements.append(heading)
+        logger.info("Added heading to document: %r", heading)
         return heading
 
     def add_paragraph(self, text: str) -> Paragraph:
         """
         A convenience method which adds a paragraph of text to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_paragraph("Mitochondria is the powerhouse of the cell.")
-            <snakemd.elements.Paragraph object at ...>
-            >>> str(doc)
-            'Mitochondria is the powerhouse of the cell.'
+            Paragraph(content=[...])
+            >>> print(doc)
+            Mitochondria is the powerhouse of the cell.
 
-        :param str text: 
+        :param str text:
             any arbitrary text
-        :return: 
+        :return:
             the :class:`Paragraph` added to this Document
         """
         paragraph = Paragraph([Inline(text)])
-        self._contents.append(paragraph)
-        logger.debug(f"Added paragraph to document\n{paragraph}")
+        self._elements.append(paragraph)
+        logger.info("Added paragraph to document: %r", paragraph)
         return paragraph
 
     def add_ordered_list(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds an ordered list to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_ordered_list(["Goku", "Piccolo", "Vegeta"])
-            <snakemd.elements.MDList object at ...>
-            >>> str(doc)
-            '1. Goku\\n2. Piccolo\\n3. Vegeta'
+            MDList(items=[...], ordered=True, checked=None)
+            >>> print(doc)
+            1. Goku
+            2. Piccolo
+            3. Vegeta
 
-        :param Iterable[str] items: 
+        :param Iterable[str] items:
             a "list" of strings
-        :return: 
+        :return:
             the :class:`MDList` added to this Document
         """
         md_list = MDList(items, ordered=True)
-        self._contents.append(md_list)
-        logger.debug(f"Added ordered list to document\n{md_list}")
+        self._elements.append(md_list)
+        logger.info("Added ordered list to document: %r", md_list)
         return md_list
 
     def add_unordered_list(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds an unordered list to the document.
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_unordered_list(["Deku", "Bakugo", "Kirishima"])
-            <snakemd.elements.MDList object at ...>
-            >>> str(doc)
-            '- Deku\\n- Bakugo\\n- Kirishima'
+            MDList(items=[...], ordered=False, checked=None)
+            >>> print(doc)
+            - Deku
+            - Bakugo
+            - Kirishima
 
-        :param Iterable[str] items: 
+        :param Iterable[str] items:
             a "list" of strings
-        :return: 
+        :return:
             the :class:`MDList` added to this Document
         """
         md_list = MDList(items)
-        self._contents.append(md_list)
-        logger.debug(f"Added unordered list to document\n{md_list}")
+        self._elements.append(md_list)
+        logger.info("Added unordered list to document: %r", md_list)
         return md_list
 
     def add_checklist(self, items: Iterable[str]) -> MDList:
         """
         A convenience method which adds a checklist to the document.
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_checklist(["Okabe", "Mayuri", "Kurisu"])
-            <snakemd.elements.MDList object at ...>
-            >>> str(doc)
-            '- [ ] Okabe\\n- [ ] Mayuri\\n- [ ] Kurisu'
+            MDList(items=[...], ordered=False, checked=False)
+            >>> print(doc)
+            - [ ] Okabe
+            - [ ] Mayuri
+            - [ ] Kurisu
 
-        :param Iterable[str] items: 
+        :param Iterable[str] items:
             a "list" of strings
-        :return: 
+        :return:
             the :class:`MDList` added to this Document
         """
         md_checklist = MDList(items, checked=False)
-        self._contents.append(md_checklist)
-        logger.debug(f"Added checklist to document\n{md_checklist}")
+        self._elements.append(md_checklist)
+        logger.info("Added checklist to document: %r", md_checklist)
         return md_checklist
 
     def add_table(
         self,
         header: Iterable[str],
         data: Iterable[Iterable[str]],
         align: Iterable[Table.Align] = None,
-        indent: int = 0
+        indent: int = 0,
     ) -> Table:
         """
         A convenience method which adds a table to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> header = ["Place", "Name"]
             >>> rows = [["1st", "Robert"], ["2nd", "Rae"]]
             >>> align = [snakemd.Table.Align.CENTER, snakemd.Table.Align.RIGHT]
             >>> doc.add_table(header, rows, align=align)
-            <snakemd.elements.Table object at ...>
-            >>> str(doc)
-            '| Place | Name   |\\n| :---: | -----: |\\n| 1st   | Robert |\\n| 2nd   | Rae    |'
+            Table(header=[...], body=[...], align=[...], indent=0)
+            >>> print(doc) # doctest: +NORMALIZE_WHITESPACE
+            | Place | Name   |
+            | :---: | -----: |
+            | 1st   | Robert |
+            | 2nd   | Rae    |
 
-        :param Iterable[str] header: 
+        :param Iterable[str] header:
             a "list" of strings
-        :param Iterable[Iterable[str]] data: 
+        :param Iterable[Iterable[str]] data:
             a "list" of "lists" of strings
-        :param Iterable[Table.Align] align: 
+        :param Iterable[Table.Align] align:
             a "list" of column alignment values;
             defaults to None
-        :param int indent: 
+        :param int indent:
             indent size for the whole table
-        :return: 
+        :return:
             the :class:`Table` added to this Document
         """
         header = [Paragraph([text]) for text in header]
         data = [[Paragraph([item]) for item in row] for row in data]
         table = Table(header, data, align, indent)
-        self._contents.append(table)
-        logger.debug(f"Added table to document\n{table}")
+        self._elements.append(table)
+        logger.info("Added table to document: %r", table)
         return table
 
     def add_code(self, code: str, lang: str = "generic") -> Code:
         """
         A convenience method which adds a code block to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_code("x = 5")
-            <snakemd.elements.Code object at ...>
-            >>> str(doc)
-            '```generic\\nx = 5\\n```'
+            Code(code='x = 5', lang='generic')
+            >>> print(doc)
+            ```generic
+            x = 5
+            ```
 
-        :param str code: 
+        :param str code:
             a preformatted code string
-        :param str lang: 
+        :param str lang:
             the language for syntax highlighting
-        :return: 
+        :return:
             the :class:`Code` block added to this Document
         """
         code_block = Code(code, lang=lang)
-        self._contents.append(code_block)
-        logger.debug(f"Added code block to document\n{code_block}")
+        self._elements.append(code_block)
+        logger.info("Added code block to document: %r", code_block)
         return code_block
 
     def add_quote(self, text: str) -> Quote:
         """
         A convenience method which adds a blockquote to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_quote("Welcome to the Internet!")
-            <snakemd.elements.Quote object at ...>
-            >>> str(doc)
-            '> Welcome to the Internet!'
+            Quote(content=[Raw(text='Welcome to the Internet!')])
+            >>> print(doc)
+            > Welcome to the Internet!
 
-        :param str text: 
+        :param str text:
             the text to be quoted
-        :return: 
+        :return:
             the :class:`Quote` added to this Document
         """
         quote = Quote(text)
-        self._contents.append(quote)
-        logger.debug(f"Added quote to document\n{quote}")
+        self._elements.append(quote)
+        logger.info("Added quote to document: %r", quote)
         return quote
 
     def add_horizontal_rule(self) -> HorizontalRule:
         """
         A convenience method which adds a horizontal rule to the document:
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_horizontal_rule()
-            <snakemd.elements.HorizontalRule object at ...>
-            >>> str(doc)
-            '***'
+            HorizontalRule()
+            >>> print(doc)
+            ***
 
-        :return: 
+        :return:
             the :class:`HorizontalRule` added to this Document
         """
-        hr = HorizontalRule()
-        self._contents.append(hr)
-        logger.debug(f"Added horizontal rule to document\n{hr}")
-        return hr
+        horizontal_rule = HorizontalRule()
+        self._elements.append(horizontal_rule)
+        logger.info("Added horizontal rule to document: %r", horizontal_rule)
+        return horizontal_rule
 
     def add_table_of_contents(self, levels: range = range(2, 3)) -> TableOfContents:
         """
         A convenience method which creates a table of contents. This function
         can be called where you want to add a table of contents to your
         document. The table itself is lazy loaded, so it always captures
         all of the heading blocks regardless of where the table of contents
         is added to the document.
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_table_of_contents()
-            <snakemd.templates.TableOfContents object at ...>
+            TableOfContents(levels=range(2, 3))
             >>> doc.add_heading("First Item", 2)
-            <snakemd.elements.Heading object at ...>
-            >>> doc.add_heading("Second Item", 2) 
-            <snakemd.elements.Heading object at ...>
-            >>> str(doc)
-            '1. [First Item](#first-item)\\n2. [Second Item](#second-item)\\n\\n## First Item\\n\\n## Second Item'
+            Heading(text=[Inline(text='First Item',...)], level=2)
+            >>> doc.add_heading("Second Item", 2)
+            Heading(text=[Inline(text='Second Item',...)], level=2)
+            >>> print(doc)
+            1. [First Item](#first-item)
+            2. [Second Item](#second-item)
+            <BLANKLINE>
+            ## First Item
+            <BLANKLINE>
+            ## Second Item
 
-        :param range levels: 
+        :param range levels:
             a range of heading levels to be included in the table of contents
-        :return: 
+        :return:
             the :class:`TableOfContents` added to this Document
         """
-        toc = TableOfContents(self, levels=levels)
-        self._contents.append(toc)
-        logger.debug(
-            f"Added table of contents to document (unable to render until file is complete)"
-        )
+        toc = TableOfContents(levels=levels)
+        self._elements.append(toc)
+        logger.info("Added table of contents to document: %r", toc)
         return toc
 
     def scramble(self) -> None:
         """
         A silly method which mixes all of the blocks in this document in
         a random order.
-        
+
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_horizontal_rule()
-            <snakemd.elements.HorizontalRule object at ...>
+            HorizontalRule()
             >>> doc.scramble()
-            >>> str(doc)
-            '***'
+            >>> print(doc)
+            ***
         """
-        random.shuffle(self._contents)
-        logger.debug(f"Scrambled document")
+        random.shuffle(self._elements)
+        logger.info("Scrambled document")
+
+    def dump(
+        self,
+        name: str,
+        directory: str | os.PathLike = "",
+        ext: str = "md",
+        encoding: str = "utf-8",
+    ) -> None:
+        """
+        Outputs the markdown document to a file. This method assumes the output
+        directory is the current working directory. Any alternative directory provided
+        will be made if it does not already exist. This method also assumes a file
+        extension of md and a file encoding of utf-8, all of which are configurable
+        through the method parameters.
 
-    def dump(self, name: str, dir: str | os.PathLike = "", ext: str = "md", encoding: str = "utf-8") -> None:
-        """
-        Outputs the markdown document to a file. This method assumes the output directory
-        is the current working directory. Any alternative directory provided will be
-        made if it does not already exist. This method also assumes a file extension of md
-        and a file encoding of utf-8, all of which are configurable through the method
-        parameters.
-        
         .. doctest:: document
-        
+
             >>> doc = snakemd.new_doc()
             >>> doc.add_horizontal_rule()
-            <snakemd.elements.HorizontalRule object at ...>
+            HorizontalRule()
             >>> doc.dump("README")
 
-        :param str name: 
+        :param str name:
             the name of the markdown file to output without the file extension
-        :param str | os.PathLike dir: 
+        :param str | os.PathLike directory:
             the output directory for the markdown file; defaults to ""
-        :param str ext: 
+
+            .. versionchanged:: 2.2
+                Renamed from dir to directory to avoid built-in clashes
+
+        :param str ext:
             the output file extension; defaults to "md"
-        :param str encoding: 
+        :param str encoding:
             the encoding to use; defaults to utf-8
         """
-        pathlib.Path(dir).mkdir(parents=True, exist_ok=True)
+        pathlib.Path(directory).mkdir(parents=True, exist_ok=True)
         with open(
-            os.path.join(dir, f"{name}.{ext}"),
-            "w+",
-            encoding=encoding
+            os.path.join(directory, f"{name}.{ext}"), "w+", encoding=encoding
         ) as output_file:
             output_file.write(str(self))
-        logger.debug(f"Dumped document to {dir} with filename {name}.{ext}")
+        logger.info("Dumped document to %s with filename %s.%s", directory, name, ext)
```

### Comparing `snakemd-2.1.0/snakemd/elements.py` & `snakemd-2.2.0b1/snakemd/elements.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+The Element module contains all of the possible
+elements that can be added to a Document.
+"""
+
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from typing import Iterable
 
@@ -9,496 +14,634 @@
 
 
 class Element(ABC):
     """
     A generic element interface which provides a framework for all
     types of elements in the collection. In short, elements must
     be able to be converted to their markdown representation using
-    the built-in :py:class:`str` constructor. 
+    the built-in :py:class:`str` constructor. They must also be
+    able to be converted into development strings using the
+    :py:func:`repr` function.
     """
 
     @abstractmethod
     def __str__(self) -> str:
         """
         The default string method to be implemented by all inheriting
-        classes. 
+        classes.
+
+        :return:
+            a markdown ready representation of the element
+        """
+
+    @abstractmethod
+    def __repr__(self) -> str:
+        """
+        The developer's string method to help make sense of
+        objects. As described by Digital Ocean, this method should
+        return a string that can be used to recreate the object.
+        This will not be true for every possible element as
+        there are internal structures as a result of
+        post-processing, but it should be more informative
+        than the default __repr__ method. Ultimately, this
+        method must be implemented by all inheriting classes.
 
-        :return: a string representation of the element
+        :return:
+            an unambiguous representation of the element
         """
 
 
 class Inline(Element):
     """
     The basic unit of text in markdown. All components which contain
     text are built using this class instead of strings directly. That
     way, those elements capture all styling information.
 
     Inline element parameters are in order of precedence. In other words,
     image markdown is applied to the text first while code markdown is
     applied last. Due to this design, some forms of inline text are not
-    possible. For example, inline elements can be used to show inline 
+    possible. For example, inline elements can be used to show inline
     markdown as an inline code element (e.g., :code:`![here](https://example.com)`).
-    However, inline elements cannot be used to style inline code (e.g., :code:`**`code`**`).
-    If styled code is necessary, it's possible to render the inline element
-    as a string and pass the result to another inline element. 
+    However, inline elements cannot be used to style inline code
+    (e.g., :code:`**`code`**`). If styled code is necessary, it's
+    possible to render the inline element as a string and pass the
+    result to another inline element.
 
     .. testsetup:: inline
-    
+
         from snakemd import Inline
 
-    :param str text: 
+    :param str text:
         the inline text to render
-    :param None | str image: 
+    :param None | str image:
         the source (either url or path) associated with an image
-        
+
         - defaults to :code:`None`
-        - set to a string representing a URL or path to render an image (i.e., :code:`![text](image)`)
-    :param None | str link: 
+        - set to a string representing a URL or path to render
+          an image (i.e., :code:`![text](image)`)
+    :param None | str link:
         the link (either url or path) associated with the inline element
-        
+
         - defaults to :code:`None`
-        - set to a string representing a URL or path to render a link (i.e., :code:`[text](link)`)
-    :param bool bold: 
+        - set to a string representing a URL or path to render a link
+          (i.e., :code:`[text](link)`)
+    :param bool bold:
         the bold state of the inline text
-        
+
         - defaults to :code:`False`
         - set to :code:`True` to render bold text (i.e., :code:`**text**`)
-    :param bool italics: 
+    :param bool italics:
         the italics state of the inline element
-        
+
         - defaults to :code:`False`
         - set to :code:`True` to render text in italics (i.e., :code:`_text_`)
-    :param bool strikethrough: 
+    :param bool strikethrough:
         the strikethrough state of the inline text
-        
+
         - defaults to :code:`False`
-        - set to :code:`True` to render text with a strikethrough 
+        - set to :code:`True` to render text with a strikethrough
           (i.e., :code:`~~text~~`)
-    :param bool code: 
+    :param bool code:
         the code state of the inline text
-        
+
         - defaults to :code:`False`
         - set to :code:`True` to render text as code (i.e., ```text```)
     """
 
     def __init__(
         self,
         text: str,
         image: None | str = None,
         link: None | str = None,
         bold: bool = False,
         italics: bool = False,
         strikethrough: bool = False,
-        code: bool = False
+        code: bool = False,
     ) -> None:
         self._text = text
         self._image = image
         self._link = link
         self._bold = bold
         self._italics = italics
         self._strikethrough = strikethrough
         self._code = code
 
     def __str__(self) -> str:
         """
-        Renders self as a string. In this case,
+        Renders self as a markdown ready string. In this case,
         inline can represent many different types of data from
         stylized text to code, links, and images.
-        
+
         .. doctest:: inline
 
             >>> inline = Inline("This is formatted text", bold=True, italics=True)
             >>> str(inline)
             '_**This is formatted text**_'
 
-        :return: 
-            the Inline object as a string
+        :return:
+            the Inline object as a markdown string
         """
         text = self._text
         if self._image:
             text = f"![{text}]({self._image})"
         if self._link:
             text = f"[{text}]({self._link})"
         if self._bold:
             text = f"**{text}**"
         if self._italics:
             text = f"_{text}_"
         if self._strikethrough:
             text = f"~~{text}~~"
         if self._code:
             text = f"`{text}`"
-        logger.debug(f"Rendered inline text: {text}")
+        logger.debug("Rendered inline text: %r", text)
         return text
 
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        :return:
+            the Inline object as a development string
+        """
+        return (
+            f"Inline("
+            f"text={self._text!r}, "
+            f"image={self._image!r}, "
+            f"link={self._link!r}, "
+            f"bold={self._bold!r}, "
+            f"italics={self._italics!r}, "
+            f"strikethrough={self._strikethrough!r}, "
+            f"code={self._code!r}"
+            ")"
+        )
+
     def is_text(self) -> bool:
         """
         Checks if this Inline element is a text-only element. If not, it must
         be an image, a link, or a code snippet.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is text")
             >>> inline.is_text()
             True
 
-        :return: 
+        :return:
             True if this is a text-only element; False otherwise
         """
         return not (self._code or self._image or self._link)
 
     def is_link(self) -> bool:
         """
         Checks if the Inline object represents a link.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is not a link")
             >>> inline.is_link()
             False
 
-        :return: 
+        :return:
             True if the object has a link; False otherwise
         """
         return bool(self._link)
 
+    def get_text(self) -> str:
+        """
+        Retrieves the text attribute of the Inline element.
+
+        .. doctest:: inline
+
+            >>> inline = Inline("This is text")
+            >>> inline.get_text()
+            'This is text'
+
+        .. versionadded:: 2.2
+            Included to avoid protected member access scenarios.
+
+        :return:
+            the text of the Inline element
+        """
+        return self._text
+
+    def get_link(self) -> str:
+        """
+        Retrieves the link attribute of the Inline element.
+
+        .. doctest:: inline
+
+            >>> inline = Inline("Here", link="https://snakemd.io")
+            >>> inline.get_link()
+            'https://snakemd.io'
+
+        .. versionadded:: 2.2
+            Included to avoid protected member access scenarios.
+
+        :return:
+            the link of the Inline element
+        """
+        return self._link
+
     def bold(self) -> Inline:
         """
         Adds bold styling to self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is bold text").bold()
-            >>> str(inline)
-            '**This is bold text**'
+            >>> print(inline)
+            **This is bold text**
 
-        :return: 
+        :return:
             self
         """
         self._bold = True
         return self
 
     def unbold(self) -> Inline:
         """
         Removes bold styling from self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is normal text", bold=True).unbold()
-            >>> str(inline)
-            'This is normal text'
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._bold = False
         return self
 
     def italicize(self) -> Inline:
         """
         Adds italics styling to self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is italicized text").italicize()
-            >>> str(inline)
-            '_This is italicized text_'
+            >>> print(inline)
+            _This is italicized text_
 
-        :return: 
+        :return:
             self
         """
         self._italics = True
         return self
 
     def unitalicize(self) -> Inline:
         """
         Removes italics styling from self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is normal text", italics=True).unitalicize()
-            >>> str(inline)
-            'This is normal text'
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._italics = False
         return self
 
     def strikethrough(self) -> Inline:
         """
         Adds strikethrough styling to self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is striked text").strikethrough()
-            >>> str(inline)
-            '~~This is striked text~~'
+            >>> print(inline)
+            ~~This is striked text~~
 
-        :return: 
+        :return:
             self
         """
         self._strikethrough = True
         return self
 
     def unstrikethrough(self) -> Inline:
         """
         Remove strikethrough styling from self.
 
         .. doctest:: inline
 
-            >>> inline = Inline("This is normal text", strikethrough=True).unstrikethrough()
-            >>> str(inline)
-            'This is normal text'
+            >>> inline = Inline("This is normal text", strikethrough=True)
+            >>> inline.unstrikethrough()
+            Inline(text='This is normal text',... strikethrough=False,...)
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._strikethrough = False
         return self
 
     def code(self) -> Inline:
         """
         Adds code style to self.
 
         .. doctest:: inline
 
             >>> inline = Inline("x = 5").code()
-            >>> str(inline)
-            '`x = 5`'
+            >>> print(inline)
+            `x = 5`
 
-        :return: 
+        :return:
             self
         """
         self._code = True
         return self
 
     def uncode(self) -> Inline:
         """
         Removes code styling from self.
 
         .. doctest:: inline
 
             >>> inline = Inline("This is normal text", code=True).uncode()
-            >>> str(inline)
-            'This is normal text'
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._code = False
         return self
 
     def link(self, link: str) -> Inline:
         """
         Adds link to self.
 
         .. doctest:: inline
 
             >>> inline = Inline("here").link("https://snakemd.io")
-            >>> str(inline)
-            '[here](https://snakemd.io)'
+            >>> print(inline)
+            [here](https://snakemd.io)
 
-        :param str link: 
+        :param str link:
             the URL or path to apply to this Inline element
-        :return: 
+        :return:
             self
         """
         self._link = link
         return self
 
     def unlink(self) -> Inline:
         """
         Removes link from self.
 
         .. doctest:: inline
 
-            >>> inline = Inline("This is normal text", link="https://snakemd.io").unlink()
-            >>> str(inline)
-            'This is normal text'
+            >>> inline = Inline("This is normal text", link="https://snakemd.io")
+            >>> inline.unlink()
+            Inline(text='This is normal text',... link=None,...)
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._link = None
         return self
 
     def reset(self) -> Inline:
         """
         Removes all settings from self (e.g., bold, code, italics, url, etc.).
         All that will remain is the text itself.
 
         .. doctest:: inline
 
-            >>> inline = Inline("This is normal text", link="https://snakemd.io", bold=True).reset()
-            >>> str(inline)
-            'This is normal text'
+            >>> inline = Inline(
+            ... "This is normal text",
+            ... link="https://snakemd.io",
+            ... bold=True
+            ... )
+            >>> inline.reset()
+            Inline(text='This is normal text',...)
+            >>> print(inline)
+            This is normal text
 
-        :return: 
+        :return:
             self
         """
         self._image = None
         self._link = None
         self._code = False
         self._italics = False
         self._bold = False
         self._strikethrough = False
         return self
 
 
-class Block(Element):
+class Block(Element):  # pylint: disable=too-few-public-methods
     """
-    A block element in Markdown. A block is defined as a standalone 
-    element starting on a newline. Examples of blocks include paragraphs 
-    (i.e., :code:`<p>`), headings (e.g., :code:`<h1>`, :code:`<h2>`, etc.), 
+    A block element in Markdown. A block is defined as a standalone
+    element starting on a newline. Examples of blocks include paragraphs
+    (i.e., :code:`<p>`), headings (e.g., :code:`<h1>`, :code:`<h2>`, etc.),
     tables (i.e., :code:`<table>`), and lists (e.g., :code:`<ol>`, :code:`<ul>`, etc.).
     """
-    pass
 
 
 class Code(Block):
     """
     A code block is a standalone block of syntax-highlighted code.
     Code blocks can have generic highlighting or highlighting based
-    on their language. 
-    
+    on their language.
+
+    .. testsetup:: code
+
+        from snakemd import Code
+
     :param str | Code code:
         the sourcecode to format as a Markdown code block
-        
-        - set to a string to render a preformatted code block (i.e., whitespace is respected)
+
+        - set to a string to render a preformatted code block
+          (i.e., whitespace is respected)
         - set to a Code object to render a nested code block
     :param str lang:
         the programming language for the code block; defaults to 'generic'
     """
 
     def __init__(self, code: str | Code, lang: str = "generic"):
-        super().__init__()
         self._code = code
         self._lang = lang
         self._backticks = self._process_backticks(code)
-        
+
     def __str__(self) -> str:
         """
         Renders the code block as a markdown string. Markdown code
         blocks are returned with the fenced code block
         format using backticks:
-        
+
         .. code-block:: markdown
-        
+
             ```python
             x = 5
             y = 2 + x
             ```
-            
+
         Code blocks can be nested and will be rendered with
         increasing numbers of backticks.
 
-        :return: 
+        :return:
             the code block as a markdown string
         """
-        ticks = '`' * self._backticks
-        return f"{ticks}{self._lang}\n{self._code}\n{ticks}"
-    
+        ticks = "`" * self._backticks
+        code_block = f"{ticks}{self._lang}\n{self._code}\n{ticks}"
+        logger.debug("Rendered code block: %r", code_block)
+        return code_block
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        .. doctest:: code
+
+            >>> code = Code('x = 87')
+            >>> repr(code)
+            "Code(code='x = 87', lang='generic')"
+
+        :return:
+            the Code object as a development string
+        """
+        return f"Code(code={self._code!r}, lang={self._lang!r})"
+
     @staticmethod
     def _process_backticks(code: str | Code) -> int:
         """
         A helper method which processes the potential hierarchy
         that exists for code.
 
         :param code: code to render
         :return: the number of appropriate backticks for this code block
         """
         if isinstance(code, Code):
-            return code._backticks + 1
-        else:
-            return 3
-    
-    
+            return code._backticks + 1  # pylint: disable=protected-access
+        return 3
+
+
 class Heading(Block):
     """
     A heading is a text block which serves as the title for a new
     section of a document. Headings come in six main sizes which
     correspond to the six headings sizes in HTML (e.g., :code:`<h1>`).
-    
+
     .. testsetup:: heading
-    
+
         from snakemd import Heading
 
-    :raises ValueError: 
+    :raises ValueError:
         when level < 1 or level > 6
-    :param str | Inline | Iterable[Inline | str] text: 
+    :param str | Inline | Iterable[Inline | str] text:
         the heading text
-        
+
         - set to a string to render raw heading text
-        - set to an Inline object to render a styled heading (e.g., bold, link, code, etc.)
-        - set to a "list" of the prior options to render a header with more granular 
+        - set to an Inline object to render a styled heading
+          (e.g., bold, link, code, etc.)
+        - set to a "list" of the prior options to render a
+          header with more granular
           control over the individual inline elements
-    :param int level: 
+    :param int level:
         the heading level between 1 and 6
     """
 
     def __init__(self, text: str | Inline | Iterable[Inline | str], level: int) -> None:
         if level < 1 or level > 6:
-            raise ValueError(
-                f"Heading level must be between 1 and 6 but was {level}"
-            )
-        super().__init__()
+            raise ValueError(f"Heading level must be between 1 and 6 but was {level}")
         self._text: list[Inline] = self._process_text(text)
         self._level: int = level
+        logger.debug("Created new heading: %r", self)
 
     def __str__(self) -> str:
         """
         Renders the heading as a markdown string. Markdown headings
         are returned using the :code:`#` syntax where the number of
         :code:`#` symbols corresponds to the heading level:
-        
+
         .. code-block:: markdown
-        
+
             # This is an H1
             ## This is an H2
             ### This is an H3
 
-        :return: 
+        :return:
             the heading as a markdown string
         """
         heading = [str(item) for item in self._text]
-        return f"{'#' * self._level} {''.join(heading)}"
+        heading = f"{'#' * self._level} {''.join(heading)}"
+        logger.debug("Rendered heading: %r", heading)
+        return heading
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        Note that Headings can accept a variety of string-like
+        inputs. However, the underlying representation forces
+        all possible inputs to be a list of Inline objects.
+        As a result, the repr representation will often be
+        significantly more complex than expected.
+
+        .. doctest:: heading
+
+            >>> heading = Heading("", 1)
+            >>> repr(heading)
+            "Heading(text=[Inline(text='',...)], level=1)"
+
+        :return:
+            the Code object as a development string
+        """
+        return f"Heading(text={self._text!r}, level={self._level})"
 
     @staticmethod
     def _process_text(text: str | Inline | Iterable[Inline | str]) -> list[Inline]:
         """
         Ensures that Heading objects are composed of a single Inline object.
 
-        :param str | Inline | Iterable[Inline | str] text: 
+        :param str | Inline | Iterable[Inline | str] text:
             an object to be forced to Inline
-        :return: 
+        :return:
             the input text as an Inline
         """
-        logger.debug(f"Processing heading text: {text}")
         if isinstance(text, str):
-            return [Inline(text)]
+            processed = [Inline(text)]
         elif isinstance(text, Inline):
-            return [text]
+            processed = [text]
         else:
-            return [
-                item if isinstance(item, Inline) else Inline(item)
-                for item in text
+            processed = [
+                item if isinstance(item, Inline) else Inline(item) for item in text
             ]
+        logger.debug("Processed heading text: %r", processed)
+        return processed
 
     def promote(self) -> Heading:
         """
         Promotes a heading up a level. Fails silently
         if the heading is already at the highest level (i.e., :code:`<h1>`).
-        
+
         .. doctest:: heading
 
             >>> heading = Heading("This is an H2 heading", 3).promote()
             >>> str(heading)
             '## This is an H2 heading'
-            
+
         :return:
             self
         """
         if self._level > 1:
             self._level -= 1
         return self
 
@@ -508,15 +651,15 @@
         the heading is already at the lowest level (i.e., :code:`<h6>`).
 
         .. doctest:: heading
 
             >>> heading = Heading("This is an H2 heading", 1).demote()
             >>> str(heading)
             '## This is an H2 heading'
-            
+
         :return:
             self
         """
         if self._level < 6:
             self._level += 1
         return self
 
@@ -528,111 +671,161 @@
 
         .. doctest:: heading
 
             >>> heading = Heading("This is the heading text", 1)
             >>> heading.get_text()
             'This is the heading text'
 
-        :return: 
+        :return:
             the heading as a string
         """
-        text_elements = [item._text for item in self._text]
-        return ''.join(text_elements)
+        text_elements = [item.get_text() for item in self._text]
+        return "".join(text_elements)
+
+    def get_level(self) -> int:
+        """
+        Retrieves the level of the heading.
+
+        .. doctest:: heading
+
+            >>> heading = Heading("This is the heading text", 1)
+            >>> heading.get_level()
+            1
+
+        .. versionadded:: 2.2
+            Included to avoid protected member access scenarios.
+
+        :return:
+            the heading level
+        """
+        return self._level
 
 
 class HorizontalRule(Block):
     """
     A horizontal rule is a line separating different sections of
     a document. Horizontal rules only come in one form,
     so there are no settings to adjust.
-    """
 
-    def __init__(self):
-        super().__init__()
+    .. testsetup:: horizontalrule
+
+        from snakemd import HorizontalRule
+    """
 
     def __str__(self) -> str:
         """
         Renders the horizontal rule as a markdown string. Markdown
         horizontal rules come in a variety of flavors, but the
-        format used in this repo is the triple asterisk 
+        format used in this repo is the triple asterisk
         (i.e., :code:`***`) to avoid clashes with list formatting.
 
-        :return: 
+        :return:
             the horizontal rule as a markdown string
         """
-        return "***"
-    
-    
+        horizontal_rule = "***"
+        logger.debug("Rendered horizontal rule: %r", horizontal_rule)
+        return horizontal_rule
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        .. doctest:: horizontalrule
+
+            >>> horizontal_rule = HorizontalRule()
+            >>> repr(horizontal_rule)
+            'HorizontalRule()'
+
+        :return:
+            the HorizontalRule object as a development string
+        """
+        return "HorizontalRule()"
+
+
 class MDList(Block):
     """
-    A markdown list is a standalone list that comes in three varieties: ordered, unordered, and checked.
+    A markdown list is a standalone list that comes in three varieties: ordered,
+    unordered, and checked.
+
+    .. testsetup:: mdlist
+
+        from snakemd import MDList
 
-    :raises ValueError: 
-        when the checked argument is an Iterable[bool] that does not 
+    :raises ValueError:
+        when the checked argument is an Iterable[bool] that does not
         match the number of top-level elements in the list
     :param Iterable[str | Inline | Block] items:
         a "list" of objects to be rendered as a list
-    :param bool ordered: 
+    :param bool ordered:
         the ordered state of the list
-        
+
         - defaults to :code:`False` which renders an unordered list (i.e., :code:`-`)
         - set to :code:`True` to render an ordered list (i.e., :code:`1.`)
-    :param None | bool | Iterable[bool] checked: 
+    :param None | bool | Iterable[bool] checked:
         the checked state of the list
-        
-        - defaults to :code:`None` which excludes checkboxes from being rendered
-        - set to :code:`False` to render a series of unchecked boxes (i.e., :code:`- [ ]`)
-        - set to :code:`True` to render a series of checked boxes (i.e., :code:`- [x]`)
-        - set to :code:`Iterable[bool]` to render the checked 
+
+        - defaults to :code:`None` which excludes checkboxes from
+          being rendered
+        - set to :code:`False` to render a series of unchecked boxes
+          (i.e., :code:`- [ ]`)
+        - set to :code:`True` to render a series of checked boxes
+          (i.e., :code:`- [x]`)
+        - set to :code:`Iterable[bool]` to render the checked
           status of the top-level list elements directly
     """
 
     def __init__(
         self,
         items: Iterable[str | Inline | Block],
         ordered: bool = False,
-        checked: None | bool | Iterable[bool] = None
+        checked: None | bool | Iterable[bool] = None,
     ) -> None:
-        super().__init__()
         self._items: list[Block] = self._process_items(items)
         self._ordered: bool = ordered
-        self._checked: bool | list[bool] = checked \
-            if checked is None or isinstance(checked, bool) \
-            else [_ for _ in checked]
+        self._checked: bool | list[bool] = (
+            checked if checked is None or isinstance(checked, bool) else list(checked)
+        )
         self._space = ""
-        if isinstance(self._checked, list) and self._top_level_count() != len(self._checked):
+        if isinstance(self._checked, list) and self._top_level_count() != len(
+            self._checked
+        ):
             raise ValueError(
-                f"Number of top-level elements in checklist does not match number of booleans supplied by checked parameter: {self._checked}"
+                "Number of top-level elements in checklist does not "
+                "match number of booleans supplied by checked parameter: "
+                f"{self._checked}"
             )
 
     def __str__(self) -> str:
         """
         Renders the markdown list as a markdown string. Markdown lists
-        come in a variety of flavors and are customized according to 
-        the settings provided. For example, if the the ordered flag is 
+        come in a variety of flavors and are customized according to
+        the settings provided. For example, if the the ordered flag is
         set, an ordered list will be rendered in markdown. Unordered
         lists and checklists both use the hyphen syntax for markdown
-        (i.e., :code:`-`) to avoid clashes with horizontal rules: 
-        
+        (i.e., :code:`-`) to avoid clashes with horizontal rules:
+
         .. code-block:: markdown
-        
+
             - This is an unordered list item
             - So, is this
-        
+
         Ordered lists use numbers for each list item:
-        
+
         .. code-block:: markdown
-        
+
             1. This is an ordered list item
             2. So, is this
 
-        :return: 
+        :return:
             the list as a markdown string
         """
-        output = list()
+        output = []
         i = 1
         for item in self._items:
             if isinstance(item, MDList):
                 item._space = self._space + " " * self._get_indent_size(i)
                 output.append(str(item))
             else:
                 # Create the start of the row based on `order` parameter
@@ -649,580 +842,658 @@
                     checked_str = "X" if self._checked[i - 1] else " "
                     row = f"{row} [{checked_str}] {item}"
                 else:
                     row = f"{row} {item}"
 
                 output.append(row)
                 i += 1
-        return "\n".join(output)
+        mdlist = "\n".join(output)
+        logger.debug("Rendered markdown list: %r", mdlist)
+        return mdlist
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        .. doctest:: mdlist
+
+            >>> mdlist = MDList(["Plus", "Ultra"])
+            >>> repr(mdlist)
+            "MDList(items=[Paragraph(...), Paragraph(...)],...)"
+
+        :return:
+            the MDList object as a development string
+        """
+        return (
+            f"MDList("
+            f"items={self._items!r}, "
+            f"ordered={self._ordered!r}, "
+            f"checked={self._checked!r}"
+            f")"
+        )
 
     @staticmethod
     def _process_items(items) -> list[Block]:
         """
         Given the variety of data that MDList can accept, this function
         forces all possible data types to be Blocks.
 
-        :param items: 
+        :param items:
             a list of items
-        :return: 
+        :return:
             a list of Blocks
         """
         processed = []
         for item in items:
             if isinstance(item, (str, Inline)):
                 processed.append(Paragraph([item]))
             else:
                 processed.append(item)
         return processed
-    
+
     def _top_level_count(self) -> int:
         """
         Given that MDList can accept a variety of blocks,
         we need to know how many items in the provided list
         are top-level elements (i.e., not nested list elements).
         We use this number to throw errors if this count does
         not match up with the checklist count.
 
-        :return: 
+        :return:
             a count of top-level elements
         """
         count = 0
         for item in self._items:
             if not isinstance(item, MDList):
                 count += 1
         return count
 
     def _get_indent_size(self, item_index: int = -1) -> int:
         """
         Returns the number of spaces that any sublists should be indented.
 
-        :param int item_index: 
+        :param int item_index:
             the index of the item to check (only used for ordered lists);
             defaults to -1
-        :return: 
+        :return:
             the number of spaces
         """
         if not self._ordered:
             return 2
-        else:
-            # Ordered items vary in length, so we adjust the result based on the index
-            return 2 + len(str(item_index))
+        # Ordered items vary in length, so we adjust the result based on the index
+        return 2 + len(str(item_index))
 
 
 class Paragraph(Block):
     """
-    A paragraph is a standalone block of text. 
-    
+    A paragraph is a standalone block of text.
+
     .. testsetup:: paragraph
-    
+
         from snakemd import Paragraph
 
-    :param str | Iterable[str | Inline] content: 
+    :param str | Iterable[str | Inline] content:
         the text to be rendered as a paragraph where whitespace is not respected
         (see :class:`snakemd.Raw` for whitespace sensitive applications)
-        
+
         - set to a string to render a single line of unformatted text
-        - set to a "list" of text objects to render a paragraph with more 
+        - set to a "list" of text objects to render a paragraph with more
           granular control over the individual text objects (e.g., linking,
-          styling, etc.)     
+          styling, etc.)
     """
 
     def __init__(self, content: str | Iterable[str | Inline]):
-        super().__init__()
         self._content: list[Inline] = self._process_content(content)
 
+    def __str__(self) -> str:
+        """
+        Renders the paragraph as a markdown string. Markdown paragraphs
+        are returned as a singular line of text with all of the
+        underlying elements rendered as expected:
+
+        .. code-block:: markdown
+
+            This is an example of a **paragraph** with _formatting_
+
+        :return:
+            the paragraph as a markdown string
+        """
+        paragraph = "".join(str(item) for item in self._content)
+        return " ".join(paragraph.split())
+
+    def __repr__(self) -> str:
+        """
+        Renders self as an unambiguous string for development.
+        In this case, it displays in the style of a dataclass,
+        where instance variables are listed with their
+        values.
+
+        Like Heading, the actual format of the development
+        string may be more complex than expected. Specifically,
+        all of the contents are automatically converted to
+        a list of Inline objects.
+
+        .. doctest:: paragraph
+
+            >>> paragraph = Paragraph("Howdy!")
+            >>> repr(paragraph)
+            "Paragraph(content=[Inline(text='Howdy!',...)])"
+
+        :return:
+            the Paragraph object as a development string
+        """
+        return f"Paragraph(content={self._content!r})"
+
     @staticmethod
     def _process_content(content) -> list[Inline]:
         """
         Processes the incoming content for the Paragraph.
 
-        :param content: 
+        :param content:
             an iterable of various text items
-        :return: 
+        :return:
             the processed iterable as a list of Inline items
         """
-        logger.debug(f"Processing paragraph content: {content}")
+
         if isinstance(content, str):
             processed = [Inline(content)]
         else:
             processed = []
             for item in content:
                 if isinstance(item, str):
                     processed.append(Inline(item))
                 else:
                     processed.append(item)
+        logger.debug("Processed paragraph content: %r", processed)
         return processed
 
-    def __str__(self) -> str:
-        """
-        Renders the paragraph as a markdown string. Markdown paragraphs
-        are returned as a singular line of text with all of the
-        underlying elements rendered as expected:
-        
-        .. code-block:: markdown
-        
-            This is an example of a **paragraph** with _formatting_
-
-        :return: 
-            the paragraph as a markdown string
-        """
-        paragraph = ''.join(str(item) for item in self._content)
-        return " ".join(paragraph.split())
-
-    def add(self, text: str | Inline) -> Paragraph:
-        """
-        Adds a text object to the paragraph.
-        
-        .. doctest:: paragraph
-        
-            >>> paragraph = Paragraph("Hello! ").add("I come in peace")
-            >>> str(paragraph)
-            'Hello! I come in peace'
-
-        :param str | Inline text: 
-            a custom Inline element
-        :return:
-            self
-        """
-        if isinstance(text, str):
-            text = Inline(text)
-        self._content.append(text)
-        return self
-
     def _replace_any(self, target: str, text: Inline, count: int = -1) -> Paragraph:
         """
         Given a target string, this helper method replaces it with the specified
         Inline object. This method was created because insert_link and
         replace were literally one line different. This method serves as the
         mediator. Note that using this method will introduce several new
         underlying Inline objects even if they could be aggregated.
         At some point, we may just expose this method because it seems handy.
         For example, I foresee a need for a function where all the person wants
         to do is add italics for every instance of a particular string.
         Though, I suppose we could include all of that in the default replace
         method.
 
-        :param str target: 
+        :param str target:
             the target string to replace
-        :param Inline text: 
+        :param Inline text:
             the Inline object to insert in place of the target
-        :param int count: 
+        :param int count:
             the number of links to insert; defaults to -1
-        :return: 
+        :return:
             self
         """
         i = 0
         content = []
         for inline_text in self._content:
-            if inline_text.is_text() and len(items := inline_text._text.split(target)) > 1:
+            if (
+                inline_text.is_text()
+                and len(items := inline_text.get_text().split(target)) > 1
+            ):
                 for item in items:
                     content.append(Inline(item))
                     if count == -1 or i < count:
                         content.append(text)
                         i += 1
                     else:
                         content.append(Inline(target))
                 content.pop()
             else:
                 content.append(inline_text)
         self._content = content
         return self
 
+    def add(self, text: str | Inline) -> Paragraph:
+        """
+        Adds a text object to the paragraph.
+
+        .. doctest:: paragraph
+
+            >>> paragraph = Paragraph("Hello! ").add("I come in peace")
+            >>> str(paragraph)
+            'Hello! I come in peace'
+
+        :param str | Inline text:
+            a custom Inline element
+        :return:
+            self
+        """
+        if isinstance(text, str):
+            text = Inline(text)
+        self._content.append(text)
+        return self
+
     def replace(self, target: str, replacement: str, count: int = -1) -> Paragraph:
         """
         A convenience method which replaces a target string with a string of
         the users choice. Like :meth:`insert_link`, this method is modeled after
         :py:meth:`str.replace` of the standard library. As a result, a count
         can be provided to limit the number of strings replaced in the paragraph.
-        
+
         .. doctest:: paragraph
-        
+
             >>> paragraph = Paragraph("I come in piece").replace("piece", "peace")
             >>> str(paragraph)
             'I come in peace'
 
-        :param str target: 
+        :param str target:
             the target string to replace
-        :param str replacement: 
+        :param str replacement:
             the string to insert in place of the target
-        :param int count: 
+        :param int count:
             the number of targets to replace; defaults to -1 (all)
-        :return: 
+        :return:
             self
         """
         return self._replace_any(target, Inline(replacement), count)
 
     def insert_link(self, target: str, link: str, count: int = -1) -> Paragraph:
         """
         A convenience method which inserts links in the paragraph
         for all matching instances of a target string. This method
         is modeled after :py:meth:`str.replace`, so a count can be
         provided to limit the number of insertions. This method
         will not replace links of text that have already been linked.
         See :meth:`snakemd.Paragraph.replace_link` for that behavior.
-        
+
         .. doctest:: paragraph
-        
-            >>> paragraph = Paragraph("Go here for docs").insert_link("here", "https://snakemd.io")
+
+            >>> paragraph = Paragraph("Go here for docs")
+            >>> paragraph.insert_link("here", "https://snakemd.io")
+            Paragraph(content=[...])
             >>> str(paragraph)
             'Go [here](https://snakemd.io) for docs'
 
-        :param str target: 
+        :param str target:
             the string to link
-        :param str link: 
+        :param str link:
             the url or path
-        :param int count: 
+        :param int count:
             the number of links to insert; defaults to -1 (all)
-        :return: 
+        :return:
             self
         """
         return self._replace_any(target, Inline(target, link=link), count)
 
-    def replace_link(self, target_link: str, replacement_link: str, count: int = -1) -> Paragraph:
+    def replace_link(
+        self, target_link: str, replacement_link: str, count: int = -1
+    ) -> Paragraph:
         """
         A convenience method which replaces matching URLs in the paragraph with
         a new url. Like :meth:`insert_link` and :meth:`replace`, this method is also
         modeled after :py:meth:`str.replace`, so a count can be provided to limit
         the number of links replaced in the paragraph. This method is useful
         if you want to replace existing URLs but don't necessarily care what
         the anchor text is.
-        
+
         .. doctest:: paragraph
-        
+
             >>> old = "https://therenegadecoder.com"
             >>> new = "https://snakemd.io"
-            >>> paragraph = Paragraph("Go here for docs").insert_link("here", old).replace_link(old, new) 
+            >>> paragraph = Paragraph("Go here for docs")
+            >>> paragraph.insert_link("here", old).replace_link(old, new)
+            Paragraph(content=[...])
             >>> str(paragraph)
             'Go [here](https://snakemd.io) for docs'
 
-        :param str target_link: 
+        :param str target_link:
             the link to replace
-        :param str replacement_link: 
+        :param str replacement_link:
             the link to swap in
-        :param int count: 
+        :param int count:
             the number of links to replace; defaults to -1 (all)
-        :return: 
+        :return:
             self
         """
         i = 0
         for text in self._content:
-            if (count == -1 or i < count) and text._link == target_link:
+            if (count == -1 or i < count) and text.get_link() == target_link:
                 text.link(replacement_link)
                 i += 1
         return self
-    
-    
+
+
 class Quote(Block):
     """
     A quote is a standalone block of emphasized text. Quotes can be
-    nested and can contain other blocks. 
+    nested and can contain other blocks.
 
     :param str | Iterable[str | Inline | Block] content:
         the text to be formatted as a Markdown quote
-         
-        - set to a string to render a whitespace respected quote (similar to :class:`snakemd.Code`)
+
+        - set to a string to render a whitespace respected quote
+          (similar to :class:`snakemd.Code`)
         - set to a "list" of text objects to render a document-like quote
           (i.e., all items will be separated by newlines)
     """
 
     def __init__(self, content: str | Iterable[str | Inline | Block]) -> None:
-        super().__init__()
         self._lines: list[Block] = self._process_content(content)
         self._depth = 1
 
-    @staticmethod
-    def _process_content(lines) -> list[Block]:
-        """
-        Converts the raw input lines to something that is
-        a bit easier to work with. In this case, the lines
-        are converted to blocks.
-
-        :param lines: 
-            a "list" of text objects or a string
-        :return: 
-            a list of Blocks
-        """
-        logger.debug(f"Processing quote lines: {lines}")
-        if isinstance(lines, str):
-            processed_lines = [Raw(lines)]
-        else:
-            processed_lines = []
-            for line in lines:
-                if isinstance(line, (str, Inline)):
-                    processed_lines.append(Raw(line))
-                else:
-                    processed_lines.append(line)
-        return processed_lines
-
     def __str__(self) -> str:
         """
         Renders the quote as a markdown string. Markdown quotes
         vary in syntax, but the general approach in this repo is
         to apply the quote symbol (i.e., :code:`>`) to the front
         of each line in the quote:
-        
+
         .. code-block:: markdown
-        
+
             > this
             > is
             > a quote
-            
+
         Quotes can also be nested. To make this possible, nested
         quotes are padded by empty quote lines:
-        
+
         .. code-block:: markdown
-        
+
             > Outer quote
-            > 
+            >
             > > Inner quote
             >
             > Outer quote
-            
+
         It's unclear what is the correct way to handle nested
         quotes, but this format seems to be the most friendly
         for GitHub markdown. Future work may involve including
-        the option to removing the padding. 
+        the option to removing the padding.
 
-        :return: 
+        :return:
             the quote formatted as a markdown string
         """
         formatted_lines: list[str] = []
         quote_markers = f"{'> ' * self._depth}"
         for line in self._lines:
             if isinstance(line, Quote):
-                line._depth = self._depth + 1
-                formatted_lines.extend([
-                    quote_markers,
-                    str(line),
-                    quote_markers
-                ])
+                line._depth = self._depth + 1  # pylint: disable=W0201
+                formatted_lines.extend([quote_markers, str(line), quote_markers])
             else:
                 split = f"\n{quote_markers}".join(str(line).splitlines())
                 formatted_lines.append(f"{quote_markers}{split}")
         return "\n".join(formatted_lines)
 
+    def __repr__(self) -> str:
+        return f"Quote(content={self._lines!r})"
+
+    @staticmethod
+    def _process_content(lines) -> list[Block]:
+        """
+        Converts the raw input lines to something that is
+        a bit easier to work with. In this case, the lines
+        are converted to blocks.
+
+        :param lines:
+            a "list" of text objects or a string
+        :return:
+            a list of Blocks
+        """
+        if isinstance(lines, str):
+            processed_lines = [Raw(lines)]
+        else:
+            processed_lines = []
+            for line in lines:
+                if isinstance(line, (str, Inline)):
+                    processed_lines.append(Raw(line))
+                else:
+                    processed_lines.append(line)
+        logger.debug("Processed quote lines: %r", processed_lines)
+        return processed_lines
+
 
 class Raw(Block):
     """
     Raw blocks allow a user to insert text into a Markdown
     document without any processing. Use this block to insert
     raw Markdown or other types of text (e.g., Jekyll frontmatter)
     into a document.
-    
+
     :param str text: the raw text to append to a Document
     """
 
     def __init__(self, text: str) -> None:
-        super().__init__()
         self._text = text
 
     def __str__(self) -> str:
         """
-        Renders the raw block as a markdown string. 
+        Renders the raw block as a markdown string.
         Raw markdown is unprocessed and passes directly
-        through to the document. 
+        through to the document.
 
         :return: the raw block as a markdown string
         """
         return self._text
 
+    def __repr__(self) -> str:
+        return f"Raw(text={self._text!r})"
+
 
 class Table(Block):
     """
     A table is a standalone block of rows and columns. Data is rendered
     according to underlying Inline items.
-    
+
     .. testsetup:: table
-    
+
         from snakemd import Table
 
-    :raises ValueError: 
-    
+    :raises ValueError:
+
         - when rows of table are of varying lengths
         - when lengths of header and rows of table do not match
-    :param Iterable[str | Inline | Paragraph] header: 
+    :param Iterable[str | Inline | Paragraph] header:
         the header row of labels
-    :param Iterable[Iterable[str | Inline | Paragraph]] body: 
+    :param Iterable[Iterable[str | Inline | Paragraph]] body:
         the collection of rows of data; defaults to an empty list
-    :param None | Iterable[Align] align: 
+    :param None | Iterable[Align] align:
         the column alignment; defaults to None
-    :param int indent: 
+    :param int indent:
         indent size for the whole table; defaults to 0
     """
 
+    class Align(Enum):
+        """
+        Align is an enum only used by the Table class to specify the alignment
+        of various columns in the table.
+        """
+
+        LEFT = auto()
+        RIGHT = auto()
+        CENTER = auto()
+
     def __init__(
         self,
         header: Iterable[str | Inline | Paragraph],
-        body: Iterable[Iterable[str | Inline | Paragraph]] = [],
+        body: Iterable[Iterable[str | Inline | Paragraph]] = None,
         align: None | Iterable[Align] = None,
-        indent: int = 0
+        indent: int = 0,
     ) -> None:
-        logger.debug(f"Initializing table\n{(header, body, align)}")
-        super().__init__()
+        logger.debug("Initializing table: (%r, %r, %r)", header, body, align)
         self._header: list[Paragraph]
         self._body: list[list[Paragraph]]
-        self._header, self._body = self._process_table(header, body)
-        if len(self._body) > 1 and not all([len(self._body[0]) == len(x) for x in self._body[1:]]):
+        self._header, self._body = self._process_table(header, body or [])
+        if len(self._body) > 1 and not all(
+            len(self._body[0]) == len(x) for x in self._body[1:]
+        ):
             raise ValueError("Table rows are not all the same length")
-        elif body and len(self._header) != len(self._body[0]):
+        if body and len(self._header) != len(self._body[0]):
             raise ValueError("Table header and rows have different lengths")
-        self._widths: list[int] = self._process_widths(
-            self._header,
-            self._body
-        )
+        self._widths: list[int] = self._process_widths(self._header, self._body)
         self._align = align
         self._indent = indent
 
     def __str__(self) -> str:
         """
         Renders the table as a markdown string. Table markdown
         follows the standard pipe syntax:
-        
-        .. code-block:: 
+
+        .. code-block::
 
             | Header 1 | Header 2 |
             | -------- | -------- |
             | Item 1A  | Item 2A  |
             | Item 1B  | Item 2B  |
-            
+
         Alignment code adds colons in the appropriate locations.
         Final tables are rendered according to the widest
         items in each column for readability.
 
-        :return: 
+        :return:
             a table as a markdown string
         """
-        rows = list()
+        rows = []
         header = [
-            str(item).ljust(self._widths[i])
-            for i, item in enumerate(self._header)
+            str(item).ljust(self._widths[i]) for i, item in enumerate(self._header)
         ]
         body = [
             [str(item).ljust(self._widths[i]) for i, item in enumerate(row)]
             for row in self._body
         ]
         rows.append(f"{' ' * self._indent}| {' | '.join(header)} |")
         if not self._align:
-            rows.append(
-                f"{' ' * self._indent}| {' | '.join('-' * width for width in self._widths)} |")
+            dashes = " | ".join("-" * width for width in self._widths)
+            rows.append(f"{' ' * self._indent}| {dashes} |")
         else:
             meta = []
             for align, width in zip(self._align, self._widths):
                 if align == Table.Align.LEFT:
                     meta.append(f":{'-' * (width - 1)}")
                 elif align == Table.Align.RIGHT:
                     meta.append(f"{'-' * (width - 1)}:")
                 else:
                     meta.append(f":{'-' * (width - 2)}:")
             rows.append(f"{' ' * self._indent}| {' | '.join(meta)} |")
-        rows.extend(
-            (f"{' ' * self._indent}| {' | '.join(row)} |" for row in body))
-        return '\n'.join(rows)
+        rows.extend((f"{' ' * self._indent}| {' | '.join(row)} |" for row in body))
+        return "\n".join(rows)
 
-    class Align(Enum):
-        """
-        Align is an enum only used by the Table class to specify the alignment
-        of various columns in the table.
-        """
-        LEFT = auto()
-        RIGHT = auto()
-        CENTER = auto()
+    def __repr__(self) -> str:
+        return (
+            f"Table("
+            f"header={self._header!r}, "
+            f"body={self._body!r}, "
+            f"align={self._align!r}, "
+            f"indent={self._indent}"
+            f")"
+        )
 
     @staticmethod
-    def _process_table(header, body) -> tuple(list[Paragraph], list[list[Paragraph]], list[int]):
-        """
-        Processes the table inputs to ensure header and body only contain paragraph blocks.
-        Also, this computes the max width of each row to ensure pretty print works every time.
+    def _process_table(
+        header, body
+    ) -> tuple(list[Paragraph], list[list[Paragraph]], list[int]):
+        """
+        Processes the table inputs to ensure header and body only contain paragraph
+        blocks.
+        Also, this computes the max width of each row to ensure pretty print works every
+        time.
 
-        :param header: 
+        :param header:
             the header row in its various forms
-        :param body: 
+        :param body:
             the table body in its various forms
-        :return: 
-            the table containing only Paragraph blocks and a list of the widest items in each row
+        :return:
+            the table containing only Paragraph blocks and
+            a list of the widest items in each row
         """
         processed_header = []
         processed_body = []
 
         # Process header
         for item in header:
             if isinstance(item, (str, Inline)):
                 processed_header.append(Paragraph([item]))
             else:
                 processed_header.append(item)
-        logger.debug(f"Processed header input\n{processed_header}")
+        logger.debug("Processed header input: %r", processed_header)
 
         # Process body
         for row in body:
             processed_row = []
             for item in row:
                 if isinstance(item, (str, Inline)):
                     processed_row.append(Paragraph([item]))
                 else:
                     processed_row.append(item)
             processed_body.append(processed_row)
-        logger.debug(f"Processed table body\n{processed_body}")
+        logger.debug("Processed table body: %r", processed_body)
 
         return processed_header, processed_body
 
     @staticmethod
     def _process_widths(header, body) -> list[int]:
         """
         Traverses the table looking to determine the appropriate
-        widths for each column. 
+        widths for each column.
 
-        :param header: 
+        :param header:
             the header row
-        :param body: 
+        :param body:
             the rows of data
-        :return: 
+        :return:
             a list of column widths
         """
         widths = [len(str(word)) for word in header]
         for row in body:
             for i, item in enumerate(row):
                 if (width := len(str(item))) > widths[i]:
                     widths[i] = width
         return widths
 
     def add_row(self, row: Iterable[str | Inline | Paragraph]) -> Table:
         """
         A convenience method which adds a row to the end of table.
         Use this method to build a table row-by-row rather than constructing
-        the table rows upfront.  
-        
+        the table rows upfront.
+
         .. doctest:: table
-        
-            >>> table = Table(["Rank", "Player"], [["1st", "Crosby"], ["2nd", "McDavid"]])
+
+            >>> table = Table(
+            ... ["Rank", "Player"],
+            ... [["1st", "Crosby"], ["2nd", "McDavid"]]
+            ... )
             >>> table.add_row(["3rd", "Matthews"])
-            <snakemd.elements.Table object at ...>
-            >>> str(table)
-            '| Rank | Player   |\\n| ---- | -------- |\\n| 1st  | Crosby   |\\n| 2nd  | McDavid  |\\n| 3rd  | Matthews |'
+            Table(header=[...], body=[...], align=None, indent=0)
+            >>> print(table)
+            | Rank | Player   |
+            | ---- | -------- |
+            | 1st  | Crosby   |
+            | 2nd  | McDavid  |
+            | 3rd  | Matthews |
 
-        :raises ValueError: 
+        :raises ValueError:
             when row is not the same width as the table header
-        :param Iterable[str | Inline | Paragraph] row: 
+        :param Iterable[str | Inline | Paragraph] row:
             a row of data
         :return:
             self
         """
 
         # Consume row
-        row_list = [_ for _ in row]
-        logger.debug(f"Adding row to table: {row_list}")
-        
+        row_list = list(row)
+        logger.debug("Adding row to table: %r", row_list)
+
         # Verify that it's safe to add
         if len(row) != len(self._header):
             raise ValueError(
-                f"Unable to add row with width {len(row_list)} to table with header of width {len(self._header)}"
+                f"Unable to add row with width {len(row_list)} "
+                f"to table with header of width {len(self._header)}"
             )
-        
+
         # Add it to table
         self._body.append(row_list)
-        
+
         # Update widths as needed
         for i, item in enumerate(row_list):
             item_width = len(str(item))
             if item_width > self._widths[i]:
                 self._widths[i] = item_width
 
         return self
```

### Comparing `snakemd-2.1.0/PKG-INFO` & `snakemd-2.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemd
-Version: 2.1.0
+Version: 2.2.0b1
 Summary: A markdown generation library for Python.
 Home-page: https://www.snakemd.io
 License: MIT
 Author: Jeremy Grifski
 Author-email: jeremy.grifski@therenegadecoder.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
+Project-URL: Changelog, https://www.snakemd.io/en/latest/version-history/
 Project-URL: Documentation, https://www.snakemd.io/en/latest/docs/
 Project-URL: Repository, https://github.com/TheRenegadeCoder/SnakeMD
-Project-URL: changelog, https://www.snakemd.io/en/latest/version-history/
 Description-Content-Type: text/markdown
 
 # Welcome to SnakeMD
 
 SnakeMD is your ticket to generating Markdown in Python. To prove it to you, we've generated this entire README using SnakeMD. See readme.py for how it was done. To get started, download and install SnakeMD:
 
 ```shell
@@ -84,17 +84,19 @@
 
 Links are targets to files or web pages and can be embedded in paragraphs in a variety of ways, such as with the insert_link() method.
 
 _SnakeMD Source_
 
 ```py
 def _insert_link(doc: Document):
-    doc.add_paragraph("Learn to program with The Renegade Coder (@RenegadeCoder94).") \
-        .insert_link("The Renegade Coder", "https://therenegadecoder.com") \
-        .insert_link("@RenegadeCoder94", "https://twitter.com/RenegadeCoder94")
+    doc.add_paragraph(
+        "Learn to program with The Renegade Coder (@RenegadeCoder94)."
+    ).insert_link("The Renegade Coder", "https://therenegadecoder.com").insert_link(
+        "@RenegadeCoder94", "https://twitter.com/RenegadeCoder94"
+    )
 ```
 
 _Markdown Source_
 
 ```markdown
 Learn to program with [The Renegade Coder](https://therenegadecoder.com) ([@RenegadeCoder94](https://twitter.com/RenegadeCoder94)).
 ```
@@ -185,21 +187,15 @@
 
 Checklists are lists in which the items themselves can be checked on and off. This feature is new as of v0.10.0.
 
 _SnakeMD Source_
 
 ```py
 def _checklist(doc: Document):
-    doc.add_checklist(
-        [
-            "Pass the puck",
-            "Shoot the puck",
-            "Score a goal"
-        ]
-    )
+    doc.add_checklist(["Pass the puck", "Shoot the puck", "Score a goal"])
 ```
 
 _Markdown Source_
 
 ```markdown
 - [ ] Pass the puck
 - [ ] Shoot the puck
@@ -217,23 +213,22 @@
 Nested lists are complex lists that contain lists. Currently, SnakeMD does not support any convenience methods to generate nested lists, but they can be created manually using the MDList object.
 
 _SnakeMD Source_
 
 ```py
 def _nested_list(doc: Document):
     doc.add_block(
-        MDList([
-            "Apples",
-            Inline("Onions", bold=True),
-            MDList([
-                "Sweet",
-                "Red"
-            ]),
-            Paragraph(["This is the end of the list!"])
-        ])
+        MDList(
+            [
+                "Apples",
+                Inline("Onions", bold=True),
+                MDList(["Sweet", "Red"]),
+                Paragraph(["This is the end of the list!"]),
+            ]
+        )
     )
 ```
 
 _Markdown Source_
 
 ```markdown
 - Apples
@@ -257,21 +252,17 @@
 
 _SnakeMD Source_
 
 ```py
 def _table(doc: Document):
     doc.add_table(
         ["Height (cm)", "Weight (kg)", "Age (y)"],
-        [
-            ['150', '70', '21'],
-            ['164', '75', '19'],
-            ['181', '87', '40']
-        ],
+        [["150", "70", "21"], ["164", "75", "19"], ["181", "87", "40"]],
         [Table.Align.LEFT, Table.Align.CENTER, Table.Align.RIGHT],
-        0
+        0,
     )
 ```
 
 _Markdown Source_
 
 ```markdown
 | Height (cm) | Weight (kg) | Age (y) |
```

