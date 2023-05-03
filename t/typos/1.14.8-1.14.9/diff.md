# Comparing `tmp/typos-1.14.8.tar.gz` & `tmp/typos-1.14.9.tar.gz`

## Comparing `typos-1.14.8.tar` & `typos-1.14.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 typos-1.14.8/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.8/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44797 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.8/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.8/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.8/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  5965618 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-04-19 14:50:07.000000 typos-1.14.8/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.8/pyproject.toml
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 typos-1.14.8/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12565 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21534 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32485 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5359 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-04-19 14:50:07.000000 typos-1.14.8/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123    51732 2023-04-19 14:50:07.000000 typos-1.14.8/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.8/PKG-INFO
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.9/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.9/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44486 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.9/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  5970347 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.14.9/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.9/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-05-03 14:05:37.000000 typos-1.14.9/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.9/pyproject.toml
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 typos-1.14.9/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12559 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21534 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32485 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5359 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-05-03 14:05:37.000000 typos-1.14.9/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123    51971 2023-05-03 14:05:37.000000 typos-1.14.9/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.9/PKG-INFO
```

### Comparing `typos-1.14.8/local_dependencies/typos-vars/Cargo.toml` & `typos-1.14.9/local_dependencies/typos-vars/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-vars"
-version = "0.8.9"
+version = "0.8.10"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.14.8/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.14.9/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/typos/Cargo.toml` & `typos-1.14.9/local_dependencies/typos/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos"
-version = "0.10.11"
+version = "0.10.12"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -18,15 +18,15 @@
   "benches/**/*",
   "examples/**/*"
 ]
 
 [dependencies]
 anyhow = "1.0"
 thiserror = "1.0"
-winnow = "0.4.1"
+winnow = "0.4.4"
 unicode-xid = "0.2.4"
 once_cell = "1.17.1"
 serde = { version = "1.0", features = ["derive"] }
 simdutf8 = "0.1.4"
 itertools = "0.10"
 unicode-segmentation = "1.10.1"
 bstr = "1.4"
```

### Comparing `typos-1.14.8/local_dependencies/typos/src/check.rs` & `typos-1.14.9/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/typos/src/dict.rs` & `typos-1.14.9/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/typos/src/tokens.rs` & `typos-1.14.9/local_dependencies/typos/src/tokens.rs`

 * *Files 1% similar despite different names*

```diff
@@ -121,24 +121,22 @@
                 Some(valid)
             }
         }
     }
 }
 
 mod parser {
-    use winnow::branch::*;
-    use winnow::bytes::*;
     use winnow::combinator::*;
     use winnow::prelude::*;
-    use winnow::sequence::*;
     use winnow::stream::AsBStr;
     use winnow::stream::AsChar;
     use winnow::stream::SliceLen;
     use winnow::stream::Stream;
     use winnow::stream::StreamIsPartial;
+    use winnow::token::*;
 
     pub(crate) fn next_identifier<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
@@ -253,49 +251,49 @@
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         preceded(
             '#',
             alt((
-                terminated(take_while_m_n(3, 8, is_lower_hex_digit), peek(sep1)),
-                terminated(take_while_m_n(3, 8, is_upper_hex_digit), peek(sep1)),
+                terminated(take_while(3..=8, is_lower_hex_digit), peek(sep1)),
+                terminated(take_while(3..=8, is_upper_hex_digit), peek(sep1)),
             )),
         )
         .parse_next(input)
     }
 
     fn uuid_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         alt((
             (
-                take_while_m_n(8, 8, is_lower_hex_digit),
+                take_while(8, is_lower_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_lower_hex_digit),
+                take_while(4, is_lower_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_lower_hex_digit),
+                take_while(4, is_lower_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_lower_hex_digit),
+                take_while(4, is_lower_hex_digit),
                 '-',
-                take_while_m_n(12, 12, is_lower_hex_digit),
+                take_while(12, is_lower_hex_digit),
             ),
             (
-                take_while_m_n(8, 8, is_upper_hex_digit),
+                take_while(8, is_upper_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_upper_hex_digit),
+                take_while(4, is_upper_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_upper_hex_digit),
+                take_while(4, is_upper_hex_digit),
                 '-',
-                take_while_m_n(4, 4, is_upper_hex_digit),
+                take_while(4, is_upper_hex_digit),
                 '-',
-                take_while_m_n(12, 12, is_upper_hex_digit),
+                take_while(12, is_upper_hex_digit),
             ),
         ))
         .recognize()
         .parse_next(input)
     }
 
     fn hash_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
@@ -310,18 +308,17 @@
         //   - Git allows abbreviated hashes, but we need a good abbreviation
         //     that won't be mistaken for a variable name.
         //   - Through experimentation we've found that there is almost
         //     never any actual text inside a hex string of 32 characters
         //     or more.
 
         const IGNORE_HEX_MIN: usize = 32;
-        const IGNORE_HEX_MAX: usize = usize::MAX;
         alt((
-            take_while_m_n(IGNORE_HEX_MIN, IGNORE_HEX_MAX, is_lower_hex_digit),
-            take_while_m_n(IGNORE_HEX_MIN, IGNORE_HEX_MAX, is_upper_hex_digit),
+            take_while(IGNORE_HEX_MIN.., is_lower_hex_digit),
+            take_while(IGNORE_HEX_MIN.., is_upper_hex_digit),
         ))
         .parse_next(input)
     }
 
     fn base64_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
         T: Stream + StreamIsPartial + PartialEq,
@@ -346,15 +343,15 @@
         {
             return Err(winnow::error::ErrMode::Backtrack(
                 winnow::error::Error::new(input, winnow::error::ErrorKind::Slice),
             ));
         }
 
         let (after, _) =
-            take_while_m_n(padding_len, padding_len, is_base64_padding).parse_next(padding)?;
+            take_while(padding_len..=padding_len, is_base64_padding).parse_next(padding)?;
 
         let after_offset = input.offset_to(&after);
         Ok(input.next_slice(after_offset))
     }
 
     fn email_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
     where
@@ -435,20 +432,15 @@
 
     fn take_many0<I, E, F>(mut f: F) -> impl FnMut(I) -> IResult<I, <I as Stream>::Slice, E>
     where
         I: Stream,
         F: winnow::Parser<I, <I as Stream>::Slice, E>,
         E: winnow::error::ParseError<I>,
     {
-        move |i: I| {
-            winnow::multi::many0(f.by_ref())
-                .map(|()| ())
-                .recognize()
-                .parse_next(i)
-        }
+        move |i: I| repeat0(f.by_ref()).map(|()| ()).recognize().parse_next(i)
     }
 
     #[inline]
     fn is_dec_digit(i: impl AsChar + Copy) -> bool {
         i.is_dec_digit()
     }
```

### Comparing `typos-1.14.8/local_dependencies/dictgen/Cargo.toml` & `typos-1.14.9/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/dictgen/src/map.rs` & `typos-1.14.9/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/dictgen/src/table.rs` & `typos-1.14.9/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/dictgen/src/trie.rs` & `typos-1.14.9/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/varcon-core/Cargo.toml` & `typos-1.14.9/local_dependencies/varcon-core/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "varcon-core"
-version = "2.2.10"
+version = "2.2.11"
 description = "Varcon-relevant data structures"
 readme = "../../README.md"
 categories = ["text-processing"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
 rust-version= "1.64.0"  # MSRV
@@ -20,12 +20,12 @@
 
 [features]
 default = []
 parser = ["winnow"]
 flags = ["enumflags2"]
 
 [dependencies]
-winnow = { version = "0.4.1", optional = true }
+winnow = { version = "0.4.4", optional = true }
 enumflags2 = { version = "0.7", optional = true }
 
 [package.metadata.docs.rs]
 features = [ "parser", "flags" ]
```

### Comparing `typos-1.14.8/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.14.9/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/varcon-core/src/lib.rs` & `typos-1.14.9/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/varcon-core/src/parser.rs` & `typos-1.14.9/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.14.9/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5430,148 +5430,283 @@
         dictgen::InsensitiveStr::Ascii("pries"),
     ],
     values: &[&["vampires"], &["vampires"], &["vampires"], &["vampires"]],
     range: 4..=5,
 };
 
 static WORD_VAL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
-    children: dictgen::DictTrieChild::Flat(&WORD_VAL_CHILDREN),
+    children: dictgen::DictTrieChild::Nested(&WORD_VAL_CHILDREN),
     value: None,
 };
 
-pub static WORD_VAL_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+static WORD_VAL_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
+    Some(&WORD_VALA_NODE),
+    None,
+    None,
+    Some(&WORD_VALD_NODE),
+    Some(&WORD_VALE_NODE),
+    None,
+    None,
+    None,
+    Some(&WORD_VALI_NODE),
+    None,
+    Some(&WORD_VALK_NODE),
+    Some(&WORD_VALL_NODE),
+    None,
+    Some(&WORD_VALN_NODE),
+    None,
+    None,
+    None,
+    None,
+    None,
+    Some(&WORD_VALT_NODE),
+    Some(&WORD_VALU_NODE),
+    None,
+    None,
+    None,
+    Some(&WORD_VALY_NODE),
+    None,
+];
+
+static WORD_VALY_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALY_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALY_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("krie")],
+    values: &[&["valkyrie"]],
+    range: 4..=4,
+};
+
+static WORD_VALU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALU_CHILDREN),
+    value: Some(&["value"]),
+};
+
+pub static WORD_VALU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
-        dictgen::InsensitiveStr::Ascii("ailable"),
-        dictgen::InsensitiveStr::Ascii("date"),
-        dictgen::InsensitiveStr::Ascii("diated"),
-        dictgen::InsensitiveStr::Ascii("enca"),
-        dictgen::InsensitiveStr::Ascii("enica"),
-        dictgen::InsensitiveStr::Ascii("entein"),
-        dictgen::InsensitiveStr::Ascii("entians"),
-        dictgen::InsensitiveStr::Ascii("entie"),
-        dictgen::InsensitiveStr::Ascii("entien"),
-        dictgen::InsensitiveStr::Ascii("entiens"),
-        dictgen::InsensitiveStr::Ascii("entimes"),
-        dictgen::InsensitiveStr::Ascii("entinas"),
-        dictgen::InsensitiveStr::Ascii("entinos"),
-        dictgen::InsensitiveStr::Ascii("entins"),
-        dictgen::InsensitiveStr::Ascii("entis"),
-        dictgen::InsensitiveStr::Ascii("entones"),
-        dictgen::InsensitiveStr::Ascii("etta"),
-        dictgen::InsensitiveStr::Ascii("eu"),
-        dictgen::InsensitiveStr::Ascii("iation"),
-        dictgen::InsensitiveStr::Ascii("iator"),
-        dictgen::InsensitiveStr::Ascii("idade"),
-        dictgen::InsensitiveStr::Ascii("idaterelase"),
-        dictgen::InsensitiveStr::Ascii("idationt"),
-        dictgen::InsensitiveStr::Ascii("idaty"),
-        dictgen::InsensitiveStr::Ascii("idd"),
-        dictgen::InsensitiveStr::Ascii("ide"),
-        dictgen::InsensitiveStr::Ascii("ididty"),
-        dictgen::InsensitiveStr::Ascii("iding"),
-        dictgen::InsensitiveStr::Ascii("iditity"),
-        dictgen::InsensitiveStr::Ascii("iditiy"),
-        dictgen::InsensitiveStr::Ascii("ied"),
-        dictgen::InsensitiveStr::Ascii("ies"),
-        dictgen::InsensitiveStr::Ascii("if"),
-        dictgen::InsensitiveStr::Ascii("itdity"),
-        dictgen::InsensitiveStr::Ascii("kirye"),
-        dictgen::InsensitiveStr::Ascii("kiyre"),
-        dictgen::InsensitiveStr::Ascii("kriye"),
-        dictgen::InsensitiveStr::Ascii("kryie"),
-        dictgen::InsensitiveStr::Ascii("kues"),
-        dictgen::InsensitiveStr::Ascii("kyire"),
-        dictgen::InsensitiveStr::Ascii("kyre"),
-        dictgen::InsensitiveStr::Ascii("lid"),
-        dictgen::InsensitiveStr::Ascii("lidation"),
-        dictgen::InsensitiveStr::Ascii("lidity"),
-        dictgen::InsensitiveStr::Ascii("lue"),
-        dictgen::InsensitiveStr::Ascii("lues"),
-        dictgen::InsensitiveStr::Ascii("necia"),
-        dictgen::InsensitiveStr::Ascii("netines"),
-        dictgen::InsensitiveStr::Ascii("tage"),
-        dictgen::InsensitiveStr::Ascii("tages"),
-        dictgen::InsensitiveStr::Ascii("u"),
-        dictgen::InsensitiveStr::Ascii("uabe"),
-        dictgen::InsensitiveStr::Ascii("ubale"),
-        dictgen::InsensitiveStr::Ascii("uble"),
-        dictgen::InsensitiveStr::Ascii("udes"),
-        dictgen::InsensitiveStr::Ascii("ueable"),
-        dictgen::InsensitiveStr::Ascii("uess"),
-        dictgen::InsensitiveStr::Ascii("uie"),
-        dictgen::InsensitiveStr::Ascii("ule"),
-        dictgen::InsensitiveStr::Ascii("us"),
-        dictgen::InsensitiveStr::Ascii("use"),
-        dictgen::InsensitiveStr::Ascii("ykrie"),
+        dictgen::InsensitiveStr::Ascii("abe"),
+        dictgen::InsensitiveStr::Ascii("bale"),
+        dictgen::InsensitiveStr::Ascii("ble"),
+        dictgen::InsensitiveStr::Ascii("des"),
+        dictgen::InsensitiveStr::Ascii("eable"),
+        dictgen::InsensitiveStr::Ascii("ess"),
+        dictgen::InsensitiveStr::Ascii("ie"),
+        dictgen::InsensitiveStr::Ascii("le"),
+        dictgen::InsensitiveStr::Ascii("s"),
+        dictgen::InsensitiveStr::Ascii("se"),
     ],
     values: &[
-        &["available"],
-        &["validate"],
-        &["validated"],
-        &["valencia"],
-        &["valencia"],
-        &["valentine"],
-        &["valentines"],
-        &["valentines"],
-        &["valentine"],
-        &["valentines"],
-        &["valentines"],
-        &["valentines"],
-        &["valentines"],
-        &["valentines"],
-        &["valentines"],
-        &["valentines"],
-        &["valletta"],
+        &["valuable"],
+        &["valuable"],
+        &["valuable"],
+        &["values"],
+        &["valuable"],
+        &["values"],
         &["value"],
+        &["value"],
+        &["values"],
+        &["values", "value"],
+    ],
+    range: 1..=5,
+};
+
+static WORD_VALT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALT_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALT_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("age"),
+        dictgen::InsensitiveStr::Ascii("ages"),
+    ],
+    values: &[&["voltage"], &["voltages"]],
+    range: 3..=4,
+};
+
+static WORD_VALN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALN_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALN_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ecia"),
+        dictgen::InsensitiveStr::Ascii("etines"),
+    ],
+    values: &[&["valencia"], &["valentines"]],
+    range: 4..=6,
+};
+
+static WORD_VALL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALL_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALL_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("id"),
+        dictgen::InsensitiveStr::Ascii("idation"),
+        dictgen::InsensitiveStr::Ascii("idity"),
+        dictgen::InsensitiveStr::Ascii("ue"),
+        dictgen::InsensitiveStr::Ascii("ues"),
+    ],
+    values: &[
+        &["valid"],
+        &["validation"],
+        &["validity"],
+        &["value"],
+        &["values"],
+    ],
+    range: 2..=7,
+};
+
+static WORD_VALK_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALK_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALK_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("irye"),
+        dictgen::InsensitiveStr::Ascii("iyre"),
+        dictgen::InsensitiveStr::Ascii("riye"),
+        dictgen::InsensitiveStr::Ascii("ryie"),
+        dictgen::InsensitiveStr::Ascii("ues"),
+        dictgen::InsensitiveStr::Ascii("yire"),
+        dictgen::InsensitiveStr::Ascii("yre"),
+    ],
+    values: &[
+        &["valkyrie"],
+        &["valkyrie"],
+        &["valkyrie"],
+        &["valkyrie"],
+        &["values"],
+        &["valkyrie"],
+        &["valkyrie"],
+    ],
+    range: 3..=4,
+};
+
+static WORD_VALI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALI_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ation"),
+        dictgen::InsensitiveStr::Ascii("ator"),
+        dictgen::InsensitiveStr::Ascii("dade"),
+        dictgen::InsensitiveStr::Ascii("daterelase"),
+        dictgen::InsensitiveStr::Ascii("dationt"),
+        dictgen::InsensitiveStr::Ascii("daty"),
+        dictgen::InsensitiveStr::Ascii("dd"),
+        dictgen::InsensitiveStr::Ascii("de"),
+        dictgen::InsensitiveStr::Ascii("didty"),
+        dictgen::InsensitiveStr::Ascii("ding"),
+        dictgen::InsensitiveStr::Ascii("ditity"),
+        dictgen::InsensitiveStr::Ascii("ditiy"),
+        dictgen::InsensitiveStr::Ascii("dty"),
+        dictgen::InsensitiveStr::Ascii("ed"),
+        dictgen::InsensitiveStr::Ascii("es"),
+        dictgen::InsensitiveStr::Ascii("f"),
+        dictgen::InsensitiveStr::Ascii("tdity"),
+    ],
+    values: &[
         &["validation"],
         &["validator"],
         &["validated"],
         &["validaterelease"],
         &["validation"],
         &["validity"],
         &["valid"],
         &["valid"],
         &["validity"],
         &["validating"],
         &["validity"],
         &["validity"],
-        &["valid"],
-        &["values"],
-        &["valid"],
         &["validity"],
-        &["valkyrie"],
-        &["valkyrie"],
-        &["valkyrie"],
-        &["valkyrie"],
+        &["valid"],
         &["values"],
-        &["valkyrie"],
-        &["valkyrie"],
         &["valid"],
-        &["validation"],
         &["validity"],
-        &["value"],
-        &["values"],
+    ],
+    range: 1..=10,
+};
+
+static WORD_VALE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALE_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALE_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("nca"),
+        dictgen::InsensitiveStr::Ascii("nica"),
+        dictgen::InsensitiveStr::Ascii("ntein"),
+        dictgen::InsensitiveStr::Ascii("ntians"),
+        dictgen::InsensitiveStr::Ascii("ntie"),
+        dictgen::InsensitiveStr::Ascii("ntien"),
+        dictgen::InsensitiveStr::Ascii("ntiens"),
+        dictgen::InsensitiveStr::Ascii("ntimes"),
+        dictgen::InsensitiveStr::Ascii("ntinas"),
+        dictgen::InsensitiveStr::Ascii("ntinos"),
+        dictgen::InsensitiveStr::Ascii("ntins"),
+        dictgen::InsensitiveStr::Ascii("ntis"),
+        dictgen::InsensitiveStr::Ascii("ntones"),
+        dictgen::InsensitiveStr::Ascii("tta"),
+        dictgen::InsensitiveStr::Ascii("u"),
+    ],
+    values: &[
         &["valencia"],
+        &["valencia"],
+        &["valentine"],
         &["valentines"],
-        &["voltage"],
-        &["voltages"],
-        &["value"],
-        &["valuable"],
-        &["valuable"],
-        &["valuable"],
-        &["values"],
-        &["valuable"],
-        &["values"],
-        &["value"],
+        &["valentines"],
+        &["valentine"],
+        &["valentines"],
+        &["valentines"],
+        &["valentines"],
+        &["valentines"],
+        &["valentines"],
+        &["valentines"],
+        &["valentines"],
+        &["valletta"],
         &["value"],
-        &["values"],
-        &["values", "value"],
-        &["valkyrie"],
     ],
-    range: 1..=11,
+    range: 1..=6,
+};
+
+static WORD_VALD_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALD_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ate"),
+        dictgen::InsensitiveStr::Ascii("iated"),
+        dictgen::InsensitiveStr::Ascii("ity"),
+    ],
+    values: &[&["validate"], &["validated"], &["validity"]],
+    range: 3..=5,
+};
+
+static WORD_VALA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_VALA_CHILDREN),
+    value: None,
+};
+
+pub static WORD_VALA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("ilable")],
+    values: &[&["available"]],
+    range: 6..=6,
 };
 
 static WORD_VAK_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_VAK_CHILDREN),
     value: None,
 };
 
@@ -25261,29 +25396,33 @@
 pub static WORD_STAI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("cally"),
         dictgen::InsensitiveStr::Ascii("dum"),
         dictgen::InsensitiveStr::Ascii("dums"),
         dictgen::InsensitiveStr::Ascii("nlees"),
         dictgen::InsensitiveStr::Ascii("on"),
+        dictgen::InsensitiveStr::Ascii("onairy"),
+        dictgen::InsensitiveStr::Ascii("onary"),
         dictgen::InsensitiveStr::Ascii("ons"),
         dictgen::InsensitiveStr::Ascii("tion"),
         dictgen::InsensitiveStr::Ascii("tions"),
     ],
     values: &[
         &["statically"],
         &["stadium"],
         &["stadiums"],
         &["stainless"],
         &["station"],
+        &["stationary"],
+        &["stationary"],
         &["stations"],
         &["station"],
         &["stations"],
     ],
-    range: 2..=5,
+    range: 2..=6,
 };
 
 static WORD_STAG_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_STAG_CHILDREN),
     value: None,
 };
 
@@ -28660,14 +28799,15 @@
         dictgen::InsensitiveStr::Ascii("ification"),
         dictgen::InsensitiveStr::Ascii("iliquy"),
         dictgen::InsensitiveStr::Ascii("itudine"),
         dictgen::InsensitiveStr::Ascii("tion"),
         dictgen::InsensitiveStr::Ascii("uable"),
         dictgen::InsensitiveStr::Ascii("um"),
         dictgen::InsensitiveStr::Ascii("utide"),
+        dictgen::InsensitiveStr::Ascii("utiin"),
         dictgen::InsensitiveStr::Ascii("veable"),
         dictgen::InsensitiveStr::Ascii("wed"),
     ],
     values: &[
         &["solarmutex"],
         &["solitary"],
         &["soldiers"],
@@ -28689,14 +28829,15 @@
         &["solidification"],
         &["soliloquy"],
         &["solitude"],
         &["solution"],
         &["soluble"],
         &["solemn"],
         &["solitude"],
+        &["solution"],
         &["solvable"],
         &["solved"],
     ],
     range: 1..=9,
 };
 
 static WORD_SOK_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
@@ -59143,14 +59284,15 @@
         dictgen::InsensitiveStr::Ascii("ition"),
         dictgen::InsensitiveStr::Ascii("itions"),
         dictgen::InsensitiveStr::Ascii("itis"),
         dictgen::InsensitiveStr::Ascii("itts"),
         dictgen::InsensitiveStr::Ascii("ium"),
         dictgen::InsensitiveStr::Ascii("iums"),
         dictgen::InsensitiveStr::Ascii("ormance"),
+        dictgen::InsensitiveStr::Ascii("tuation"),
         dictgen::InsensitiveStr::Ascii("uation"),
         dictgen::InsensitiveStr::Ascii("uations"),
         dictgen::InsensitiveStr::Ascii("utaion"),
         dictgen::InsensitiveStr::Ascii("utaions"),
     ],
     values: &[
         &["premade"],
@@ -59198,14 +59340,15 @@
         &["permissions"],
         &["permits"],
         &["permits"],
         &["premium"],
         &["premiums"],
         &["performance"],
         &["permutation"],
+        &["permutation"],
         &["permutations"],
         &["permutation"],
         &["permutations"],
     ],
     range: 3..=8,
 };
 
@@ -80945,14 +81088,15 @@
 static WORD_LIN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_LIN_CHILDREN),
     value: None,
 };
 
 pub static WORD_LIN_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("aer"),
         dictgen::InsensitiveStr::Ascii("cese"),
         dictgen::InsensitiveStr::Ascii("cesed"),
         dictgen::InsensitiveStr::Ascii("ceses"),
         dictgen::InsensitiveStr::Ascii("clon"),
         dictgen::InsensitiveStr::Ascii("colin"),
         dictgen::InsensitiveStr::Ascii("colon"),
         dictgen::InsensitiveStr::Ascii("earily"),
@@ -80983,14 +81127,15 @@
         dictgen::InsensitiveStr::Ascii("kfy"),
         dictgen::InsensitiveStr::Ascii("naena"),
         dictgen::InsensitiveStr::Ascii("tain"),
         dictgen::InsensitiveStr::Ascii("ueps"),
         dictgen::InsensitiveStr::Ascii("z"),
     ],
     values: &[
+        &["linear"],
         &["license"],
         &["licensed"],
         &["licenses"],
         &["lincoln"],
         &["lincoln"],
         &["lincoln"],
         &["linearly", "linearity"],
@@ -85536,14 +85681,15 @@
         dictgen::InsensitiveStr::Ascii("lidades"),
         dictgen::InsensitiveStr::Ascii("lidante"),
         dictgen::InsensitiveStr::Ascii("lidare"),
         dictgen::InsensitiveStr::Ascii("lidas"),
         dictgen::InsensitiveStr::Ascii("lidatiopn"),
         dictgen::InsensitiveStr::Ascii("lide"),
         dictgen::InsensitiveStr::Ascii("lidiate"),
+        dictgen::InsensitiveStr::Ascii("lis"),
         dictgen::InsensitiveStr::Ascii("lubale"),
         dictgen::InsensitiveStr::Ascii("lud"),
         dictgen::InsensitiveStr::Ascii("lueble"),
         dictgen::InsensitiveStr::Ascii("raibly"),
         dictgen::InsensitiveStr::Ascii("riabil"),
         dictgen::InsensitiveStr::Ascii("riabley"),
         dictgen::InsensitiveStr::Ascii("riablly"),
@@ -85570,14 +85716,15 @@
         &["invalidates"],
         &["invalidate"],
         &["invalidate"],
         &["invalidates"],
         &["invalidation"],
         &["invalid"],
         &["invalidate"],
+        &["invalid"],
         &["invaluable"],
         &["invalid"],
         &["invaluable"],
         &["invariably"],
         &["invariably"],
         &["invariably"],
         &["invariably"],
@@ -88734,14 +88881,15 @@
         dictgen::InsensitiveStr::Ascii("tating"),
         dictgen::InsensitiveStr::Ascii("tation"),
         dictgen::InsensitiveStr::Ascii("tations"),
         dictgen::InsensitiveStr::Ascii("teneous"),
         dictgen::InsensitiveStr::Ascii("tenious"),
         dictgen::InsensitiveStr::Ascii("tialed"),
         dictgen::InsensitiveStr::Ascii("tiaties"),
+        dictgen::InsensitiveStr::Ascii("tiatoins"),
         dictgen::InsensitiveStr::Ascii("ty"),
         dictgen::InsensitiveStr::Ascii("ze"),
     ],
     values: &[
         &["instantiation"],
         &["instance"],
         &["instantiate"],
@@ -88770,14 +88918,15 @@
         &["instantiating"],
         &["instantiation"],
         &["instantiations"],
         &["instantaneous"],
         &["instantaneous"],
         &["instantiated"],
         &["instantiates"],
+        &["instantiations"],
         &["instantly"],
         &["instance"],
     ],
     range: 1..=9,
 };
 
 static WORD_INSTAL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
@@ -93596,16 +93745,19 @@
 
 static WORD_INAV_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_INAV_CHILDREN),
     value: None,
 };
 
 pub static WORD_INAV_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("lid")],
-    values: &[&["invalid"]],
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("lid"),
+        dictgen::InsensitiveStr::Ascii("lis"),
+    ],
+    values: &[&["invalid"], &["invalid"]],
     range: 3..=3,
 };
 
 static WORD_INAU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_INAU_CHILDREN),
     value: None,
 };
@@ -115769,14 +115921,15 @@
         dictgen::InsensitiveStr::Ascii("ronously"),
         dictgen::InsensitiveStr::Ascii("rorneous"),
         dictgen::InsensitiveStr::Ascii("rorneously"),
         dictgen::InsensitiveStr::Ascii("rorneus"),
         dictgen::InsensitiveStr::Ascii("rornous"),
         dictgen::InsensitiveStr::Ascii("rornously"),
         dictgen::InsensitiveStr::Ascii("rorr"),
+        dictgen::InsensitiveStr::Ascii("rorrs"),
         dictgen::InsensitiveStr::Ascii("ros"),
         dictgen::InsensitiveStr::Ascii("rot"),
         dictgen::InsensitiveStr::Ascii("rots"),
         dictgen::InsensitiveStr::Ascii("rro"),
         dictgen::InsensitiveStr::Ascii("rror"),
         dictgen::InsensitiveStr::Ascii("rrors"),
         dictgen::InsensitiveStr::Ascii("rros"),
@@ -115821,14 +115974,15 @@
         &["erroneous"],
         &["erroneously"],
         &["erroneous"],
         &["erroneous"],
         &["erroneously"],
         &["error"],
         &["errors"],
+        &["errors"],
         &["error"],
         &["errors"],
         &["error"],
         &["error"],
         &["errors"],
         &["errors"],
         &["erupted"],
@@ -116051,14 +116205,15 @@
         dictgen::InsensitiveStr::Ascii("ect"),
         dictgen::InsensitiveStr::Ascii("ected"),
         dictgen::InsensitiveStr::Ascii("ectedly"),
         dictgen::InsensitiveStr::Ascii("ecting"),
         dictgen::InsensitiveStr::Ascii("ects"),
         dictgen::InsensitiveStr::Ascii("hememeral"),
         dictgen::InsensitiveStr::Ascii("hememeris"),
+        dictgen::InsensitiveStr::Ascii("hermeral"),
         dictgen::InsensitiveStr::Ascii("hipany"),
         dictgen::InsensitiveStr::Ascii("idsodes"),
         dictgen::InsensitiveStr::Ascii("igramic"),
         dictgen::InsensitiveStr::Ascii("ihpany"),
         dictgen::InsensitiveStr::Ascii("ilepsey"),
         dictgen::InsensitiveStr::Ascii("ilespy"),
         dictgen::InsensitiveStr::Ascii("ilgoue"),
@@ -116095,14 +116250,15 @@
         &["expect"],
         &["expected"],
         &["expectedly"],
         &["expecting"],
         &["expects"],
         &["ephemeral"],
         &["ephemeris"],
+        &["ephemeral"],
         &["epiphany"],
         &["episodes"],
         &["epigrammatic"],
         &["epiphany"],
         &["epilepsy"],
         &["epilepsy"],
         &["epilogue"],
@@ -119584,14 +119740,15 @@
         dictgen::InsensitiveStr::Ascii("fordlessly"),
         dictgen::InsensitiveStr::Ascii("fords"),
         dictgen::InsensitiveStr::Ascii("fortlesly"),
         dictgen::InsensitiveStr::Ascii("fortlessely"),
         dictgen::InsensitiveStr::Ascii("fortlessley"),
         dictgen::InsensitiveStr::Ascii("fortlessy"),
         dictgen::InsensitiveStr::Ascii("fulence"),
+        dictgen::InsensitiveStr::Ascii("icient"),
         dictgen::InsensitiveStr::Ascii("orceable"),
     ],
     values: &[
         &["effect"],
         &["effective"],
         &["effectively"],
         &["evil"],
@@ -119642,14 +119799,15 @@
         &["effortlessly"],
         &["efforts", "affords"],
         &["effortlessly"],
         &["effortlessly"],
         &["effortlessly"],
         &["effortlessly"],
         &["effluence"],
+        &["efficient"],
         &["enforceable"],
     ],
     range: 2..=11,
 };
 
 static WORD_EE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_EE_CHILDREN),
@@ -122222,29 +122380,31 @@
 };
 
 pub static WORD_DIT_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("actorship"),
         dictgen::InsensitiveStr::Ascii("ance"),
         dictgen::InsensitiveStr::Ascii("inguishes"),
+        dictgen::InsensitiveStr::Ascii("o"),
         dictgen::InsensitiveStr::Ascii("ribute"),
         dictgen::InsensitiveStr::Ascii("ributed"),
         dictgen::InsensitiveStr::Ascii("ribution"),
         dictgen::InsensitiveStr::Ascii("ributions"),
     ],
     values: &[
         &["dictatorship"],
         &["distance"],
         &["distinguishes"],
+        &["ditto"],
         &["distribute"],
         &["distributed"],
         &["distribution"],
         &["distributions"],
     ],
-    range: 4..=9,
+    range: 1..=9,
 };
 
 static WORD_DIS_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_DIS_CHILDREN),
     value: None,
 };
 
@@ -142923,25 +143083,27 @@
         dictgen::InsensitiveStr::Ascii("tuive"),
         dictgen::InsensitiveStr::Ascii("tutive"),
         dictgen::InsensitiveStr::Ascii("uence"),
         dictgen::InsensitiveStr::Ascii("uences"),
         dictgen::InsensitiveStr::Ascii("uentes"),
         dictgen::InsensitiveStr::Ascii("uently"),
         dictgen::InsensitiveStr::Ascii("uitively"),
+        dictgen::InsensitiveStr::Ascii("utevily"),
     ],
     values: &[
         &["consecutive"],
         &["consecutively"],
         &["consecutive"],
         &["consecutive"],
         &["consequence"],
         &["consequences"],
         &["consequences"],
         &["consequently"],
         &["consecutively"],
+        &["consecutively"],
     ],
     range: 4..=8,
 };
 
 static WORD_CONSEA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CONSEA_CHILDREN),
     value: None,
@@ -164369,14 +164531,15 @@
         dictgen::InsensitiveStr::Ascii("iobok"),
         dictgen::InsensitiveStr::Ascii("iobookas"),
         dictgen::InsensitiveStr::Ascii("iobookmrs"),
         dictgen::InsensitiveStr::Ascii("ioboook"),
         dictgen::InsensitiveStr::Ascii("ioboooks"),
         dictgen::InsensitiveStr::Ascii("ioboost"),
         dictgen::InsensitiveStr::Ascii("omoderator"),
+        dictgen::InsensitiveStr::Ascii("ovisual"),
     ],
     values: &[
         &["audacity"],
         &["audible"],
         &["audacity"],
         &["audience"],
         &["audience"],
@@ -164384,14 +164547,15 @@
         &["audiobook"],
         &["audiobooks"],
         &["audiobooks"],
         &["audiobook"],
         &["audiobook"],
         &["audiobooks"],
         &["automoderator"],
+        &["audiovisual"],
     ],
     range: 4..=10,
 };
 
 static WORD_AUC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_AUC_CHILDREN),
     value: None,
```

### Comparing `typos-1.14.8/rust_src/typos-cli/Cargo.toml` & `typos-1.14.9/rust_src/typos-cli/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.14.8"
+version = "1.14.9"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -47,51 +47,51 @@
 [[bin]]
 name = "typos"
 path = "src/bin/typos-cli/main.rs"
 doc = false
 
 [dependencies]
 typos = { version = "^0.10", path = "../../local_dependencies/typos" }
-varcon-core = { version = "^2.2.9", path = "../../local_dependencies/varcon-core" }
+varcon-core = { version = "^2.2.11", path = "../../local_dependencies/varcon-core" }
 typos-dict = { version = "^0.9", path = "../../local_dependencies/typos-dict", optional = true }
 typos-vars = { version = "^0.8", path = "../../local_dependencies/typos-vars", optional = true }
 unicase = "2.6"
 anyhow = "1.0"
-clap = { version = "4.2.1", features = ["derive"] }
+clap = { version = "4.2.5", features = ["derive"] }
 clap-verbosity-flag = "2.0"
 ignore = "0.4"
 serde = { version = "1.0", features = ["derive"] }
 toml = "0.7.3"
 log = "0.4"
 env_logger = { version = "0.10", default-features = false, features = ["auto-color"] }
 atty = "0.2.14"
 bstr = "1.4"
 once_cell = "1.17.1"
 ahash = "0.8"
 difflib = "0.4"
 proc-exit = "2.0"
-human-panic = "1.1.3"
+human-panic = "1.1.4"
 content_inspector = "0.2.4"
 unicode-segmentation = "1.10.1"
 derive_more = "0.99.17"
 derive_setters = "0.1"
 itertools = "0.10"
 serde_json = "1.0"
 kstring = { version = "2.0.0", features = ["serde"] }
 typed-arena = "2.0.2"
 maplit = "1.0"
 unicode-width = "0.1.10"
 unic-emoji-char = "0.9.0"
 thread_local = "1.1.7"
 globset = "0.4.10"
 anstyle = "1.0.0"
-anstream = "0.3.0"
+anstream = "0.3.1"
 colorchoice-clap = "1.0.0"
 serde_regex = "1.1.0"
-regex = "1.7.3"
+regex = "1.8.1"
 encoding_rs = "0.8.32"
 
 [[bench]]
 name = "checks"
 harness = false
 
 [[bench]]
```

### Comparing `typos-1.14.8/rust_src/typos-cli/benches/checks.rs` & `typos-1.14.9/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/benches/corrections.rs` & `typos-1.14.9/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/benches/data.rs` & `typos-1.14.9/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.14.9/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.14.9/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files 0% similar despite different names*

```diff
@@ -348,17 +348,17 @@
     fn test_calculate_visible_column_width_horizontal_tab() {
         assert_eq!(1, calculate_visible_column_width("\t"));
     }
 
     #[test]
     fn test_calculate_visible_column_width_latin_cyrillic() {
         let latin_cyrillic_chars = [
-            "À",  /* U+00C0; Latin Capital Letter A with Grave */
+            "À", /* U+00C0; Latin Capital Letter A with Grave */
             "À", /* U+0041 U+0300; Latin Capital Letter A, Combining Grave Accent */
-            "А",  /* U+0410 Cyrillic Capital Letter A */
+            "А", /* U+0410 Cyrillic Capital Letter A */
         ];
         for (i, ch) in latin_cyrillic_chars.iter().enumerate() {
             let width = calculate_visible_column_width(ch);
             assert_eq!(1, width, "latin_cyrillic[{}]: {}", i, ch,);
         }
     }
 
@@ -396,16 +396,16 @@
             assert_eq!(2, width, "emoji[{}]: {}", i, ch);
         }
     }
 
     #[test]
     fn test_calculate_visible_column_width_zwj_sequences() {
         let zwj_sequences = [
-            "😵‍💫",       /* U+1F635 U+200D U+1F4AB */
-            "👁️‍🗨️", /* U+1F441 U+FE0F U+200D U+1F5E8 U+FE0F */
+            "😵‍💫", /* U+1F635 U+200D U+1F4AB */
+            "👁️‍🗨️",   /* U+1F441 U+FE0F U+200D U+1F5E8 U+FE0F */
         ];
         for (i, ch) in zwj_sequences.iter().enumerate() {
             let width = calculate_visible_column_width(ch);
             assert_eq!(2, width, "zwj[{}]: {}", i, ch);
         }
     }
 }
```

### Comparing `typos-1.14.8/rust_src/typos-cli/src/config.rs` & `typos-1.14.9/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/default_types.rs` & `typos-1.14.9/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/dict.rs` & `typos-1.14.9/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/file.rs` & `typos-1.14.9/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/file_type.rs` & `typos-1.14.9/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/policy.rs` & `typos-1.14.9/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/rust_src/typos-cli/src/report.rs` & `typos-1.14.9/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.8/Cargo.lock` & `typos-1.14.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.3.0"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -81,17 +90,17 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
@@ -229,38 +238,38 @@
  "strsim 0.10.0",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.2"
+version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
+checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap-verbosity-flag"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23e2b6c3dcdb73299f48ae05b294da14e2f560b3ed2c09e742269eb1b22af231"
 dependencies = [
- "clap 4.2.2",
+ "clap 4.2.5",
  "log",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.2"
+version = "4.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
+checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim 0.10.0",
 ]
@@ -336,15 +345,15 @@
 
 [[package]]
 name = "colorchoice-clap"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "412e88a3a3a3f52e436909b49beb467a05649e8b0dda0e6202bd05c1b63dbc49"
 dependencies = [
- "clap 4.2.2",
+ "clap 4.2.5",
  "colorchoice",
 ]
 
 [[package]]
 name = "content_inspector"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -678,15 +687,15 @@
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.19",
  "bstr",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
@@ -1216,34 +1225,34 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 1.0.1",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
 
@@ -1570,15 +1579,15 @@
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typos"
-version = "0.10.11"
+version = "0.10.12"
 dependencies = [
  "anyhow",
  "bstr",
  "itertools",
  "once_cell",
  "serde",
  "simdutf8",
@@ -1586,24 +1595,24 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.14.8"
+version = "1.14.9"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
  "bstr",
- "clap 4.2.2",
+ "clap 4.2.5",
  "clap-verbosity-flag",
  "colorchoice-clap",
  "content_inspector",
  "criterion",
  "derive_more",
  "derive_setters",
  "difflib",
@@ -1634,29 +1643,29 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.9.25"
+version = "0.9.26"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "itertools",
  "snapbox",
  "unicase",
  "varcon",
 ]
 
 [[package]]
 name = "typos-vars"
-version = "0.8.9"
+version = "0.8.10"
 dependencies = [
  "codegenrs",
  "dictgen",
  "itertools",
  "snapbox",
  "typos",
  "unicase",
@@ -1751,24 +1760,24 @@
 checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "varcon"
-version = "0.6.8"
+version = "0.6.9"
 dependencies = [
  "codegenrs",
  "snapbox",
  "varcon-core",
 ]
 
 [[package]]
 name = "varcon-core"
-version = "2.2.10"
+version = "2.2.11"
 dependencies = [
  "enumflags2",
  "winnow",
 ]
 
 [[package]]
 name = "version_check"
@@ -2053,13 +2062,13 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "5617da7e1f97bf363947d767b91aaf3c2bbc19db7fda9c65af1278713d58e0a2"
 dependencies = [
  "memchr",
 ]
```

### Comparing `typos-1.14.8/PKG-INFO` & `typos-1.14.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.14.8
+Version: 1.14.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

