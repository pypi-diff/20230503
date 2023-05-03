# Comparing `tmp/glyphsets-0.6.0.tar.gz` & `tmp/glyphsets-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyphsets-0.6.0.tar", last modified: Tue Mar 21 13:53:37 2023, max compression
+gzip compressed data, was "glyphsets-0.6.1.tar", last modified: Wed May  3 15:30:47 2023, max compression
```

## Comparing `glyphsets-0.6.0.tar` & `glyphsets-0.6.1.tar`

### file list

```diff
@@ -1,491 +1,505 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.989259 glyphsets-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.905260 glyphsets-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-21 13:53:21.000000 glyphsets-0.6.0/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-21 13:53:21.000000 glyphsets-0.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-21 13:53:21.000000 glyphsets-0.6.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.905260 glyphsets-0.6.0/Archive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/Archive/GF Glyph Sets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.909260 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.929260 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.929260 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.909260 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/RECOMMENDED.md
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/TROUBLESHOOTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    75853 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104148 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/locl.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.933260 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    43666 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
--rw-r--r--   0 runner    (1001) docker     (123)    89964 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.937260 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (123)    35092 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/Directory.png
--rw-r--r--   0 runner    (1001) docker     (123)    98535 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
--rw-r--r--   0 runner    (1001) docker     (123)    84092 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
--rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    45217 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    53065 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/list-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-21 13:53:21.000000 glyphsets-0.6.0/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Arabic/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.913260 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.913260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.941260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.945260 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.945260 glyphsets-0.6.0/GF_glyphsets/Greek/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.945260 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    56469 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
--rw-r--r--   0 runner    (1001) docker     (123)    30534 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    26352 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Greek/nam/
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.917260 glyphsets-0.6.0/GF_glyphsets/Greek/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Latin/
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    38145 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
--rw-r--r--   0 runner    (1001) docker     (123)    62282 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    46764 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.953260 glyphsets-0.6.0/GF_glyphsets/Latin/nam/
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_African.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.917260 glyphsets-0.6.0/GF_glyphsets/Latin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Phonetics/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.917260 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.957260 glyphsets-0.6.0/GF_glyphsets/TransLatin/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/GF_glyphsets/TransLatin/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.917260 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 13:53:21.000000 glyphsets-0.6.0/GF_glyphsets/update-gs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-21 13:53:21.000000 glyphsets-0.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.921260 glyphsets-0.6.0/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/Lib/glyphsets/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/codepoints.py
--rw-r--r--   0 runner    (1001) docker     (123)   588153 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.989259 glyphsets-0.6.0/Lib/glyphsets/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   284694 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   298348 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   241902 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    46227 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    91251 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    80178 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   190939 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/math.nam
--rw-r--r--   0 runner    (1001) docker     (123)    95179 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    24495 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   117935 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   212192 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/wgl-latin.enc
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    29660 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-21 13:53:21.000000 glyphsets-0.6.0/Lib/glyphsets/test_strings.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.961260 glyphsets-0.6.0/Lib/glyphsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-21 13:53:37.000000 glyphsets-0.6.0/Lib/glyphsets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-21 13:53:37.989259 glyphsets-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-21 13:53:21.000000 glyphsets-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-21 13:53:21.000000 glyphsets-0.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.989259 glyphsets-0.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-21 13:53:21.000000 glyphsets-0.6.0/scripts/create-glyphset.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 13:53:37.989259 glyphsets-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-21 13:53:21.000000 glyphsets-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.989259 glyphsets-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:53:37.989259 glyphsets-0.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    90712 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/data/MavenPro[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/test_glyphdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/test_teststrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-21 13:53:21.000000 glyphsets-0.6.0/tests/testcoverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/RECOMMENDED.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    75853 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/locl.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    43666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
+-rw-r--r--   0 runner    (1001) docker     (123)    89964 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    35092 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/Directory.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98535 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84092 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53065 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-03 15:30:34.000000 glyphsets-0.6.1/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    56469 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    30534 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    26352 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    38180 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    62282 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    46764 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_African.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Phonetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/update-gs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 15:30:34.000000 glyphsets-0.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/Lib/glyphsets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/codepoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588180 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.916824 glyphsets-0.6.1/Lib/glyphsets/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    57487 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/batak_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/braille_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/carian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   284694 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   298348 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   241902 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    46227 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/greek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    91251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    80178 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/korean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    37112 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/latin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   190939 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/math.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    95179 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/math_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/miao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/modi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mro_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/multani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    24495 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/music_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/newa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nko_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/osage_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/runic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   117935 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/takri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   212192 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/thai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/toto_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/wgl-latin.enc
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    30939 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/yi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/test_strings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/Lib/glyphsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-03 15:30:47.920824 glyphsets-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-03 15:30:34.000000 glyphsets-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:30:34.000000 glyphsets-0.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 15:30:34.000000 glyphsets-0.6.1/scripts/create-glyphset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:30:47.920824 glyphsets-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    90712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/data/MavenPro[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_glyphdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_teststrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/testcoverage.py
```

### Comparing `glyphsets-0.6.0/.github/workflows/publish-release.yml` & `glyphsets-0.6.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/.github/workflows/test.yml` & `glyphsets-0.6.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Arabic/README.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-core.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/README.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/README.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/RECOMMENDED.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/RECOMMENDED.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/TROUBLESHOOTING.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/README.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/Vietnamese/img/locl.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt` & `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/README.md` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/Directory.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/Directory.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/ListFilters.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ListFilters.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-1.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-2.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-2.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/fix-3.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-3.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Archive/GF Glyph Sets/tutorials/img/list-filter.png` & `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/CHANGELOG.md` & `glyphsets-0.6.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/README.md` & `glyphsets-0.6.1/GF_glyphsets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist` & `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam` & `glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam` & `glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/README.md` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/README.md` & `glyphsets-0.6.1/GF_glyphsets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Core.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam` & `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt` & `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/README.md` & `glyphsets-0.6.1/GF_glyphsets/Latin/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist`

 * *Files 0% similar despite different names*

#### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist`

```diff
@@ -533,14 +533,15 @@
         <string>zmacronbelow</string>
         <string>wmod</string>
         <string>clickalveolar</string>
         <string>zmod</string>
         <string>commaabovecomb</string>
         <string>macronbelowcomb</string>
         <string>lowlinecomb</string>
+        <string>commaturnedmod</string>
         <string>glottalstopmod</string>
         <string>Ccircumflex</string>
         <string>Gcircumflex</string>
         <string>Hcircumflex</string>
         <string>Jcircumflex</string>
         <string>Scircumflex</string>
         <string>Tbar</string>
```

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {
-.appVersion = "3139";
+.appVersion = "3151";
 .formatVersion = 3;
 date = "2021-10-28 12:22:31 +0000";
 familyName = "GF Latin Minorities";
 fontMaster = (
 {
 id = m01;
 metricValues = (
@@ -1555,14 +1555,25 @@
 layerId = m01;
 width = 600;
 }
 );
 unicode = 700;
 },
 {
+glyphname = commaturnedmod;
+lastChange = "2023-03-17 14:37:04 +0000";
+layers = (
+{
+layerId = m01;
+width = 600;
+}
+);
+unicode = 699;
+},
+{
 color = 3;
 glyphname = glottalstopmod;
 lastChange = "2022-09-14 12:57:10 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
```

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_African.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_African.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 0x028A LATIN SMALL LETTER UPSILON
 0x0292 LATIN SMALL LETTER EZH
 0x0294 LATIN LETTER GLOTTAL STOP
 0x0295 LATIN LETTER PHARYNGEAL VOICED FRICATIVE
 0x02B7 MODIFIER LETTER SMALL W
 0x02B8 MODIFIER LETTER SMALL Y
 0x02B9 MODIFIER LETTER PRIME
+0x02BB MODIFIER LETTER TURNED COMMA
 0x02BC MODIFIER LETTER APOSTROPHE
 0x02C0 MODIFIER LETTER GLOTTAL STOP
 0x02C8 MODIFIER LETTER VERTICAL LINE
 0x0313 COMBINING COMMA ABOVE
 0x0315 COMBINING COMMA ABOVE RIGHT
 0x0323 COMBINING DOT BELOW
 0x0331 COMBINING MACRON BELOW
```

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Core.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam` & `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 zmacronbelow
 wmod
 clickalveolar
 zmod
 commaabovecomb
 macronbelowcomb
 lowlinecomb
+commaturnedmod
 glottalstopmod
 Ccircumflex
 Gcircumflex
 Hcircumflex
 Jcircumflex
 Scircumflex
 Tbar
```

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt`

 * *Files 14% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 zmacronbelow
 uni02B7
 uni01C2
 uni1DBB
 uni0313
 uni0331
 uni0332
+uni02BB
 uni02C0
 Ccircumflex
 Gcircumflex
 Hcircumflex
 Jcircumflex
 Scircumflex
 Tbar
```

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/README.md` & `glyphsets-0.6.1/GF_glyphsets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/GF_glyphsets/update-gs.sh` & `glyphsets-0.6.1/GF_glyphsets/update-gs.sh`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/LICENSE` & `glyphsets-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/__init__.py` & `glyphsets-0.6.1/Lib/glyphsets/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/__main__.py` & `glyphsets-0.6.1/Lib/glyphsets/__main__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/codepoints.py` & `glyphsets-0.6.1/Lib/glyphsets/codepoints.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/data.json` & `glyphsets-0.6.1/Lib/glyphsets/data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999915225500169%*

 * *Differences: {"'glyphs'": "{2221: {'glyphsets': {insert: [(1, 'GF_Latin_Beyond')]}}}"}*

```diff
@@ -20384,15 +20384,16 @@
             "nice_name": "fourthtonechinese",
             "production_name": "uni02CB",
             "unicode": 715
         },
         {
             "character": "\u02bb",
             "glyphsets": [
-                "GF_Latin_African"
+                "GF_Latin_African",
+                "GF_Latin_Beyond"
             ],
             "nice_name": "commaturnedmod",
             "production_name": "uni02BB",
             "unicode": 699
         },
         {
             "character": "\u02c0",
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/README.md` & `glyphsets-0.6.1/Lib/glyphsets/encodings/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/adlam_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/adlam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/ahom_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/ahom_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/armenian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/armenian_unique-glyphs.nam`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 0x0559 ՙ  ARMENIAN MODIFIER LETTER LEFT HALF RING
 0x055A ՚  ARMENIAN APOSTROPHE
 0x055B ՛  ARMENIAN EMPHASIS MARK
 0x055C ՜  ARMENIAN EXCLAMATION MARK
 0x055D ՝  ARMENIAN COMMA
 0x055E ՞  ARMENIAN QUESTION MARK
 0x055F ՟  ARMENIAN ABBREVIATION MARK
+0x0560 ՠ ARMENIAN SMALL LETTER TURNED AYB
 0x0561 ա  ARMENIAN SMALL LETTER AYB
 0x0562 բ  ARMENIAN SMALL LETTER BEN
 0x0563 գ  ARMENIAN SMALL LETTER GIM
 0x0564 դ  ARMENIAN SMALL LETTER DA
 0x0565 ե  ARMENIAN SMALL LETTER ECH
 0x0566 զ  ARMENIAN SMALL LETTER ZA
 0x0567 է  ARMENIAN SMALL LETTER EH
@@ -78,14 +79,15 @@
 0x0581 ց  ARMENIAN SMALL LETTER CO
 0x0582 ւ  ARMENIAN SMALL LETTER YIWN
 0x0583 փ  ARMENIAN SMALL LETTER PIWR
 0x0584 ք  ARMENIAN SMALL LETTER KEH
 0x0585 օ  ARMENIAN SMALL LETTER OH
 0x0586 ֆ  ARMENIAN SMALL LETTER FEH
 0x0587 և  ARMENIAN SMALL LIGATURE ECH YIWN
+0x0588 ֈ  ARMENIAN SMALL LETTER YI WITH STROKE
 0x0589 ։ ARMENIAN FULL STOP
 0x058A ֊  ARMENIAN HYPHEN
 0x058D ֍  RIGHT-FACING ARMENIAN ETERNITY SIGN
 0x058E ֎  LEFT-FACING ARMENIAN ETERNITY SIGN
 0x058F ֏  ARMENIAN DRAM SIGN
 0x2024 ․  ONE DOT LEADER
 0xFB13 ﬓ  ARMENIAN SMALL LIGATURE MEN NOW
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/avestan_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/avestan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/balinese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/balinese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/bamum_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/bamum_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/batak_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/batak_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/bengali_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/bengali_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 0x0964 । DEVANAGARI DANDA
 0x0965 ॥ DEVANAGARI DOUBLE DANDA
+0x0980 ঀ BENGALI ANJI
 0x0981 ঁ BENGALI SIGN CANDRABINDU
 0x0982 ং BENGALI SIGN ANUSVARA
 0x0983 ঃ BENGALI SIGN VISARGA
 0x0985 অ BENGALI LETTER A
 0x0986 আ BENGALI LETTER AA
 0x0987 ই BENGALI LETTER I
 0x0988 ঈ BENGALI LETTER II
@@ -88,12 +89,17 @@
 0x09F5 ৵ BENGALI CURRENCY NUMERATOR TWO
 0x09F6 ৶ BENGALI CURRENCY NUMERATOR THREE
 0x09F7 ৷ BENGALI CURRENCY NUMERATOR FOUR
 0x09F8 ৸ BENGALI CURRENCY NUMERATOR ONE LESS THAN THE DENOMINATOR
 0x09F9 ৹ BENGALI CURRENCY DENOMINATOR SIXTEEN
 0x09FA ৺ BENGALI ISSHAR
 0x09FB ৻ BENGALI GANDA MARK
+0x09FC ৼ BENGALI LETTER VEDIC ANUSVARA
+0x09FD ৽ BENGALI ABBREVIATION SIGN
+0x09FE ৾ BENGALI SANDHI MARK
+0x1CF7 ᳷ VEDIC SIGN ATIKRAMA
+0x1CFA ᳺ VEDIC SIGN DOUBLE ANUSVARA ANTARGOMUKHA
 0x200B ​ ZERO WIDTH SPACE
 0x200C ‌ ZERO WIDTH NON-JOINER
 0x200D ‍ ZERO WIDTH JOINER
 0x20B9 ₹ 
-0x25CC ◌ DOTTED CIRCLE
+0x25CC ◌ DOTTED CIRCLE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/buginese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/buginese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/buhid_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/buhid_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-0x0000 
-0x000D 
+0x0000 <control>
+0x000D <control>
 0x0020 SPACE
 0x00A0 NO-BREAK SPACE
 0x0131 LATIN SMALL LETTER DOTLESS I
 0x02C7 CARON
 0x02D8 BREVE
 0x02D9 DOT ABOVE
 0x02DA RING ABOVE
@@ -715,8 +715,23 @@
 0x18EF CANADIAN SYLLABICS CARRIER GAA
 0x18F0 CANADIAN SYLLABICS CARRIER GWA
 0x18F1 CANADIAN SYLLABICS SAYISI JUU
 0x18F2 CANADIAN SYLLABICS CARRIER JWA
 0x18F3 CANADIAN SYLLABICS BEAVER DENE L
 0x18F4 CANADIAN SYLLABICS BEAVER DENE R
 0x18F5 CANADIAN SYLLABICS CARRIER DENTAL S
-0x25CC DOTTED CIRCLE
+0x11AB0 CANADIAN SYLLABICS NATTILIK HI
+0x11AB1 CANADIAN SYLLABICS NATTILIK HII
+0x11AB2 CANADIAN SYLLABICS NATTILIK HO
+0x11AB3 CANADIAN SYLLABICS NATTILIK HOO
+0x11AB4 CANADIAN SYLLABICS NATTILIK HA
+0x11AB5 CANADIAN SYLLABICS NATTILIK HAA
+0x11AB6 CANADIAN SYLLABICS NATTILIK SHRI
+0x11AB7 CANADIAN SYLLABICS NATTILIK SHRII
+0x11AB8 CANADIAN SYLLABICS NATTILIK SHRO
+0x11AB9 CANADIAN SYLLABICS NATTILIK SHROO
+0x11ABA CANADIAN SYLLABICS NATTILIK SHRA
+0x11ABB CANADIAN SYLLABICS NATTILIK SHRAA
+0x11ABC CANADIAN SYLLABICS SPE
+0x11ABD CANADIAN SYLLABICS SPI
+0x11ABE CANADIAN SYLLABICS SPO
+0x11ABF CANADIAN SYLLABICS SPA
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/carian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/carian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/chakma_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/chakma_unique-glyphs.nam`

 * *Files 1% similar despite different names*

```diff
@@ -91,7 +91,8 @@
 0x11140 CHAKMA SECTION MARK
 0x11141 CHAKMA DANDA
 0x11142 CHAKMA DOUBLE DANDA
 0x11143 CHAKMA QUESTION MARK
 0x11144 CHAKMA LETTER LHAA
 0x11145 CHAKMA VOWEL SIGN AA
 0x11146 CHAKMA VOWEL SIGN EI
+0x11147 CHAKMA LETTER VAA
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cham_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/coptic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/coptic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/deseret_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/deseret_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
 0x1CF0 ᳰ VEDIC SIGN RTHANG LONG ANUSVARA
 0x1CF1 ᳱ VEDIC SIGN ANUSVARA UBHAYATO MUKHA
 0x1CF2 ᳲ VEDIC SIGN ARDHAVISARGA
 0x1CF3 ᳳ 
 0x1CF4 ᳴ 
 0x1CF5 ᳵ 
 0x1CF6 ᳶ 
+0x1CF7 ᳷ VEDIC SIGN ATIKRAMA
 0x1CF8 ᳸ 
 0x1CF9 ᳹ 
 0x200B ​ ZERO WIDTH SPACE
 0x200C ‌ ZERO WIDTH NON-JOINER
 0x200D ‍ ZERO WIDTH JOINER
 0x2044 ⁄ FRACTION SLASH
 0x20A8 ₨ RUPEE SIGN
@@ -209,7 +210,11 @@
 0xA8F5 ꣵ DEVANAGARI SIGN CANDRABINDU TWO
 0xA8F6 ꣶ DEVANAGARI SIGN CANDRABINDU THREE
 0xA8F7 ꣷ DEVANAGARI SIGN CANDRABINDU AVAGRAHA
 0xA8F8 ꣸ DEVANAGARI SIGN PUSHPIKA
 0xA8F9 ꣹ DEVANAGARI GAP FILLER
 0xA8FA ꣺ DEVANAGARI CARET
 0xA8FB ꣻ DEVANAGARI HEADSTROKE
+0xA8FC  ꣼ DEVANAGARI SIGN SIDDHAM
+0xA8FD  ꣽ DEVANAGARI JAIN OM
+0xA8FE  ꣾ DEVANAGARI LETTER AY
+0xA8FF  ◌ꣿ DEVANAGARI VOWEL SIGN AY
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/dogra_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/dogra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/duployan_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/duployan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam`

 * *Files 10% similar despite different names*

```diff
@@ -489,7 +489,35 @@
 0xAB28 ꬨ
 0xAB29 ꬩ
 0xAB2A ꬪ
 0xAB2B ꬫ
 0xAB2C ꬬ
 0xAB2D ꬭ
 0xAB2E ꬮ
+0x1E7E0  𞟠 ETHIOPIC SYLLABLE HHYA
+0x1E7E1  𞟡 ETHIOPIC SYLLABLE HHYU
+0x1E7E2  𞟢 ETHIOPIC SYLLABLE HHYI
+0x1E7E3  𞟣 ETHIOPIC SYLLABLE HHYAA
+0x1E7E4  𞟤 ETHIOPIC SYLLABLE HHYEE
+0x1E7E5  𞟥 ETHIOPIC SYLLABLE HHYE
+0x1E7E6  𞟦 ETHIOPIC SYLLABLE HHYO
+0x1E7E8  𞟨 ETHIOPIC SYLLABLE GURAGE HHWA
+0x1E7E9  𞟩 ETHIOPIC SYLLABLE HHWI
+0x1E7EA  𞟪 ETHIOPIC SYLLABLE HHWEE
+0x1E7EB  𞟫 ETHIOPIC SYLLABLE HHWE
+0x1E7ED  𞟭 ETHIOPIC SYLLABLE GURAGE MWI
+0x1E7EE  𞟮 ETHIOPIC SYLLABLE GURAGE MWEE
+0x1E7F0  𞟰 ETHIOPIC SYLLABLE GURAGE QWI
+0x1E7F1  𞟱 ETHIOPIC SYLLABLE GURAGE QWEE
+0x1E7F2  𞟲 ETHIOPIC SYLLABLE GURAGE QWE
+0x1E7F3  𞟳 ETHIOPIC SYLLABLE GURAGE BWI
+0x1E7F4  𞟴 ETHIOPIC SYLLABLE GURAGE BWEE
+0x1E7F5  𞟵 ETHIOPIC SYLLABLE GURAGE KWI
+0x1E7F6  𞟶 ETHIOPIC SYLLABLE GURAGE KWEE
+0x1E7F7  𞟷 ETHIOPIC SYLLABLE GURAGE KWE
+0x1E7F8  𞟸 ETHIOPIC SYLLABLE GURAGE GWI
+0x1E7F9  𞟹 ETHIOPIC SYLLABLE GURAGE GWEE
+0x1E7FA  𞟺 ETHIOPIC SYLLABLE GURAGE GWE
+0x1E7FB  𞟻 ETHIOPIC SYLLABLE GURAGE FWI
+0x1E7FC  𞟼 ETHIOPIC SYLLABLE GURAGE FWEE
+0x1E7FD  𞟽 ETHIOPIC SYLLABLE GURAGE PWI
+0x1E7FE  𞟾 ETHIOPIC SYLLABLE GURAGE PWEE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/gothic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/gothic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/grantha_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/grantha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/greek_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/greek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam`

 * *Files 7% similar despite different names*

```diff
@@ -80,14 +80,21 @@
 0x0AEB  ૫ GUJARATI DIGIT FIVE
 0x0AEC  ૬ GUJARATI DIGIT SIX
 0x0AED  ૭ GUJARATI DIGIT SEVEN
 0x0AEE  ૮ GUJARATI DIGIT EIGHT
 0x0AEF  ૯ GUJARATI DIGIT NINE
 0x0AF0  ૰ 
 0x0AF1  ૱ GUJARATI RUPEE SIGN
+0x0AF9  ૹ GUJARATI LETTER ZHA
+0x0AFA  ◌ૺ GUJARATI SIGN SUKUN
+0x0AFB  ◌ૻ GUJARATI SIGN SHADDA
+0x0AFC  ◌ૼ GUJARATI SIGN MADDAH
+0x0AFD  ◌૽ GUJARATI SIGN THREE-DOT NUKTA ABOVE
+0x0AFE  ◌૾ GUJARATI SIGN CIRCLE NUKTA ABOVE
+0x0AFF  ◌૿ GUJARATI SIGN TWO-CIRCLE NUKTA ABOVE
 0x200B  ​ ZERO WIDTH SPACE
 0x200C  ‌ ZERO WIDTH NON-JOINER
 0x200D  ‍ ZERO WIDTH JOINER
 0x20B9  ₹ 
 0x25CC  ◌ DOTTED CIRCLE
 0xA830  ꠰ NORTH INDIC FRACTION ONE QUARTER
 0xA831  ꠱ NORTH INDIC FRACTION ONE HALF
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 0x0A6F  ੯ GURMUKHI DIGIT NINE
 0x0A70  ੰ GURMUKHI TIPPI
 0x0A71  ੱ GURMUKHI ADDAK
 0x0A72  ੲ GURMUKHI IRI
 0x0A73  ੳ GURMUKHI URA
 0x0A74  ੴ GURMUKHI EK ONKAR
 0x0A75  ੵ GURMUKHI SIGN YAKASH
+0x0A76  ੶ GURMUKHI ABBREVIATION SIGN
 0x200B  ​ ZERO WIDTH SPACE
 0x200C  ‌ ZERO WIDTH NON-JOINER
 0x200D  ‍ ZERO WIDTH JOINER
 0x20B9  ₹ 
 0x25CC  ◌ DOTTED CIRCLE
 0x262C  ☬ ADI SHAKTI
 0xA830  ꠰ NORTH INDIC FRACTION ONE QUARTER
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/hatran_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/hatran_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/japanese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/japanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/javanese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/javanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/kannada_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/kannada_unique-glyphs.nam`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 0x0964  । DEVANAGARI DANDA
 0x0965  ॥ DEVANAGARI DOUBLE DANDA
+0x0C80  ಀ KANNADA SIGN SPACING CANDRABINDU
+0x0C81  ◌ಁ KANNADA SIGN CANDRABINDU
 0x0C82  ಂ KANNADA SIGN ANUSVARA
 0x0C83  ಃ KANNADA SIGN VISARGA
+0x0C84  ಄ KANNADA SIGN SIDDHAM
 0x0C85  ಅ KANNADA LETTER A
 0x0C86  ಆ KANNADA LETTER AA
 0x0C87  ಇ KANNADA LETTER I
 0x0C88  ಈ KANNADA LETTER II
 0x0C89  ಉ KANNADA LETTER U
 0x0C8A  ಊ KANNADA LETTER UU
 0x0C8B  ಋ KANNADA LETTER VOCALIC R
@@ -65,14 +68,15 @@
 0x0CC8  ೈ KANNADA VOWEL SIGN AI
 0x0CCA  ೊ KANNADA VOWEL SIGN O
 0x0CCB  ೋ KANNADA VOWEL SIGN OO
 0x0CCC  ೌ KANNADA VOWEL SIGN AU
 0x0CCD  ್ KANNADA SIGN VIRAMA
 0x0CD5  ೕ KANNADA LENGTH MARK
 0x0CD6  ೖ KANNADA AI LENGTH MARK
+0x0CDD  ೝ KANNADA LETTER NAKAARA POLLU
 0x0CDE  ೞ KANNADA LETTER FA
 0x0CE0  ೠ KANNADA LETTER VOCALIC RR
 0x0CE1  ೡ KANNADA LETTER VOCALIC LL
 0x0CE2  ೢ KANNADA VOWEL SIGN VOCALIC L
 0x0CE3  ೣ KANNADA VOWEL SIGN VOCALIC LL
 0x0CE6  ೦ KANNADA DIGIT ZERO
 0x0CE7  ೧ KANNADA DIGIT ONE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/khojki_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/khojki_unique-glyphs.nam`

 * *Files 1% similar despite different names*

```diff
@@ -83,7 +83,8 @@
 0x11238 KHOJKI DANDA
 0x11239 KHOJKI DOUBLE DANDA
 0x1123A KHOJKI WORD SEPARATOR
 0x1123B KHOJKI SECTION MARK
 0x1123C KHOJKI DOUBLE SECTION MARK
 0x1123D KHOJKI ABBREVIATION SIGN
 0x1123E KHOJKI SIGN SUKUN
+0x11241 KHOJKI VOWEL SIGN VOCALIC R
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/korean_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/korean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/lao_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/lao_unique-glyphs.nam`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 #Copied from https://github.com/google/fonts/blob/master/tools/encodings/lao_unique-glyphs.nam
 0x0E81 LAO LETTER KO
 0x0E82 LAO LETTER KHO SUNG
 0x0E84 LAO LETTER KHO TAM
+0x0E86 LAO LETTER PALI GHA
 0x0E87 LAO LETTER NGO
 0x0E88 LAO LETTER CO
+0x0E89 LAO LETTER PALI CHA
 0x0E8A LAO LETTER SO TAM
+0x0E8C LAO LETTER PALI JHA
 0x0E8D LAO LETTER NYO
+0x0E8E LAO LETTER PALI NYA
+0x0E8F LAO LETTER PALI TTA
+0x0E90 LAO LETTER PALI TTHA
+0x0E91 LAO LETTER PALI DDA
+0x0E92 LAO LETTER PALI DDHA
+0x0E93 LAO LETTER PALI NNA
 0x0E94 LAO LETTER DO
 0x0E95 LAO LETTER TO
 0x0E96 LAO LETTER THO SUNG
 0x0E97 LAO LETTER THO TAM
+0x0E98 LAO LETTER PALI DHA
 0x0E99 LAO LETTER NO
 0x0E9A LAO LETTER BO
 0x0E9B LAO LETTER PO
 0x0E9C LAO LETTER PHO SUNG
 0x0E9D LAO LETTER FO TAM
 0x0E9E LAO LETTER PHO TAM
 0x0E9F LAO LETTER FO SUNG
+0x0EA0 LAO LETTER PALI BHA
 0x0EA1 LAO LETTER MO
 0x0EA2 LAO LETTER YO
 0x0EA3 LAO LETTER LO LING
 0x0EA5 LAO LETTER LO LOOT
 0x0EA7 LAO LETTER WO
+0x0EA8 LAO LETTER SANSKRIT SHA
+0x0EA9 LAO LETTER SANSKRIT SSA
 0x0EAA LAO LETTER SO SUNG
 0x0EAB LAO LETTER HO SUNG
+0x0EAC LAO LETTER PALI LLA
 0x0EAD LAO LETTER O
 0x0EAE LAO LETTER HO TAM
 0x0EAF LAO ELLIPSIS
 0x0EB0 LAO VOWEL SIGN A
 0x0EB1 LAO VOWEL SIGN MAI KAN
 0x0EB2 LAO VOWEL SIGN AA
 0x0EB3 LAO VOWEL SIGN AM
 0x0EB4 LAO VOWEL SIGN I
 0x0EB5 LAO VOWEL SIGN II
 0x0EB6 LAO VOWEL SIGN Y
 0x0EB7 LAO VOWEL SIGN YY
 0x0EB8 LAO VOWEL SIGN U
 0x0EB9 LAO VOWEL SIGN UU
+0x0EBA LAO SIGN PALI VIRAMA
 0x0EBB LAO VOWEL SIGN MAI KON
 0x0EBC LAO SEMIVOWEL SIGN LO
 0x0EBD LAO SEMIVOWEL SIGN NYO
 0x0EC0 LAO VOWEL SIGN E
 0x0EC1 LAO VOWEL SIGN EI
 0x0EC2 LAO VOWEL SIGN O
 0x0EC3 LAO VOWEL SIGN AY
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam`

 * *Files 6% similar despite different names*

```diff
@@ -327,15 +327,110 @@
 0x0249  ɉ LATIN SMALL LETTER J WITH STROKE
 0x024A  Ɋ LATIN CAPITAL LETTER SMALL Q WITH HOOK TAIL
 0x024B  ɋ LATIN SMALL LETTER Q WITH HOOK TAIL
 0x024C  Ɍ LATIN CAPITAL LETTER R WITH STROKE
 0x024D  ɍ LATIN SMALL LETTER R WITH STROKE
 0x024E  Ɏ LATIN CAPITAL LETTER Y WITH STROKE
 0x024F  ɏ LATIN SMALL LETTER Y WITH STROKE
+0x0250  ɐ LATIN SMALL LETTER TURNED A
+0x0251  ɑ LATIN SMALL LETTER ALPHA
+0x0252  ɒ LATIN SMALL LETTER TURNED ALPHA
+0x0253  ɓ LATIN SMALL LETTER B WITH HOOK
+0x0254  ɔ LATIN SMALL LETTER OPEN O
+0x0255  ɕ LATIN SMALL LETTER C WITH CURL
+0x0256  ɖ LATIN SMALL LETTER D WITH TAIL
+0x0257  ɗ LATIN SMALL LETTER D WITH HOOK
+0x0258  ɘ LATIN SMALL LETTER REVERSED E
 0x0259  ə LATIN SMALL LETTER SCHWA
+0x025A  ɚ LATIN SMALL LETTER SCHWA WITH HOOK
+0x025B  ɛ LATIN SMALL LETTER OPEN E
+0x025C  ɜ LATIN SMALL LETTER REVERSED OPEN E
+0x025D  ɝ LATIN SMALL LETTER REVERSED OPEN E WITH HOOK
+0x025E  ɞ LATIN SMALL LETTER CLOSED REVERSED OPEN E
+0x025F  ɟ LATIN SMALL LETTER DOTLESS J WITH STROKE
+0x0260  ɠ LATIN SMALL LETTER G WITH HOOK
+0x0261  ɡ LATIN SMALL LETTER SCRIPT G
+0x0262  ɢ LATIN LETTER SMALL CAPITAL G
+0x0263  ɣ LATIN SMALL LETTER GAMMA
+0x0264  ɤ LATIN SMALL LETTER RAMS HORN
+0x0265  ɥ LATIN SMALL LETTER TURNED H
+0x0266  ɦ LATIN SMALL LETTER H WITH HOOK
+0x0267  ɧ LATIN SMALL LETTER HENG WITH HOOK
+0x0268  ɨ LATIN SMALL LETTER I WITH STROKE
+0x0269  ɩ LATIN SMALL LETTER IOTA
+0x026A  ɪ LATIN LETTER SMALL CAPITAL I
+0x026B  ɫ LATIN SMALL LETTER L WITH MIDDLE TILDE
+0x026C  ɬ LATIN SMALL LETTER L WITH BELT
+0x026D  ɭ LATIN SMALL LETTER L WITH RETROFLEX HOOK
+0x026E  ɮ LATIN SMALL LETTER LEZH
+0x026F  ɯ LATIN SMALL LETTER TURNED M
+0x0270  ɰ LATIN SMALL LETTER TURNED M WITH LONG LEG
+0x0271  ɱ LATIN SMALL LETTER M WITH HOOK
+0x0272  ɲ LATIN SMALL LETTER N WITH LEFT HOOK
+0x0273  ɳ LATIN SMALL LETTER N WITH RETROFLEX HOOK
+0x0274  ɴ LATIN LETTER SMALL CAPITAL N
+0x0275  ɵ LATIN SMALL LETTER BARRED O
+0x0276  ɶ LATIN LETTER SMALL CAPITAL OE
+0x0277  ɷ LATIN SMALL LETTER CLOSED OMEGA
+0x0278  ɸ LATIN SMALL LETTER PHI
+0x0279  ɹ LATIN SMALL LETTER TURNED R
+0x027A  ɺ LATIN SMALL LETTER TURNED R WITH LONG LEG
+0x027B  ɻ LATIN SMALL LETTER TURNED R WITH HOOK
+0x027C  ɼ LATIN SMALL LETTER R WITH LONG LEG
+0x027D  ɽ LATIN SMALL LETTER R WITH TAIL
+0x027E  ɾ LATIN SMALL LETTER R WITH FISHHOOK
+0x027F  ɿ LATIN SMALL LETTER REVERSED R WITH FISHHOOK
+0x0280  ʀ LATIN LETTER SMALL CAPITAL R
+0x0281  ʁ LATIN LETTER SMALL CAPITAL INVERTED R
+0x0282  ʂ LATIN SMALL LETTER S WITH HOOK
+0x0283  ʃ LATIN SMALL LETTER ESH
+0x0284  ʄ LATIN SMALL LETTER DOTLESS J WITH STROKE AND HOOK
+0x0285  ʅ LATIN SMALL LETTER SQUAT REVERSED ESH
+0x0286  ʆ LATIN SMALL LETTER ESH WITH CURL
+0x0287  ʇ LATIN SMALL LETTER TURNED T
+0x0288  ʈ LATIN SMALL LETTER T WITH RETROFLEX HOOK
+0x0289  ʉ LATIN SMALL LETTER U BAR
+0x028A  ʊ LATIN SMALL LETTER UPSILON
+0x028B  ʋ LATIN SMALL LETTER V WITH HOOK
+0x028C  ʌ LATIN SMALL LETTER TURNED V
+0x028D  ʍ LATIN SMALL LETTER TURNED W
+0x028E  ʎ LATIN SMALL LETTER TURNED Y
+0x028F  ʏ LATIN LETTER SMALL CAPITAL Y
+0x0290  ʐ LATIN SMALL LETTER Z WITH RETROFLEX HOOK
+0x0291  ʑ LATIN SMALL LETTER Z WITH CURL
+0x0292  ʒ LATIN SMALL LETTER EZH
+0x0293  ʓ LATIN SMALL LETTER EZH WITH CURL
+0x0294  ʔ LATIN LETTER GLOTTAL STOP
+0x0295  ʕ LATIN LETTER PHARYNGEAL VOICED FRICATIVE
+0x0296  ʖ LATIN LETTER INVERTED GLOTTAL STOP
+0x0297  ʗ LATIN LETTER STRETCHED C
+0x0298  ʘ LATIN LETTER BILABIAL CLICK
+0x0299  ʙ LATIN LETTER SMALL CAPITAL B
+0x029A  ʚ LATIN SMALL LETTER CLOSED OPEN E
+0x029B  ʛ LATIN LETTER SMALL CAPITAL G WITH HOOK
+0x029C  ʜ LATIN LETTER SMALL CAPITAL H
+0x029D  ʝ LATIN SMALL LETTER J WITH CROSSED-TAIL
+0x029E  ʞ LATIN SMALL LETTER TURNED K
+0x029F  ʟ LATIN LETTER SMALL CAPITAL L
+0x02A0  ʠ LATIN SMALL LETTER Q WITH HOOK
+0x02A1  ʡ LATIN LETTER GLOTTAL STOP WITH STROKE
+0x02A2  ʢ LATIN LETTER REVERSED GLOTTAL STOP WITH STROKE
+0x02A3  ʣ LATIN SMALL LETTER DZ DIGRAPH
+0x02A4  ʤ LATIN SMALL LETTER DEZH DIGRAPH
+0x02A5  ʥ LATIN SMALL LETTER DZ DIGRAPH WITH CURL
+0x02A6  ʦ LATIN SMALL LETTER TS DIGRAPH
+0x02A7  ʧ LATIN SMALL LETTER TESH DIGRAPH
+0x02A8  ʨ LATIN SMALL LETTER TC DIGRAPH WITH CURL
+0x02A9  ʩ LATIN SMALL LETTER FENG DIGRAPH
+0x02AA  ʪ LATIN SMALL LETTER LS DIGRAPH
+0x02AB  ʫ LATIN SMALL LETTER LZ DIGRAPH
+0x02AC  ʬ LATIN LETTER BILABIAL PERCUSSIVE
+0x02AD  ʭ LATIN LETTER BIDENTAL PERCUSSIVE
+0x02AE  ʮ LATIN SMALL LETTER TURNED H WITH FISHHOOK
+0x02AF  ʯ LATIN SMALL LETTER TURNED H WITH FISHHOOK AND TAIL
 0x1E00  Ḁ LATIN CAPITAL LETTER A WITH RING BELOW
 0x1E01  ḁ LATIN SMALL LETTER A WITH RING BELOW
 0x1E02  Ḃ LATIN CAPITAL LETTER B WITH DOT ABOVE
 0x1E03  ḃ LATIN SMALL LETTER B WITH DOT ABOVE
 0x1E04  Ḅ LATIN CAPITAL LETTER B WITH DOT BELOW
 0x1E05  ḅ LATIN SMALL LETTER B WITH DOT BELOW
 0x1E06  Ḇ LATIN CAPITAL LETTER B WITH LINE BELOW
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/latin_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/latin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/limbu_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/limbu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/lisu_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/lisu_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -52,7 +52,8 @@
 0xA4F9 LISU LETTER TONE NA PO
 0xA4FA LISU LETTER TONE MYA CYA
 0xA4FB LISU LETTER TONE MYA BO
 0xA4FC LISU LETTER TONE MYA NA
 0xA4FD LISU LETTER TONE MYA JEU
 0xA4FE LISU PUNCTUATION COMMA
 0xA4FF LISU PUNCTUATION FULL STOP
+0x11FB0 LISU LETTER YHA
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/lycian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/lycian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/lydian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/lydian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 0x0307  ̇ COMBINING DOT ABOVE
 0x0323  ̣ COMBINING DOT BELOW
 0x0964  । DEVANAGARI DANDA
 0x0965  ॥ DEVANAGARI DOUBLE DANDA
+0x0D00  ◌ഀ MALAYALAM SIGN COMBINING ANUSVARA ABOVE
+0x0D01  ◌ഁ MALAYALAM SIGN CANDRABINDU
 0x0D02  ം MALAYALAM SIGN ANUSVARA
 0x0D03  ഃ MALAYALAM SIGN VISARGA
+0x0D04  ഄ MALAYALAM LETTER VEDIC ANUSVARA
 0x0D05  അ MALAYALAM LETTER A
 0x0D06  ആ MALAYALAM LETTER AA
 0x0D07  ഇ MALAYALAM LETTER I
 0x0D08  ഈ MALAYALAM LETTER II
 0x0D09  ഉ MALAYALAM LETTER U
 0x0D0A  ഊ MALAYALAM LETTER UU
 0x0D0B  ഋ MALAYALAM LETTER VOCALIC R
@@ -52,14 +55,16 @@
 0x0D34  ഴ MALAYALAM LETTER LLLA
 0x0D35  വ MALAYALAM LETTER VA
 0x0D36  ശ MALAYALAM LETTER SHA
 0x0D37  ഷ MALAYALAM LETTER SSA
 0x0D38  സ MALAYALAM LETTER SA
 0x0D39  ഹ MALAYALAM LETTER HA
 0x0D3A  ഺ 
+0x0D3B  ◌഻ MALAYALAM SIGN VERTICAL BAR VIRAMA
+0x0D3C  ◌഼ MALAYALAM SIGN CIRCULAR VIRAMA
 0x0D3D  ഽ MALAYALAM SIGN AVAGRAHA
 0x0D3E  ാ MALAYALAM VOWEL SIGN AA
 0x0D3F  ി MALAYALAM VOWEL SIGN I
 0x0D40  ീ MALAYALAM VOWEL SIGN II
 0x0D41  ു MALAYALAM VOWEL SIGN U
 0x0D42  ൂ MALAYALAM VOWEL SIGN UU
 0x0D43  ൃ MALAYALAM VOWEL SIGN VOCALIC R
@@ -68,16 +73,27 @@
 0x0D47  േ MALAYALAM VOWEL SIGN EE
 0x0D48  ൈ MALAYALAM VOWEL SIGN AI
 0x0D4A  ൊ MALAYALAM VOWEL SIGN O
 0x0D4B  ോ MALAYALAM VOWEL SIGN OO
 0x0D4C  ൌ MALAYALAM VOWEL SIGN AU
 0x0D4D  ് MALAYALAM SIGN VIRAMA
 0x0D4E  ൎ 
+0x0D4F  ൏ MALAYALAM SIGN PARA
+0x0D54  ൔ MALAYALAM LETTER CHILLU M
+0x0D55  ൕ MALAYALAM LETTER CHILLU Y
+0x0D56  ൖ MALAYALAM LETTER CHILLU LLL
 0x0D57  ൗ MALAYALAM AU LENGTH MARK
-0x0D60  ൠ MALAYALAM LETTER VOCALIC RR
+0x0D58  ൘ MALAYALAM FRACTION ONE ONE-HUNDRED-AND-SIXTIETH
+0x0D59  ൙ MALAYALAM FRACTION ONE FORTIETH
+0x0D5A  ൚ MALAYALAM FRACTION THREE EIGHTIETHS
+0x0D5B  ൛ MALAYALAM FRACTION ONE TWENTIETH
+0x0D5C  ൜ MALAYALAM FRACTION ONE TENTH
+0x0D5D  ൝ MALAYALAM FRACTION THREE TWENTIETHS
+0x0D5E  ൞ MALAYALAM FRACTION ONE FIFTH
+0x0D5F  ൟ MALAYALAM LETTER ARCHAIC II0x0D60  ൠ MALAYALAM LETTER VOCALIC RR
 0x0D61  ൡ MALAYALAM LETTER VOCALIC LL
 0x0D62  ൢ MALAYALAM VOWEL SIGN VOCALIC L
 0x0D63  ൣ MALAYALAM VOWEL SIGN VOCALIC LL
 0x0D66  ൦ MALAYALAM DIGIT ZERO
 0x0D67  ൧ MALAYALAM DIGIT ONE
 0x0D68  ൨ MALAYALAM DIGIT TWO
 0x0D69  ൩ MALAYALAM DIGIT THREE
@@ -89,14 +105,17 @@
 0x0D6F  ൯ MALAYALAM DIGIT NINE
 0x0D70  ൰ MALAYALAM NUMBER TEN
 0x0D71  ൱ MALAYALAM NUMBER ONE HUNDRED
 0x0D72  ൲ MALAYALAM NUMBER ONE THOUSAND
 0x0D73  ൳ MALAYALAM FRACTION ONE QUARTER
 0x0D74  ൴ MALAYALAM FRACTION ONE HALF
 0x0D75  ൵ MALAYALAM FRACTION THREE QUARTERS
+0x0D76  ൶ MALAYALAM FRACTION ONE SIXTEENTH
+0x0D77  ൷ MALAYALAM FRACTION ONE EIGHTH
+0x0D78  ൸ MALAYALAM FRACTION THREE SIXTEENTHS
 0x0D79  ൹ MALAYALAM DATE MARK
 0x0D7A  ൺ MALAYALAM LETTER CHILLU NN
 0x0D7B  ൻ MALAYALAM LETTER CHILLU N
 0x0D7C  ർ MALAYALAM LETTER CHILLU RR
 0x0D7D  ൽ MALAYALAM LETTER CHILLU L
 0x0D7E  ൾ MALAYALAM LETTER CHILLU LL
 0x0D7F  ൿ MALAYALAM LETTER CHILLU K
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/marchen_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/marchen_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/math.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/math.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/math_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/math_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/miao_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/miao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/modi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/modi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/mro_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/mro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/multani_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/multani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/music_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/music_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam`

 * *Files 1% similar despite different names*

```diff
@@ -221,7 +221,8 @@
 0xAA78 MYANMAR SYMBOL AITON ONE
 0xAA79 MYANMAR SYMBOL AITON TWO
 0xAA7A MYANMAR LETTER AITON RA
 0xAA7B MYANMAR SIGN PAO KAREN TONE
 0xAA7C MYANMAR SIGN TAI LAING TONE-2
 0xAA7D MYANMAR SIGN TAI LAING TONE-5
 0xAA7E MYANMAR LETTER SHWE PALAUNG CHA
+0xAA7F MYANMAR LETTER SHWE PALAUNG SHA
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/newa_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/newa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/nko_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/nko_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/nushu_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/nushu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/ogham_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/ogham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/oriya_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/oriya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/osage_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/osage_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/rejang_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/rejang_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/runic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/runic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/sharada_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/sharada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/shavian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/shavian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/siddham_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/siddham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/symbols_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/symbols_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/syriac_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/syriac_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam`

 * *Files 19% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 0x1706 TAGALOG LETTER TA
 0x1707 TAGALOG LETTER DA
 0x1708 TAGALOG LETTER NA
 0x1709 TAGALOG LETTER PA
 0x170A TAGALOG LETTER BA
 0x170B TAGALOG LETTER MA
 0x170C TAGALOG LETTER YA
+0x170D TAGALOG LETTER RA
 0x170E TAGALOG LETTER LA
 0x170F TAGALOG LETTER WA
 0x1710 TAGALOG LETTER SA
 0x1711 TAGALOG LETTER HA
 0x1712 TAGALOG VOWEL SIGN I
 0x1713 TAGALOG VOWEL SIGN U
 0x1714 TAGALOG SIGN VIRAMA
+0x1715 TAGALOG SIGN PAMUDPOD
+0x171F TAGALOG LETTER ARCHAIC RA
 0x1735 PHILIPPINE SINGLE PUNCTUATION
 0x1736 PHILIPPINE DOUBLE PUNCTUATION
 0x200B ZERO WIDTH SPACE
 0x200C ZERO WIDTH NON-JOINER
 0x200D ZERO WIDTH JOINER
 0x25CC DOTTED CIRCLE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/takri_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/takri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tamil_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tamil_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,95 @@
 0x0020 SPACE
 0x00A0 NO-BREAK SPACE
+0x0000   <control>
+0x000D   <control>
+0x0020   SPACE
+0x00A0   NO-BREAK SPACE
+0x16A70  𖩰 TANGSA LETTER OZ
+0x16A71  𖩱 TANGSA LETTER OC
+0x16A72  𖩲 TANGSA LETTER OQ
+0x16A73  𖩳 TANGSA LETTER OX
+0x16A74  𖩴 TANGSA LETTER AZ
+0x16A75  𖩵 TANGSA LETTER AC
+0x16A76  𖩶 TANGSA LETTER AQ
+0x16A77  𖩷 TANGSA LETTER AX
+0x16A78  𖩸 TANGSA LETTER VZ
+0x16A79  𖩹 TANGSA LETTER VC
+0x16A7A  𖩺 TANGSA LETTER VQ
+0x16A7B  𖩻 TANGSA LETTER VX
+0x16A7C  𖩼 TANGSA LETTER EZ
+0x16A7D  𖩽 TANGSA LETTER EC
+0x16A7E  𖩾 TANGSA LETTER EQ
+0x16A7F  𖩿 TANGSA LETTER EX
 0x16A80  𖪀 TANGSA LETTER IZ
+0x16A81  𖪁 TANGSA LETTER IC
 0x16A82  𖪂 TANGSA LETTER IQ
 0x16A83  𖪃 TANGSA LETTER IX
 0x16A84  𖪄 TANGSA LETTER UZ
 0x16A85  𖪅 TANGSA LETTER UC
 0x16A86  𖪆 TANGSA LETTER UQ
 0x16A87  𖪇 TANGSA LETTER UX
+0x16A88  𖪈 TANGSA LETTER AWZ
+0x16A89  𖪉 TANGSA LETTER AWC
+0x16A8A  𖪊 TANGSA LETTER AWQ
+0x16A8B  𖪋 TANGSA LETTER AWX
 0x16A8C  𖪌 TANGSA LETTER UIZ
 0x16A8D  𖪍 TANGSA LETTER UIC
+0x16A8E  𖪎 TANGSA LETTER UIQ
 0x16A8F  𖪏 TANGSA LETTER UIX
 0x16A90  𖪐 TANGSA LETTER FINAL NG
+0x16A91  𖪑 TANGSA LETTER LONG UEX
 0x16A92  𖪒 TANGSA LETTER SHORT UEZ
+0x16A93  𖪓 TANGSA LETTER SHORT AWX
+0x16A94  𖪔 TANGSA LETTER UEC
 0x16A95  𖪕 TANGSA LETTER UEZ
 0x16A96  𖪖 TANGSA LETTER UEQ
 0x16A97  𖪗 TANGSA LETTER UEX
 0x16A98  𖪘 TANGSA LETTER UIUZ
 0x16A99  𖪙 TANGSA LETTER UIUC
+0x16A9A  𖪚 TANGSA LETTER UIUQ
+0x16A9B  𖪛 TANGSA LETTER UIUX
+0x16A9C  𖪜 TANGSA LETTER MZ
+0x16A9D  𖪝 TANGSA LETTER MC
+0x16A9E  𖪞 TANGSA LETTER MQ
+0x16A9F  𖪟 TANGSA LETTER MX
 0x16AA0  𖪠 TANGSA LETTER KA
 0x16AA1  𖪡 TANGSA LETTER KHA
 0x16AA2  𖪢 TANGSA LETTER GA
 0x16AA3  𖪣 TANGSA LETTER NGA
 0x16AA4  𖪤 TANGSA LETTER SA
 0x16AA5  𖪥 TANGSA LETTER YA
 0x16AA6  𖪦 TANGSA LETTER WA
 0x16AA7  𖪧 TANGSA LETTER PA
+0x16AA8  𖪨 TANGSA LETTER NYA
 0x16AA9  𖪩 TANGSA LETTER PHA
 0x16AAA  𖪪 TANGSA LETTER BA
 0x16AAB  𖪫 TANGSA LETTER MA
 0x16AAC  𖪬 TANGSA LETTER NA
 0x16AAD  𖪭 TANGSA LETTER HA
 0x16AAE  𖪮 TANGSA LETTER LA
+0x16AAF  𖪯 TANGSA LETTER HTA
 0x16AB0  𖪰 TANGSA LETTER TA
+0x16AB1  𖪱 TANGSA LETTER DA
 0x16AB2  𖪲 TANGSA LETTER RA
+0x16AB3  𖪳 TANGSA LETTER NHA
 0x16AB4  𖪴 TANGSA LETTER SHA
 0x16AB5  𖪵 TANGSA LETTER CA
+0x16AB6  𖪶 TANGSA LETTER TSA
 0x16AB7  𖪷 TANGSA LETTER GHA
 0x16AB8  𖪸 TANGSA LETTER HTTA
 0x16AB9  𖪹 TANGSA LETTER THA
-0x16A70  𖩰 TANGSA LETTER OZ
-0x16A71  𖩱 TANGSA LETTER OC
-0x16A72  𖩲 TANGSA LETTER OQ
-0x16A74  𖩴 TANGSA LETTER AZ
-0x16A75  𖩵 TANGSA LETTER AC
-0x16A76  𖩶 TANGSA LETTER AQ
-0x16A77  𖩷 TANGSA LETTER AX
-0x16A78  𖩸 TANGSA LETTER VZ
-0x16A79  𖩹 TANGSA LETTER VC
-0x16A7B  𖩻 TANGSA LETTER VX
-0x16A7C  𖩼 TANGSA LETTER EZ
-0x16A7D  𖩽 TANGSA LETTER EC
-0x16A7F  𖩿 TANGSA LETTER EX
+0x16ABA  𖪺 TANGSA LETTER XA
+0x16ABB  𖪻 TANGSA LETTER FA
+0x16ABC  𖪼 TANGSA LETTER DHA
+0x16ABD  𖪽 TANGSA LETTER CHA
+0x16ABE  𖪾 TANGSA LETTER ZA
+0x16AC0  𖫀 TANGSA DIGIT ZERO
+0x16AC1  𖫁 TANGSA DIGIT ONE
+0x16AC2  𖫂 TANGSA DIGIT TWO
+0x16AC3  𖫃 TANGSA DIGIT THREE
+0x16AC4  𖫄 TANGSA DIGIT FOUR
+0x16AC5  𖫅 TANGSA DIGIT FIVE
+0x16AC6  𖫆 TANGSA DIGIT SIX
+0x16AC7  𖫇 TANGSA DIGIT SEVEN
+0x16AC8  𖫈 TANGSA DIGIT EIGHT
+0x16AC9  𖫉 TANGSA DIGIT NINE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tangut_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tangut_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/telugu_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/telugu_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 0x0952 DEVANAGARI STRESS SIGN ANUDATTA
 0x0964 DEVANAGARI DANDA
 0x0965 DEVANAGARI DOUBLE DANDA
 0x0C00 TELUGU SIGN COMBINING CANDRABINDU ABOVE
 0x0C01 TELUGU SIGN CANDRABINDU
 0x0C02 TELUGU SIGN ANUSVARA
 0x0C03 TELUGU SIGN VISARGA
+0x0C04 TELUGU SIGN COMBINING ANUSVARA ABOVE
 0x0C05 TELUGU LETTER A
 0x0C06 TELUGU LETTER AA
 0x0C07 TELUGU LETTER I
 0x0C08 TELUGU LETTER II
 0x0C09 TELUGU LETTER U
 0x0C0A TELUGU LETTER UU
 0x0C0B TELUGU LETTER VOCALIC R
@@ -53,14 +54,15 @@
 0x0C33 TELUGU LETTER LLA
 0x0C34 TELUGU LETTER LLLA
 0x0C35 TELUGU LETTER VA
 0x0C36 TELUGU LETTER SHA
 0x0C37 TELUGU LETTER SSA
 0x0C38 TELUGU LETTER SA
 0x0C39 TELUGU LETTER HA
+0x0C3C TELUGU SIGN NUKTA
 0x0C3D TELUGU SIGN AVAGRAHA
 0x0C3E TELUGU VOWEL SIGN AA
 0x0C3F TELUGU VOWEL SIGN I
 0x0C40 TELUGU VOWEL SIGN II
 0x0C41 TELUGU VOWEL SIGN U
 0x0C42 TELUGU VOWEL SIGN UU
 0x0C43 TELUGU VOWEL SIGN VOCALIC R
@@ -73,28 +75,30 @@
 0x0C4C TELUGU VOWEL SIGN AU
 0x0C4D TELUGU SIGN VIRAMA
 0x0C55 TELUGU LENGTH MARK
 0x0C56 TELUGU AI LENGTH MARK
 0x0C58 TELUGU LETTER TSA
 0x0C59 TELUGU LETTER DZA
 0x0C5A TELUGU LETTER RRRA
+0x0C5D TELUGU LETTER NAKAARA POLLU
 0x0C60 TELUGU LETTER VOCALIC RR
 0x0C61 TELUGU LETTER VOCALIC LL
 0x0C62 TELUGU VOWEL SIGN VOCALIC L
 0x0C63 TELUGU VOWEL SIGN VOCALIC LL
 0x0C66 TELUGU DIGIT ZERO
 0x0C67 TELUGU DIGIT ONE
 0x0C68 TELUGU DIGIT TWO
 0x0C69 TELUGU DIGIT THREE
 0x0C6A TELUGU DIGIT FOUR
 0x0C6B TELUGU DIGIT FIVE
 0x0C6C TELUGU DIGIT SIX
 0x0C6D TELUGU DIGIT SEVEN
 0x0C6E TELUGU DIGIT EIGHT
 0x0C6F TELUGU DIGIT NINE
+0x0C77 TELUGU SIGN SIDDHAM
 0x0C78 TELUGU FRACTION DIGIT ZERO FOR ODD POWERS OF FOUR
 0x0C79 TELUGU FRACTION DIGIT ONE FOR ODD POWERS OF FOUR
 0x0C7A TELUGU FRACTION DIGIT TWO FOR ODD POWERS OF FOUR
 0x0C7B TELUGU FRACTION DIGIT THREE FOR ODD POWERS OF FOUR
 0x0C7C TELUGU FRACTION DIGIT ONE FOR EVEN POWERS OF FOUR
 0x0C7D TELUGU FRACTION DIGIT TWO FOR EVEN POWERS OF FOUR
 0x0C7E TELUGU FRACTION DIGIT THREE FOR EVEN POWERS OF FOUR
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/thaana_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/thaana_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/thai_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/thai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/toto_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/toto_unique-glyphs.nam`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 0x1E29B  𞊛 TOTO LETTER YA
 0x1E29C  𞊜 TOTO LETTER WA
 0x1E29D  𞊝 TOTO LETTER JA
 0x1E29E  𞊞 TOTO LETTER HA
 0x1E29F  𞊟 TOTO LETTER RA
 0x1E2A0  𞊠 TOTO LETTER LA
 0x1E2A1  𞊡 TOTO LETTER I
+0x1E2A2  𞊢 TOTO LETTER BREATHY I
 0x1E2A3  𞊣 TOTO LETTER IU
+0x1E2A4  𞊤 TOTO LETTER BREATHY IU
 0x1E2A5  𞊥 TOTO LETTER U
 0x1E2A6  𞊦 TOTO LETTER E
 0x1E2A7  𞊧 TOTO LETTER BREATHY E
 0x1E2A8  𞊨 TOTO LETTER EO
+0x1E2A9  𞊩 TOTO LETTER BREATHY EO
 0x1E2AA  𞊪 TOTO LETTER O
 0x1E2AB  𞊫 TOTO LETTER AE
+0x1E2AC  𞊬 TOTO LETTER BREATHY AE
 0x1E2AD  𞊭 TOTO LETTER A
 0x1E2AE  𞊮 TOTO SIGN RISING TONE
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/vai_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/vai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/wancho_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/wancho_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/wgl-latin.enc` & `glyphsets-0.6.1/Lib/glyphsets/encodings/wgl-latin.enc`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/yi_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/yi_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,59 @@
 0x0000 NULL
 0x000D CARRIAGE RETURN (CR)
 0x0020 SPACE
 0x00A0 NO-BREAK SPACE
+0x02C7 CARON
+0x02D8 BREVE
+0x02D9 DOT ABOVE
+0x02DB OGONEK
+0x03C0 GREEK SMALL LETTER PI
+0x200C ZERO WIDTH NON-JOINER
+0x200D ZERO WIDTH JOINER
+0x2010 HYPHEN
+0x2011 NON-BREAKING HYPHEN
+0x202F NARROW NO-BREAK SPACE
+0x2219 BULLET OPERATOR
+0x2460 CIRCLED DIGIT ONE
+0x2461 CIRCLED DIGIT TWO
+0x2462 CIRCLED DIGIT THREE
+0x2463 CIRCLED DIGIT FOUR
+0x2464 CIRCLED DIGIT FIVE
+0x2465 CIRCLED DIGIT SIX
+0x2466 CIRCLED DIGIT SEVEN
+0x2467 CIRCLED DIGIT EIGHT
+0x2468 CIRCLED DIGIT NINE
+0x2469 CIRCLED NUMBER TEN
+0x246A CIRCLED NUMBER ELEVEN
+0x246B CIRCLED NUMBER TWELVE
+0x246C CIRCLED NUMBER THIRTEEN
+0x246D CIRCLED NUMBER FOURTEEN
+0x246E CIRCLED NUMBER FIFTEEN
+0x246F CIRCLED NUMBER SIXTEEN
+0x2470 CIRCLED NUMBER SEVENTEEN
+0x2471 CIRCLED NUMBER EIGHTEEN
+0x2472 CIRCLED NUMBER NINETEEN
+0x2473 CIRCLED NUMBER TWENTY
+0x25CC DOTTED CIRCLE
+0x3000 IDEOGRAPHIC SPACE
 0x3001 IDEOGRAPHIC COMMA
 0x3002 IDEOGRAPHIC FULL STOP
+0x3003 DITTO MARK
 0x3008 LEFT ANGLE BRACKET
 0x3009 RIGHT ANGLE BRACKET
 0x300A LEFT DOUBLE ANGLE BRACKET
 0x300B RIGHT DOUBLE ANGLE BRACKET
 0x300C LEFT CORNER BRACKET
 0x300D RIGHT CORNER BRACKET
 0x300E LEFT WHITE CORNER BRACKET
 0x300F RIGHT WHITE CORNER BRACKET
 0x3010 LEFT BLACK LENTICULAR BRACKET
 0x3011 RIGHT BLACK LENTICULAR BRACKET
+0x3012 POSTAL MARK
+0x3013 GETA MARK
 0x3014 LEFT TORTOISE SHELL BRACKET
 0x3015 RIGHT TORTOISE SHELL BRACKET
 0x3016 LEFT WHITE LENTICULAR BRACKET
 0x3017 RIGHT WHITE LENTICULAR BRACKET
 0x3018 LEFT WHITE TORTOISE SHELL BRACKET
 0x3019 RIGHT WHITE TORTOISE SHELL BRACKET
 0x301A LEFT WHITE SQUARE BRACKET
@@ -1239,17 +1275,29 @@
 0xA4C0 YI RADICAL SHAT
 0xA4C1 YI RADICAL ZUR
 0xA4C2 YI RADICAL SHOP
 0xA4C3 YI RADICAL CHE
 0xA4C4 YI RADICAL ZZIET
 0xA4C5 YI RADICAL NBIE
 0xA4C6 YI RADICAL KE
+0xFE00 VARIATION SELECTOR-1
 0xFF01 FULLWIDTH EXCLAMATION MARK
+0xFF02 FULLWIDTH QUOTATION MARK
+0xFF08 FULLWIDTH LEFT PARENTHESIS
+0xFF09 FULLWIDTH RIGHT PARENTHESIS
 0xFF0C FULLWIDTH COMMA
+0xFF0E FULLWIDTH FULL STOP
+0xFF0F FULLWIDTH SOLIDUS
 0xFF1A FULLWIDTH COLON
 0xFF1B FULLWIDTH SEMICOLON
 0xFF1F FULLWIDTH QUESTION MARK
+0xFF3B FULLWIDTH LEFT SQUARE BRACKET
+0xFF3D FULLWIDTH RIGHT SQUARE BRACKET
+0xFF5B FULLWIDTH LEFT CURLY BRACKET
+0xFF5C FULLWIDTH VERTICAL LINE
+0xFF5D FULLWIDTH RIGHT CURLY BRACKET
+0xFF5E FULLWIDTH TILDE
 0xFF61 HALFWIDTH IDEOGRAPHIC FULL STOP
 0xFF62 HALFWIDTH LEFT CORNER BRACKET
 0xFF63 HALFWIDTH RIGHT CORNER BRACKET
 0xFF64 HALFWIDTH IDEOGRAPHIC COMMA
 0xFF65 HALFWIDTH KATAKANA MIDDLE DOT
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam` & `glyphsets-0.6.1/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/subsets.py` & `glyphsets-0.6.1/Lib/glyphsets/subsets.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets/test_strings.json` & `glyphsets-0.6.1/Lib/glyphsets/test_strings.json`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/Lib/glyphsets.egg-info/PKG-INFO` & `glyphsets-0.6.1/Lib/glyphsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.0/Lib/glyphsets.egg-info/SOURCES.txt` & `glyphsets-0.6.1/Lib/glyphsets.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -260,32 +260,36 @@
 Lib/glyphsets/encodings/balinese_unique-glyphs.nam
 Lib/glyphsets/encodings/bamum_unique-glyphs.nam
 Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
 Lib/glyphsets/encodings/batak_unique-glyphs.nam
 Lib/glyphsets/encodings/bengali_unique-glyphs.nam
 Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
 Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
+Lib/glyphsets/encodings/braille_unique-glyphs.nam
 Lib/glyphsets/encodings/buginese_unique-glyphs.nam
 Lib/glyphsets/encodings/buhid_unique-glyphs.nam
 Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
 Lib/glyphsets/encodings/carian_unique-glyphs.nam
 Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
 Lib/glyphsets/encodings/chakma_unique-glyphs.nam
 Lib/glyphsets/encodings/cham_unique-glyphs.nam
 Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
 Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
 Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
 Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
+Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
 Lib/glyphsets/encodings/coptic_unique-glyphs.nam
 Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
 Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
+Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
 Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
 Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
 Lib/glyphsets/encodings/deseret_unique-glyphs.nam
 Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
+Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
 Lib/glyphsets/encodings/dogra_unique-glyphs.nam
 Lib/glyphsets/encodings/duployan_unique-glyphs.nam
 Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
 Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
 Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
 Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
 Lib/glyphsets/encodings/georgian_unique-glyphs.nam
@@ -305,16 +309,18 @@
 Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
 Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
 Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
 Lib/glyphsets/encodings/japanese_unique-glyphs.nam
 Lib/glyphsets/encodings/javanese_unique-glyphs.nam
 Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
 Lib/glyphsets/encodings/kannada_unique-glyphs.nam
+Lib/glyphsets/encodings/kawi_unique-glyphs.nam
 Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
 Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
+Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
 Lib/glyphsets/encodings/khmer_unique-glyphs.nam
 Lib/glyphsets/encodings/khojki_unique-glyphs.nam
 Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
 Lib/glyphsets/encodings/korean_unique-glyphs.nam
 Lib/glyphsets/encodings/lao_unique-glyphs.nam
 Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
 Lib/glyphsets/encodings/latin_unique-glyphs.nam
@@ -322,34 +328,39 @@
 Lib/glyphsets/encodings/limbu_unique-glyphs.nam
 Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
 Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
 Lib/glyphsets/encodings/lisu_unique-glyphs.nam
 Lib/glyphsets/encodings/lycian_unique-glyphs.nam
 Lib/glyphsets/encodings/lydian_unique-glyphs.nam
 Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
+Lib/glyphsets/encodings/makasar_unique-glyphs.nam
 Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
 Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
 Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
 Lib/glyphsets/encodings/marchen_unique-glyphs.nam
 Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
 Lib/glyphsets/encodings/math.nam
 Lib/glyphsets/encodings/math_unique-glyphs.nam
 Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
 Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
 Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
 Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
+Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
+Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
 Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
 Lib/glyphsets/encodings/miao_unique-glyphs.nam
 Lib/glyphsets/encodings/modi_unique-glyphs.nam
 Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
 Lib/glyphsets/encodings/mro_unique-glyphs.nam
 Lib/glyphsets/encodings/multani_unique-glyphs.nam
 Lib/glyphsets/encodings/music_unique-glyphs.nam
 Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
 Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
+Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
+Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
 Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
 Lib/glyphsets/encodings/newa_unique-glyphs.nam
 Lib/glyphsets/encodings/nko_unique-glyphs.nam
 Lib/glyphsets/encodings/nushu_unique-glyphs.nam
 Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
 Lib/glyphsets/encodings/ogham_unique-glyphs.nam
 Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
@@ -357,17 +368,19 @@
 Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
 Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
 Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
 Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
 Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
 Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
 Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
+Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
 Lib/glyphsets/encodings/oriya_unique-glyphs.nam
 Lib/glyphsets/encodings/osage_unique-glyphs.nam
 Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
+Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
 Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
 Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
 Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
 Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
 Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
 Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
 Lib/glyphsets/encodings/rejang_unique-glyphs.nam
@@ -402,14 +415,15 @@
 Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
 Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
 Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
 Lib/glyphsets/encodings/toto_unique-glyphs.nam
 Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
 Lib/glyphsets/encodings/vai_unique-glyphs.nam
 Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
+Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
 Lib/glyphsets/encodings/wancho_unique-glyphs.nam
 Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
 Lib/glyphsets/encodings/wgl-latin.enc
 Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
 Lib/glyphsets/encodings/yi_unique-glyphs.nam
 Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
 scripts/create-glyphset.py
```

### Comparing `glyphsets-0.6.0/PKG-INFO` & `glyphsets-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.0/README.md` & `glyphsets-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/scripts/create-glyphset.py` & `glyphsets-0.6.1/scripts/create-glyphset.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/setup.py` & `glyphsets-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/tests/__init__.py` & `glyphsets-0.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/tests/data/MavenPro[wght].ttf` & `glyphsets-0.6.1/tests/data/MavenPro[wght].ttf`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/tests/test_glyphdata.py` & `glyphsets-0.6.1/tests/test_glyphdata.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.0/tests/testcoverage.py` & `glyphsets-0.6.1/tests/testcoverage.py`

 * *Files identical despite different names*

