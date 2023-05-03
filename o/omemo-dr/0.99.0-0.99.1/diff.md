# Comparing `tmp/omemo-dr-0.99.0.tar.gz` & `tmp/omemo-dr-0.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omemo-dr-0.99.0.tar", last modified: Sun Mar 26 21:18:56 2023, max compression
+gzip compressed data, was "omemo-dr-0.99.1.tar", last modified: Wed May  3 19:56:31 2023, max compression
```

## Comparing `omemo-dr-0.99.0.tar` & `omemo-dr-0.99.1.tar`

### file list

```diff
@@ -1,209 +1,210 @@
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    35122 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/LICENSE
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       62 2023-03-26 20:15:40.000000 omemo-dr-0.99.0/MANIFEST.in
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    43500 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/PKG-INFO
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2432 2023-03-26 13:27:30.000000 omemo-dr-0.99.0/README.md
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.486659 omemo-dr-0.99.0/curve25519/
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.486659 omemo-dr-0.99.0/curve25519/curve/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    31932 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/curve25519-donna.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      137 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/curve25519-donna.h
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.494659 omemo-dr-0.99.0/curve25519/curve/ed25519/
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.498659 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      663 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/compare.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      129 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/compare.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      536 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/convert.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1624 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/crypto_additions.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      156 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3046 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/curve_sigs.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      662 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/curve_sigs.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1139 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ed_sigs.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      321 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ed_sigs.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2236 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/elligator.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      333 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      205 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_isequal.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      242 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_isreduced.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      425 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_mont_rhs.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      319 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1355 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_sqrt.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      279 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_isneutral.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1966 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      201 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_neg.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      440 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3141 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_scalarmult.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      314 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.498659 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      384 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_constants.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      284 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2660 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1034 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      948 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1821 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_x.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      621 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/keygen.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      389 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/keygen.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      951 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/open_modified.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      113 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sc_clamp.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      465 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sc_cmov.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      996 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sc_neg.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1326 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sign_modified.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      594 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/utility.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      252 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/utility.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2367 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/xeddsa.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      636 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/xeddsa.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      280 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/zeroize.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      174 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/additions/zeroize.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      121 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/api.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    76457 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/base.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2388 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/base2.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       91 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/d.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       90 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/d2.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1939 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      170 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_0.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      170 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_1.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1255 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_add.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1283 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_cmov.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      454 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_copy.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2222 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_frombytes.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      135 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_invert.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      266 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_isnegative.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      453 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_isnonzero.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    10744 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_mul.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      855 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_neg.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      127 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_pow22523.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5980 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sq.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     6106 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sq2.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1255 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sub.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3189 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/fe_tobytes.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2869 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      125 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_add.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2080 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_add.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2371 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_double_scalarmult.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      987 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_frombytes.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      128 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_madd.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1900 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_madd.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      128 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_msub.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1900 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_msub.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      165 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p1p1_to_p2.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      191 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p1p1_to_p3.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       86 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p2_0.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      112 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p2_dbl.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1476 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p2_dbl.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      100 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p3_0.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      131 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p3_dbl.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      246 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p3_to_cached.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      149 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p3_to_p2.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      228 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p3_tobytes.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      110 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_precomp_0.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2477 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_scalarmult_base.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      125 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_sub.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2080 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_sub.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      225 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/ge_tobytes.c
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.498659 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       81 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       87 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      751 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2034 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       93 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       99 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      579 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.498659 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_sha512/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     6416 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_sha512/blocks.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1807 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_sha512/hash.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1036 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/open.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5518 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/pow22523.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5527 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/pow225521.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      382 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/sc.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    12494 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/sc_muladd.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     8139 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/sc_reduce.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      817 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/sign.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       87 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/sqrtm1.h
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.498659 omemo-dr-0.99.0/curve25519/curve/ed25519/tests/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      563 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/tests/internal_fast_tests.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      540 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve/ed25519/tests/internal_slow_tests.h
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     8043 2023-03-26 11:36:38.000000 omemo-dr-0.99.0/curve25519/curve25519module.c
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     4981 2023-03-26 21:14:42.000000 omemo-dr-0.99.0/pyproject.toml
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       38 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/setup.cfg
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      685 2023-03-26 20:15:01.000000 omemo-dr-0.99.0/setup.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.486659 omemo-dr-0.99.0/src/
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.502659 omemo-dr-0.99.0/src/omemo_dr/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       22 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/__init__.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.502659 omemo-dr-0.99.0/src/omemo_dr/curve/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1045 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/curve/__init__.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.502659 omemo-dr-0.99.0/src/omemo_dr/ecc/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/ecc/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2552 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ecc/curve.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2215 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ecc/djbec.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      350 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ecc/ec.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      429 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ecc/eckeypair.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      889 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/exceptions.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1029 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/identitykey.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1471 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/identitykeypair.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.502659 omemo-dr-0.99.0/src/omemo_dr/kdf/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 13:20:33.000000 omemo-dr-0.99.0/src/omemo_dr/kdf/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      605 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/kdf/derivedmessagesecrets.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      360 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/kdf/derivedrootsecrets.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1897 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/kdf/hkdf.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      485 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/kdf/messagekeys.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.506659 omemo-dr-0.99.0/src/omemo_dr/protocol/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 13:20:37.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      497 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/ciphertextmessage.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2884 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/omemo_keyexchange.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     4940 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/omemo_message.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     8074 2023-03-26 15:46:44.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/omemo_pb2.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5013 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/prekeywhispermessage.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     4878 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/whispermessage.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    15498 2023-03-26 15:46:44.000000 omemo-dr-0.99.0/src/omemo_dr/protocol/whisperprotos_pb2.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/py.typed
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.506659 omemo-dr-0.99.0/src/omemo_dr/ratchet/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3216 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/aliceaxolotlparameters.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3033 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/bobaxolotlparamaters.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1622 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/chainkey.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5196 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/ratchetingsession.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1340 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/ratchet/rootkey.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     6307 2023-03-26 17:59:20.000000 omemo-dr-0.99.0/src/omemo_dr/sessionbuilder.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    11030 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/sessioncipher.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.506659 omemo-dr-0.99.0/src/omemo_dr/state/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/state/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      302 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/axolotlstore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      613 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/identitykeystore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1844 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/prekeybundle.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1464 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/prekeyrecord.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      538 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/state/prekeystore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2863 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/sessionrecord.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    14986 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/sessionstate.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      837 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/sessionstore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1812 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/signedprekeyrecord.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      736 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/state/signedprekeystore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    43661 2023-03-26 15:46:44.000000 omemo-dr-0.99.0/src/omemo_dr/state/storageprotos_pb2.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/src/omemo_dr/util/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/src/omemo_dr/util/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1305 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/util/byteutil.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3159 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/util/keyhelper.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       39 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/src/omemo_dr/util/medium.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.502659 omemo-dr-0.99.0/src/omemo_dr.egg-info/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    43500 2023-03-26 21:18:56.000000 omemo-dr-0.99.0/src/omemo_dr.egg-info/PKG-INFO
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     7031 2023-03-26 21:18:56.000000 omemo-dr-0.99.0/src/omemo_dr.egg-info/SOURCES.txt
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        1 2023-03-26 21:18:56.000000 omemo-dr-0.99.0/src/omemo_dr.egg-info/dependency_links.txt
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)       87 2023-03-26 21:18:56.000000 omemo-dr-0.99.0/src/omemo_dr.egg-info/requires.txt
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        9 2023-03-26 21:18:56.000000 omemo-dr-0.99.0/src/omemo_dr.egg-info/top_level.txt
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/tests/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/tests/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     2777 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/inmemoryaxolotlstore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1093 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/inmemoryidentitykeystore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      844 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/inmemoryprekeystore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1354 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/inmemorysessionstore.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     1095 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/inmemorysignedprekeystore.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/tests/kdf/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/tests/kdf/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    12304 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/kdf/test_hkdf.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/tests/ratchet/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 11:36:23.000000 omemo-dr-0.99.0/tests/ratchet/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     3866 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/ratchet/test_chainkey.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     7814 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/ratchet/test_ratchetingsession.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     5761 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/ratchet/test_rootkey.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)    13546 2023-03-26 20:33:50.000000 omemo-dr-0.99.0/tests/test_sessionbuilder.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     7716 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/test_sessioncipher.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)     9272 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/test_sigs.py
-drwxrwxr-x   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 21:18:56.510659 omemo-dr-0.99.0/tests/util/
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)        0 2023-03-26 13:20:21.000000 omemo-dr-0.99.0/tests/util/__init__.py
--rw-rw-r--   0 lovetox   (1000) lovetox   (1000)      810 2023-03-26 17:38:42.000000 omemo-dr-0.99.0/tests/util/test_byteutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    43228 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.171828 omemo-dr-0.99.1/curve25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.171828 omemo-dr-0.99.1/curve25519/curve/
+-rw-rw-rw-   0 root         (0) root         (0)    31932 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/curve25519-donna.c
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/curve25519-donna.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.179829 omemo-dr-0.99.1/curve25519/curve/ed25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.183829 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/compare.c
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/compare.h
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/convert.c
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/curve_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/curve_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ed_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ed_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     2236 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/elligator.c
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_isequal.c
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_isreduced.c
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_mont_rhs.c
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_sqrt.c
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_isneutral.c
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.187829 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_x.h
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/keygen.c
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/keygen.h
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/open_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sc_clamp.c
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sc_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sc_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sign_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/utility.c
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/utility.h
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/xeddsa.c
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/xeddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/zeroize.c
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/additions/zeroize.h
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/api.h
+-rw-rw-rw-   0 root         (0) root         (0)    76457 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/base.h
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/base2.h
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/d.h
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/d2.h
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe.h
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_1.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_copy.c
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_invert.c
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_isnegative.c
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_isnonzero.c
+-rw-rw-rw-   0 root         (0) root         (0)    10744 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_mul.c
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_pow22523.c
+-rw-rw-rw-   0 root         (0) root         (0)     5980 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sq.c
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sq2.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/fe_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge.h
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_add.h
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_double_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_madd.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_madd.h
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_msub.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_msub.h
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p1p1_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p1p1_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p2_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p2_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p2_dbl.h
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p3_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p3_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p3_to_cached.c
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p3_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p3_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_precomp_0.c
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_scalarmult_base.c
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_sub.h
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/ge_tobytes.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.187829 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.187829 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_sha512/
+-rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_sha512/blocks.c
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_sha512/hash.c
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/open.c
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/pow22523.h
+-rw-rw-rw-   0 root         (0) root         (0)     5527 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/pow225521.h
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/sc.h
+-rw-rw-rw-   0 root         (0) root         (0)    12494 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/sc_muladd.c
+-rw-rw-rw-   0 root         (0) root         (0)     8139 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/sc_reduce.c
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/sign.c
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/sqrtm1.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.187829 omemo-dr-0.99.1/curve25519/curve/ed25519/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/tests/internal_fast_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/curve25519/curve/ed25519/tests/internal_slow_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)     8040 2023-04-09 19:22:07.000000 omemo-dr-0.99.1/curve25519/curve25519module.c
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-26 20:37:13.000000 omemo-dr-0.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.167827 omemo-dr-0.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.187829 omemo-dr-0.99.1/src/omemo_dr/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.191830 omemo-dr-0.99.1/src/omemo_dr/curve/
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/curve/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.191830 omemo-dr-0.99.1/src/omemo_dr/ecc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/ecc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2613 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ecc/curve.py
+-rw-rw-rw-   0 root         (0) root         (0)     2259 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ecc/djbec.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ecc/ec.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ecc/eckeypair.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/identitykey.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/identitykeypair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.191830 omemo-dr-0.99.1/src/omemo_dr/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/kdf/derivedmessagesecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/kdf/derivedrootsecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/kdf/hkdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/kdf/messagekeys.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/observable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.191830 omemo-dr-0.99.1/src/omemo_dr/protocol/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/ciphertextmessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4099 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/omemo_keyexchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     5043 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/omemo_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     8074 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/omemo_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5085 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/prekeywhispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4939 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/whispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)    15498 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/protocol/whisperprotos_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.195830 omemo-dr-0.99.1/src/omemo_dr/ratchet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/aliceparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/bobparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/chainkey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5537 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/ratchetingsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/ratchet/rootkey.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5575 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    11003 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/sessioncipher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.195830 omemo-dr-0.99.1/src/omemo_dr/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/state/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/prekeybundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/prekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)     2925 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/sessionrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)    15547 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/sessionstate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/signedprekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)    43661 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/state/storageprotos_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4452 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/state/store.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.195830 omemo-dr-0.99.1/src/omemo_dr/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/util/byteutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/src/omemo_dr/util/keyhelper.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/src/omemo_dr/util/medium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.191830 omemo-dr-0.99.1/src/omemo_dr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43228 2023-05-03 19:56:31.000000 omemo-dr-0.99.1/src/omemo_dr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6972 2023-05-03 19:56:31.000000 omemo-dr-0.99.1/src/omemo_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:56:31.000000 omemo-dr-0.99.1/src/omemo_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-03 19:56:31.000000 omemo-dr-0.99.1/src/omemo_dr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-03 19:56:31.000000 omemo-dr-0.99.1/src/omemo_dr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/inmemoryidentitykeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/inmemoryprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/inmemorysessionstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/inmemorysignedprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/inmemorystore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/tests/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/tests/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12318 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/kdf/test_hkdf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/tests/ratchet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/tests/ratchet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/ratchet/test_chainkey.py
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/ratchet/test_ratchetingsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/ratchet/test_rootkey.py
+-rw-rw-rw-   0 root         (0) root         (0)    10477 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/test_sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/test_sessioncipher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9370 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/test_sigs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:56:31.199830 omemo-dr-0.99.1/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.1/tests/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-03 19:53:25.000000 omemo-dr-0.99.1/tests/util/test_byteutil.py
```

### Comparing `omemo-dr-0.99.0/LICENSE` & `omemo-dr-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/PKG-INFO` & `omemo-dr-0.99.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.0
+Version: 0.99.1
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -712,50 +712,45 @@
 
 ## Install time
 
 At install time, a libaxolotl client needs to generate its identity keys, registration id, and
 prekeys.
 
 ```python
-    identityKeyPair = KeyHelper.generateIdentityKeyPair()
-    registrationId  = KeyHelper.generateRegistrationId()
-    preKeys         = KeyHelper.generatePreKeys(startId, 100)
-    lastResortKey   = KeyHelper.generateLastResortKey()
-    signedPreKey    = KeyHelper.generateSignedPreKey(identityKeyPair, 5)
+    identity_key_pair = KeyHelper.generate_identity_key_pair()
+    registration_id   = KeyHelper.generate_registration_id()
+    pre_keys          = KeyHelper.generate_pre_keys(start_id, 100)
+    last_resort_key   = KeyHelper.generate_last_resort_key()
+    signed_pre_key    = KeyHelper.generate_signed_pre_key(identity_key_pair, 5)
 
-    #Store identityKeyPair somewhere durable and safe.
-    #Store registrationId somewhere durable and safe.
+    #Store identity_key_pair somewhere durable and safe.
+    #Store registration_id somewhere durable and safe.
 
-    #Store preKeys in PreKeyStore.
+    #Store pre_keys in PreKeyStore.
     #Store signed prekey in SignedPreKeyStore.
 ```
 
 ## Building a session
 
-A libaxolotl client needs to implement four interfaces: IdentityKeyStore, PreKeyStore, 
-SignedPreKeyStore, and SessionStore.  These will manage loading and storing of identity, 
+A libaxolotl client needs to implement the Store interface. This will manage loading and storing of identity, 
 prekeys, signed prekeys, and session state.
 
-Once those are implemented, building a session is fairly straightforward:
+Once this is implemented, building a session is fairly straightforward:
 
 ```python
-sessionStore      = MySessionStore()
-preKeyStore       = MyPreKeyStore()
-signedPreKeyStore = MySignedPreKeyStore()
-identityStore     = MyIdentityKeyStore()
-
-# Instantiate a SessionBuilder for a remote recipientId + deviceId tuple.
-sessionBuilder = SessionBuilder(sessionStore, preKeyStore, signedPreKeyStore,
-                                                   identityStore, recipientId, deviceId)
+store      = MyStore()
+
+# Instantiate a SessionBuilder for a remote recipient_id + device_id tuple.
+session_builder = SessionBuilder(store, recipient_id, device_id)
 
 # Build a session with a PreKey retrieved from the server.
-sessionBuilder.process(retrievedPreKey)
+sessionBuilder.process(retrieved_pre_key)
 
-sessionCipher = SessionCipher(sessionStore, recipientId, deviceId)
-message       = sessionCipher.encrypt("Hello world!")
+session_cipher = SessionCipher(store, recipient_id, device_id)
+message        = session_cipher.encrypt("Hello world!")
 
 deliver(message.serialize())
 ```
 
 # Development
 
 ## Generating protobuf files
```

### Comparing `omemo-dr-0.99.0/curve25519/curve/curve25519-donna.c` & `omemo-dr-0.99.1/curve25519/curve/curve25519-donna.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/compare.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/compare.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/convert.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/convert.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/crypto_additions.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/crypto_additions.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/curve_sigs.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/curve_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/curve_sigs.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/curve_sigs.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ed_sigs.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ed_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/elligator.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/elligator.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/fe_sqrt.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/fe_sqrt.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_montx_to_p3.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_montx_to_p3.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/ge_scalarmult.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/ge_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_labelset.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_labelset.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/generalized/gen_x.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/generalized/gen_x.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/keygen.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/keygen.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/open_modified.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/open_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sc_neg.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sc_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/sign_modified.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/sign_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/utility.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/utility.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/xeddsa.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/xeddsa.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/additions/xeddsa.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/additions/xeddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/base.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/base.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/base2.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/base2.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_add.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_add.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_cmov.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_cmov.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_frombytes.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_mul.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_mul.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_neg.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sq.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sq.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sq2.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sq2.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_sub.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_sub.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/fe_tobytes.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/fe_tobytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_add.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_add.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_double_scalarmult.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_double_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_frombytes.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_madd.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_madd.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_msub.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_msub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_p2_dbl.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_p2_dbl.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_scalarmult_base.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_scalarmult_base.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/ge_sub.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/ge_sub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_sign.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_sign.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_sha512/blocks.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_sha512/blocks.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/nacl_sha512/hash.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/nacl_sha512/hash.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/open.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/open.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/pow22523.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/pow22523.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/pow225521.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/pow225521.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/sc_muladd.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/sc_muladd.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/sc_reduce.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/sc_reduce.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/sign.c` & `omemo-dr-0.99.1/curve25519/curve/ed25519/sign.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/tests/internal_fast_tests.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/tests/internal_fast_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve/ed25519/tests/internal_slow_tests.h` & `omemo-dr-0.99.1/curve25519/curve/ed25519/tests/internal_slow_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/curve25519/curve25519module.c` & `omemo-dr-0.99.1/curve25519/curve25519module.c`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
 
 static struct PyModuleDef
 curve25519_module = {
     PyModuleDef_HEAD_INIT,
     "_curve",
     NULL,
-    NULL,
+    0,
     curve25519_functions,
 };
 
 PyObject *
 PyInit__curve(void)
 {
     return PyModule_Create(&curve25519_module);
```

### Comparing `omemo-dr-0.99.0/pyproject.toml` & `omemo-dr-0.99.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools>=65.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omemo-dr"
-version = "0.99.0"
 requires-python = ">=3.10"
 description = "OMEMO Double Ratchet"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   {email = "philipp@hoerist.com"},
   {name = "Philipp Hörist"}
@@ -20,22 +19,26 @@
   "Topic :: Security :: Cryptography",
   "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 dependencies = [
   "cryptography",
   "protobuf>=3.0.0",
 ]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "ruff>=0.0.254",
   "codespell[toml]>=2.2.4",
   "black>=23.1.0"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "omemo_dr.__version__"}
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 "omemo_dr" = ["py.typed"]
 
 [tool.codespell]
@@ -52,24 +55,17 @@
 reportMissingModuleSource = "none"
 
 exclude = [
   "**/__pycache__",
   ".git",
   "build",
   "node_modules",
-  "src/omemo_dr/protocol/omemo_keyexchange.py",
   "src/omemo_dr/protocol/omemo_pb2.py",
   "src/omemo_dr/protocol/whisperprotos_pb2.py",
-  "src/omemo_dr/ratchet/aliceaxolotlparameters.py",
-  "src/omemo_dr/ratchet/bobaxolotlparamaters.py",
-  "src/omemo_dr/ratchet/ratchetingsession.py",
-  "src/omemo_dr/sessionbuilder.py",
   "src/omemo_dr/state/storageprotos_pb2.py",
-  "src/omemo_dr/curve/__init__.py",
-  "tests/*",
 ]
 
 [tool.ruff]
 line-length = 88
 
 select = [
   "A",      # flake8-builtins
@@ -174,8 +170,8 @@
 ]
 skip_gitignore = true
 skip_glob = ["**/*pb2.py"]
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
-extend-exclude = ".*pb2.py"
+force-exclude = ".*pb2.py"
```

### Comparing `omemo-dr-0.99.0/setup.py` & `omemo-dr-0.99.1/setup.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/src/omemo_dr/ecc/curve.py` & `omemo-dr-0.99.1/src/omemo_dr/ecc/curve.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 ED25519_KEY_LEN = 32
 
 
 class Curve:
     DJB_TYPE = 5
 
     @staticmethod
-    def _generatePrivateKey() -> bytes:
+    def _generate_private_key() -> bytes:
         rand = os.urandom(32)
         return curve.generate_private_key(rand)
 
     @staticmethod
-    def _generatePublicKey(privateKey: bytes) -> bytes:
-        return curve.generate_public_key(privateKey)
+    def _generate_public_key(private_key: bytes) -> bytes:
+        return curve.generate_public_key(private_key)
 
     @staticmethod
-    def generateKeyPair() -> ECKeyPair:
-        privateKey = Curve._generatePrivateKey()
-        publicKey = Curve._generatePublicKey(privateKey)
-        return ECKeyPair(CurvePublicKey(publicKey), DjbECPrivateKey(privateKey))
+    def generate_key_pair() -> ECKeyPair:
+        private_key = Curve._generate_private_key()
+        public_key = Curve._generate_public_key(private_key)
+        return ECKeyPair(CurvePublicKey(public_key), DjbECPrivateKey(private_key))
 
     @staticmethod
-    def decodePoint(
+    def decode_point(
         _bytes: bytearray, offset: int = 0
     ) -> Union[CurvePublicKey, EdPublicKey]:
         key_type = _bytes[0]
         key_len = len(_bytes)
 
         if key_len == CURVE25519_KEY_LEN and key_type == Curve.DJB_TYPE:
             return CurvePublicKey(bytes(_bytes[1:]))
@@ -48,40 +48,42 @@
 
         else:
             raise InvalidKeyException(
                 "Unknown key type or length: %s - %s" % (key_type, key_len)
             )
 
     @staticmethod
-    def decodePrivatePoint(_bytes: bytes) -> DjbECPrivateKey:
+    def decode_private_point(_bytes: bytes) -> DjbECPrivateKey:
         return DjbECPrivateKey(bytes(_bytes))
 
     @staticmethod
-    def calculateAgreement(
-        publicKey: CurvePublicKey, privateKey: DjbECPrivateKey
+    def calculate_agreement(
+        public_key: CurvePublicKey, private_key: DjbECPrivateKey
     ) -> bytes:
         return curve.calculate_agreement(
-            privateKey.getPrivateKey(), publicKey.get_bytes()
+            private_key.get_private_key(), public_key.get_bytes()
         )
 
     @staticmethod
-    def verifySignature(
-        ecPublicSigningKey: Union[CurvePublicKey, EdPublicKey],
+    def verify_signature(
+        ec_public_signing_key: Union[CurvePublicKey, EdPublicKey],
         message: bytes,
         signature: bytes,
     ) -> bool:
-        if isinstance(ecPublicSigningKey, CurvePublicKey):
+        if isinstance(ec_public_signing_key, CurvePublicKey):
             result = curve.verify_signature_curve(
-                ecPublicSigningKey.get_bytes(), message, signature
+                ec_public_signing_key.get_bytes(), message, signature
             )
         else:
             result = curve.verify_signature_ed(
-                ecPublicSigningKey.get_bytes(), message, signature
+                ec_public_signing_key.get_bytes(), message, signature
             )
         return result == 0
 
     @staticmethod
-    def calculateSignature(privateSigningKey: DjbECPrivateKey, message: bytes) -> bytes:
+    def calculate_signature(
+        private_signing_key: DjbECPrivateKey, message: bytes
+    ) -> bytes:
         rand = os.urandom(64)
         return curve.calculate_signature(
-            rand, privateSigningKey.getPrivateKey(), message
+            rand, private_signing_key.get_private_key(), message
         )
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/ecc/djbec.py` & `omemo-dr-0.99.1/src/omemo_dr/ecc/djbec.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,77 +12,77 @@
 CURVE25519_KEY_LEN = 33
 ED25519_KEY_LEN = 32
 DJB_TYPE = 5
 
 
 class DjbECPublicKey(ECPublicKey):
     def __init__(self, _bytes: bytes) -> None:
-        self._publicKey = _bytes
+        self._public_key = _bytes
 
-    def getType(self) -> int:
+    def get_type(self) -> int:
         from .curve import Curve
 
         return Curve.DJB_TYPE
 
     def get_bytes(self) -> bytes:
-        return self._publicKey
+        return self._public_key
 
-    def getPublicKey(self) -> bytes:
-        return self._publicKey
+    def get_public_key(self) -> bytes:
+        return self._public_key
 
     def __eq__(self, other: Any) -> bool:
-        return self._publicKey == other.getPublicKey()
+        return self._public_key == other.get_public_key()
 
     def __lt__(self, other: Any) -> bool:
-        myVal = int(binascii.hexlify(self._publicKey), 16)
-        otherVal = int(binascii.hexlify(other.getPublicKey()), 16)
+        my_val = int(binascii.hexlify(self._public_key), 16)
+        other_val = int(binascii.hexlify(other.get_public_key()), 16)
 
-        return myVal < otherVal
+        return my_val < other_val
 
     def __cmp__(self, other: Any) -> int:
-        myVal = int(binascii.hexlify(self._publicKey), 16)
-        otherVal = int(binascii.hexlify(other.getPublicKey()), 16)
+        my_val = int(binascii.hexlify(self._public_key), 16)
+        other_val = int(binascii.hexlify(other.get_public_key()), 16)
 
-        if myVal < otherVal:
+        if my_val < other_val:
             return -1
-        elif myVal == otherVal:
+        elif my_val == other_val:
             return 0
         else:
             return 1
 
 
 class CurvePublicKey(DjbECPublicKey):
     def serialize(self) -> bytes:
         from .curve import Curve
 
-        combined = ByteUtil.combine([Curve.DJB_TYPE], self._publicKey)
+        combined = ByteUtil.combine([Curve.DJB_TYPE], self._public_key)
         return bytes(combined)
 
     def to_ed(self) -> EdPublicKey:
-        return EdPublicKey(curve.convert_curve_to_ed_pubkey(self._publicKey))
+        return EdPublicKey(curve.convert_curve_to_ed_pubkey(self._public_key))
 
 
 class EdPublicKey(DjbECPublicKey):
     def to_curve(self) -> CurvePublicKey:
-        return CurvePublicKey(curve.convert_ed_to_curve_pubkey(self._publicKey))
+        return CurvePublicKey(curve.convert_ed_to_curve_pubkey(self._public_key))
 
     def serialize(self) -> bytes:
-        return self._publicKey
+        return self._public_key
 
 
 class DjbECPrivateKey(ECPrivateKey):
-    def __init__(self, privateKey: bytes) -> None:
-        self.privateKey = privateKey
+    def __init__(self, private_key: bytes) -> None:
+        self._private_key = private_key
 
-    def getType(self) -> int:
+    def get_type(self) -> int:
         from .curve import Curve
 
         return Curve.DJB_TYPE
 
-    def getPrivateKey(self) -> bytes:
-        return self.privateKey
+    def get_private_key(self) -> bytes:
+        return self._private_key
 
     def serialize(self) -> bytes:
-        return self.privateKey
+        return self._private_key
 
     def __eq__(self, other: Any) -> bool:
-        return self.privateKey == other.getPrivateKey()
+        return self._private_key == other.get_private_key()
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/identitykeypair.py` & `omemo-dr-0.99.1/src/omemo_dr/identitykeypair.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,35 +13,35 @@
 class IdentityKeyPair:
     def __init__(self, structure: IdentityKeyPairStructureProto) -> None:
         self._structure = structure
 
     @classmethod
     def new(
         cls,
-        identityKeyPublicKey: IdentityKey,
-        ecPrivateKey: DjbECPrivateKey,
+        identity_key_public_key: IdentityKey,
+        ec_private_key: DjbECPrivateKey,
     ) -> IdentityKeyPair:
         structure = cast(IdentityKeyPairStructureProto, IdentityKeyPairStructure())
 
-        structure.publicKey = identityKeyPublicKey.serialize()
-        structure.privateKey = ecPrivateKey.serialize()
+        structure.publicKey = identity_key_public_key.serialize()
+        structure.privateKey = ec_private_key.serialize()
 
         return cls(structure)
 
     @classmethod
     def from_bytes(cls, serialized: bytes) -> IdentityKeyPair:
         structure = cast(IdentityKeyPairStructureProto, IdentityKeyPairStructure())
         structure.ParseFromString(serialized)
         return cls(structure)
 
-    def getPublicKey(self) -> IdentityKey:
+    def get_public_key(self) -> IdentityKey:
         return IdentityKey(bytearray(self._structure.publicKey), offset=0)
 
-    def getPrivateKey(self) -> DjbECPrivateKey:
-        return Curve.decodePrivatePoint(bytearray(self._structure.privateKey))
+    def get_private_key(self) -> DjbECPrivateKey:
+        return Curve.decode_private_point(bytearray(self._structure.privateKey))
 
     def serialize(self) -> bytes:
         return self._structure.SerializeToString()
 
 
 class IdentityKeyPairStructureProto(google.protobuf.message.Message):
     publicKey: bytes
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/kdf/hkdf.py` & `omemo-dr-0.99.1/src/omemo_dr/kdf/hkdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,57 +6,57 @@
 import hmac
 import math
 
 
 class HKDF:
     HASH_OUTPUT_SIZE = 32
 
-    def __init__(self, sessionVersion: int) -> None:
-        if sessionVersion not in (2, 3, 4):
-            raise AssertionError("Unknown version: %s " % sessionVersion)
+    def __init__(self, session_version: int) -> None:
+        if session_version not in (2, 3, 4):
+            raise AssertionError("Unknown version: %s " % session_version)
 
-        self.sessionVersion = sessionVersion
+        self.session_version = session_version
 
-    def deriveSecrets(
+    def derive_secrets(
         self,
-        inputKeyMaterial: bytes,
+        input_key_material: bytes,
         info: bytes,
-        outputLength: int,
+        output_length: int,
         salt: Optional[bytes] = None,
     ) -> bytes:
         salt = salt or bytearray(self.HASH_OUTPUT_SIZE)
-        prk = self.extract(salt, inputKeyMaterial)
-        return self.expand(prk, info, outputLength)
+        prk = self._extract(salt, input_key_material)
+        return self._expand(prk, info, output_length)
 
-    def extract(self, salt: bytes, inputKeyMaterial: bytes) -> bytes:
+    def _extract(self, salt: bytes, input_key_material: bytes) -> bytes:
         mac = hmac.new(bytes(salt), digestmod=hashlib.sha256)
-        mac.update(bytes(inputKeyMaterial))
+        mac.update(bytes(input_key_material))
         return mac.digest()
 
-    def expand(self, prk: bytes, info: bytes, outputSize: int) -> bytes:
-        iterations = int(math.ceil(float(outputSize) / float(self.HASH_OUTPUT_SIZE)))
+    def _expand(self, prk: bytes, info: bytes, output_size: int) -> bytes:
+        iterations = int(math.ceil(float(output_size) / float(self.HASH_OUTPUT_SIZE)))
         mixin = bytearray()
         results = bytearray()
-        remainingBytes = outputSize
+        remaining_bytes = output_size
 
         for i in range(
-            self.getIterationStartOffset(), iterations + self.getIterationStartOffset()
+            self._get_iteration_start_offset(),
+            iterations + self._get_iteration_start_offset(),
         ):
             mac = hmac.new(prk, digestmod=hashlib.sha256)
             mac.update(bytes(mixin))
-            if info is not None:
-                mac.update(bytes(info))
+            mac.update(bytes(info))
             updateChr = chr(i % 256)
             mac.update(updateChr.encode())
 
             stepResult = mac.digest()
-            stepSize = min(remainingBytes, len(stepResult))
+            stepSize = min(remaining_bytes, len(stepResult))
             results.extend(stepResult[:stepSize])
             mixin = stepResult
-            remainingBytes -= stepSize
+            remaining_bytes -= stepSize
 
         return bytes(results)
 
-    def getIterationStartOffset(self) -> int:
-        if self.sessionVersion == 2:
+    def _get_iteration_start_offset(self) -> int:
+        if self.session_version == 2:
             return 0
         return 1
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/protocol/omemo_message.py` & `omemo-dr-0.99.1/src/omemo_dr/protocol/omemo_message.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,66 +12,68 @@
 from ..exceptions import InvalidKeyException
 from ..exceptions import InvalidMessageException
 from ..identitykey import IdentityKey
 from ..util.byteutil import ByteUtil
 from . import omemo_pb2 as omemoprotos
 from .ciphertextmessage import CiphertextMessage
 
+MAC_LENGTH = 16
 
-class OMEMOMessage(CiphertextMessage):
-    MAC_LENGTH = 16
 
+class OMEMOMessage(CiphertextMessage):
     def __init__(
         self,
         serialized: bytes,
-        senderRatchetKey: CurvePublicKey,
+        sender_ratchet_key: CurvePublicKey,
         counter: int,
-        previousCounter: int,
+        previous_counter: int,
         ciphertext: bytes,
     ):
-        self.serialized = serialized
-        self.senderRatchetKey = senderRatchetKey
-        self.counter = counter
-        self.previousCounter = previousCounter
-        self.ciphertext = ciphertext
+        self._serialized = serialized
+        self._sender_ratchet_key = sender_ratchet_key
+        self._counter = counter
+        self._previous_counter = previous_counter
+        self._ciphertext = ciphertext
 
     @classmethod
     def new(
         cls,
-        messageVersion: int,
-        macKey: bytes,
-        ECPublicKey_senderRatchetKey: CurvePublicKey,
+        message_version: int,
+        mac_key: bytes,
+        ec_public_key_sender_ratchet_key: CurvePublicKey,
         counter: int,
-        previousCounter: int,
+        previous_counter: int,
         ciphertext: bytes,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
     ) -> OMEMOMessage:
         omemo_message = cast(OMEMOMessageProto, omemoprotos.OMEMOMessage())
 
-        omemo_message.dh_pub = ECPublicKey_senderRatchetKey.serialize()
+        omemo_message.dh_pub = ec_public_key_sender_ratchet_key.serialize()
         omemo_message.n = counter
-        omemo_message.pn = previousCounter
+        omemo_message.pn = previous_counter
         omemo_message.ciphertext = ciphertext
         omemo_message = omemo_message.SerializeToString()
 
-        mac = cls.getMac(senderIdentityKey, receiverIdentityKey, macKey, omemo_message)
+        mac = cls.get_mac(
+            sender_identity_key, receiver_identity_key, mac_key, omemo_message
+        )
 
         authenticated_message = cast(
             OMEMOAuthenticatedMessageProto, omemoprotos.OMEMOAuthenticatedMessage()
         )
         authenticated_message.mac = mac
         authenticated_message.message = omemo_message
         authenticated_message = authenticated_message.SerializeToString()
 
         return cls(
             authenticated_message,
-            ECPublicKey_senderRatchetKey,
+            ec_public_key_sender_ratchet_key,
             counter,
-            previousCounter,
+            previous_counter,
             ciphertext,
         )
 
     @classmethod
     def from_bytes(cls, serialized: bytes) -> OMEMOMessage:
         authenticated_message = cast(
             OMEMOAuthenticatedMessageProto, omemoprotos.OMEMOAuthenticatedMessage()
@@ -85,76 +87,78 @@
 
         try:
             omemo_message.ParseFromString(authenticated_message.message)
         except google.protobuf.message.DecodeError as error:
             raise InvalidMessageException(str(error))
 
         try:
-            senderRatchetKey = Curve.decodePoint(bytearray(omemo_message.dh_pub), 0)
-            assert isinstance(senderRatchetKey, CurvePublicKey)
+            sender_ratchet_key = Curve.decode_point(bytearray(omemo_message.dh_pub), 0)
+            assert isinstance(sender_ratchet_key, CurvePublicKey)
         except InvalidKeyException as error:
             raise InvalidMessageException(str(error))
 
         return OMEMOMessage(
             serialized,
-            senderRatchetKey,
+            sender_ratchet_key,
             omemo_message.n,
             omemo_message.pn,
             omemo_message.ciphertext,
         )
 
-    def getSenderRatchetKey(self) -> CurvePublicKey:
-        return self.senderRatchetKey
+    def get_sender_ratchet_key(self) -> CurvePublicKey:
+        return self._sender_ratchet_key
 
-    def getMessageVersion(self) -> int:
+    def get_message_version(self) -> int:
         return 4
 
-    def getCounter(self) -> int:
-        return self.counter
+    def get_counter(self) -> int:
+        return self._counter
 
-    def getBody(self) -> bytes:
-        return self.ciphertext
+    def get_body(self) -> bytes:
+        return self._ciphertext
 
-    def verifyMac(
+    def verify_mac(
         self,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
-        macKey: bytes,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
+        mac_key: bytes,
     ):
         parts = ByteUtil.split(
-            self.serialized,
-            len(self.serialized) - self.__class__.MAC_LENGTH,
-            self.__class__.MAC_LENGTH,
+            self._serialized,
+            len(self._serialized) - MAC_LENGTH,
+            MAC_LENGTH,
         )
 
-        ourMac = self.getMac(senderIdentityKey, receiverIdentityKey, macKey, parts[0])
-        theirMac = parts[1]
+        our_mac = self.get_mac(
+            sender_identity_key, receiver_identity_key, mac_key, parts[0]
+        )
+        their_mac = parts[1]
 
-        if ourMac != theirMac:
+        if our_mac != their_mac:
             raise InvalidMessageException("Bad Mac!")
 
     @classmethod
-    def getMac(
+    def get_mac(
         cls,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
-        macKey: bytes,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
+        mac_key: bytes,
         serialized: bytes,
     ) -> bytes:
-        mac = hmac.new(macKey, digestmod=hashlib.sha256)
-        mac.update(senderIdentityKey.getPublicKey().serialize())
-        mac.update(receiverIdentityKey.getPublicKey().serialize())
+        mac = hmac.new(mac_key, digestmod=hashlib.sha256)
+        mac.update(sender_identity_key.get_public_key().serialize())
+        mac.update(receiver_identity_key.get_public_key().serialize())
         mac.update(bytes(serialized))
-        fullMac = mac.digest()
-        return ByteUtil.trim(fullMac, cls.MAC_LENGTH)
+        full_mac = mac.digest()
+        return ByteUtil.trim(full_mac, MAC_LENGTH)
 
     def serialize(self) -> bytes:
-        return self.serialized
+        return self._serialized
 
-    def getType(self) -> int:
+    def get_type(self) -> int:
         return CiphertextMessage.WHISPER_TYPE
 
 
 class OMEMOMessageProto(google.protobuf.message.Message):
     n: int
     pn: int
     dh_pub: bytes
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/protocol/omemo_pb2.py` & `omemo-dr-0.99.1/src/omemo_dr/protocol/omemo_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/src/omemo_dr/protocol/whispermessage.py` & `omemo-dr-0.99.1/src/omemo_dr/protocol/whispermessage.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,154 +12,155 @@
 from ..exceptions import InvalidKeyException
 from ..exceptions import InvalidMessageException
 from ..identitykey import IdentityKey
 from ..util.byteutil import ByteUtil
 from . import whisperprotos_pb2 as whisperprotos
 from .ciphertextmessage import CiphertextMessage
 
+MAC_LENGTH = 8
 
-class WhisperMessage(CiphertextMessage):
-    MAC_LENGTH = 8
 
+class WhisperMessage(CiphertextMessage):
     def __init__(
         self,
         serialized: bytes,
-        senderRatchetKey: CurvePublicKey,
+        sender_ratchet_key: CurvePublicKey,
         counter: int,
-        previousCounter: int,
+        previous_counter: int,
         ciphertext: bytes,
     ) -> None:
-        self.serialized = serialized
-        self.senderRatchetKey = senderRatchetKey
-        self.counter = counter
-        self.previousCounter = previousCounter
-        self.ciphertext = ciphertext
+        self._serialized = serialized
+        self._sender_ratchet_key = sender_ratchet_key
+        self._counter = counter
+        self._previous_counter = previous_counter
+        self._ciphertext = ciphertext
 
     @classmethod
     def new(
         cls,
-        messageVersion: int,
-        macKey: bytes,
-        ECPublicKey_senderRatchetKey: CurvePublicKey,
+        message_version: int,
+        mac_key: bytes,
+        ec_public_key_sender_ratchet_key: CurvePublicKey,
         counter: int,
-        previousCounter: int,
+        previous_counter: int,
         ciphertext: bytes,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
     ) -> WhisperMessage:
-        version = ByteUtil.intsToByteHighAndLow(messageVersion, messageVersion)
+        version = ByteUtil.ints_to_byte_high_and_low(message_version, message_version)
 
         message = cast(WhisperMessageProto, whisperprotos.WhisperMessage())
-        message.ratchetKey = ECPublicKey_senderRatchetKey.serialize()
+        message.ratchetKey = ec_public_key_sender_ratchet_key.serialize()
         message.counter = counter
-        message.previousCounter = previousCounter
+        message.previousCounter = previous_counter
         message.ciphertext = ciphertext
         message = message.SerializeToString()
 
-        mac = cls.getMac(
-            senderIdentityKey,
-            receiverIdentityKey,
-            macKey,
+        mac = cls.get_mac(
+            sender_identity_key,
+            receiver_identity_key,
+            mac_key,
             ByteUtil.combine(version, message),
         )
 
         serialized = bytes(ByteUtil.combine(version, message, mac))
 
         return cls(
             serialized,
-            ECPublicKey_senderRatchetKey,
+            ec_public_key_sender_ratchet_key,
             counter,
-            previousCounter,
+            previous_counter,
             ciphertext,
         )
 
     @classmethod
     def from_bytes(cls, serialized: bytes) -> WhisperMessage:
-        messageParts = ByteUtil.split(
+        message_parts = ByteUtil.split(
             serialized,
             1,
-            len(serialized) - 1 - WhisperMessage.MAC_LENGTH,
-            WhisperMessage.MAC_LENGTH,
+            len(serialized) - 1 - MAC_LENGTH,
+            MAC_LENGTH,
         )
 
-        version = ByteUtil.highBitsToInt(messageParts[0][0])
-        message = messageParts[1]
-        _mac = messageParts[2]
+        version = ByteUtil.high_bits_to_int(message_parts[0][0])
+        message = message_parts[1]
 
         if version != 3:
             raise InvalidMessageException("Unknown version: %s" % version)
 
-        whisperMessage = cast(WhisperMessageProto, whisperprotos.WhisperMessage())
-        whisperMessage.ParseFromString(message)
+        whisper_message = cast(WhisperMessageProto, whisperprotos.WhisperMessage())
+        whisper_message.ParseFromString(message)
 
-        if not whisperMessage.ciphertext or not whisperMessage.ratchetKey:
+        if not whisper_message.ciphertext or not whisper_message.ratchetKey:
             raise InvalidMessageException("Incomplete message")
 
         try:
-            senderRatchetKey = Curve.decodePoint(
-                bytearray(whisperMessage.ratchetKey), 0
+            sender_ratchet_key = Curve.decode_point(
+                bytearray(whisper_message.ratchetKey), 0
             )
-            assert isinstance(senderRatchetKey, CurvePublicKey)
+            assert isinstance(sender_ratchet_key, CurvePublicKey)
         except InvalidKeyException as e:
             raise InvalidMessageException(str(e))
 
         return WhisperMessage(
             serialized,
-            senderRatchetKey,
-            whisperMessage.counter,
-            whisperMessage.previousCounter,
-            whisperMessage.ciphertext,
+            sender_ratchet_key,
+            whisper_message.counter,
+            whisper_message.previousCounter,
+            whisper_message.ciphertext,
         )
 
-    def getSenderRatchetKey(self) -> CurvePublicKey:
-        return self.senderRatchetKey
+    def get_sender_ratchet_key(self) -> CurvePublicKey:
+        return self._sender_ratchet_key
 
-    def getMessageVersion(self) -> int:
+    def get_message_version(self) -> int:
         return 3
 
-    def getCounter(self) -> int:
-        return self.counter
+    def get_counter(self) -> int:
+        return self._counter
 
-    def getBody(self) -> bytes:
-        return self.ciphertext
+    def get_body(self) -> bytes:
+        return self._ciphertext
 
-    def verifyMac(
+    def verify_mac(
         self,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
-        macKey: bytes,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
+        mac_key: bytes,
     ) -> None:
         parts = ByteUtil.split(
-            self.serialized, len(self.serialized) - self.MAC_LENGTH, self.MAC_LENGTH
+            self._serialized, len(self._serialized) - MAC_LENGTH, MAC_LENGTH
+        )
+        our_mac = self.get_mac(
+            sender_identity_key, receiver_identity_key, mac_key, parts[0]
         )
-        ourMac = self.getMac(senderIdentityKey, receiverIdentityKey, macKey, parts[0])
-        theirMac = parts[1]
+        their_mac = parts[1]
 
-        if ourMac != theirMac:
+        if our_mac != their_mac:
             raise InvalidMessageException("Bad Mac!")
 
     @classmethod
-    def getMac(
+    def get_mac(
         cls,
-        senderIdentityKey: IdentityKey,
-        receiverIdentityKey: IdentityKey,
-        macKey: bytes,
+        sender_identity_key: IdentityKey,
+        receiver_identity_key: IdentityKey,
+        mac_key: bytes,
         serialized: bytes,
     ) -> bytes:
-        mac = hmac.new(macKey, digestmod=hashlib.sha256)
-        mac.update(senderIdentityKey.getPublicKey().serialize())
-        mac.update(receiverIdentityKey.getPublicKey().serialize())
+        mac = hmac.new(mac_key, digestmod=hashlib.sha256)
+        mac.update(sender_identity_key.get_public_key().serialize())
+        mac.update(receiver_identity_key.get_public_key().serialize())
         mac.update(serialized)
-        fullMac = mac.digest()
-        return ByteUtil.trim(fullMac, cls.MAC_LENGTH)
+        full_mac = mac.digest()
+        return ByteUtil.trim(full_mac, MAC_LENGTH)
 
     def serialize(self) -> bytes:
-        return self.serialized
+        return self._serialized
 
-    def getType(self) -> int:
+    def get_type(self) -> int:
         return CiphertextMessage.WHISPER_TYPE
 
 
 class WhisperMessageProto(google.protobuf.message.Message):
     ratchetKey: bytes
     counter: int
     previousCounter: int
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/protocol/whisperprotos_pb2.py` & `omemo-dr-0.99.1/src/omemo_dr/protocol/whisperprotos_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/src/omemo_dr/ratchet/chainkey.py` & `omemo-dr-0.99.1/src/omemo_dr/ratchet/chainkey.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,41 +13,41 @@
     CHAIN_KEY_SEED = bytearray([0x02])
 
     def __init__(self, kdf: HKDF, key: bytes, index: int) -> None:
         self.kdf = kdf
         self.key = key
         self.index = index
 
-    def getKey(self) -> bytes:
+    def get_key(self) -> bytes:
         return self.key
 
-    def getIndex(self) -> int:
+    def get_index(self) -> int:
         return self.index
 
-    def getNextChainKey(self) -> ChainKey:
-        nextKey = self.getBaseMaterial(self.__class__.CHAIN_KEY_SEED)
+    def get_next_chain_key(self) -> ChainKey:
+        nextKey = self.get_base_material(self.__class__.CHAIN_KEY_SEED)
         return ChainKey(self.kdf, nextKey, self.index + 1)
 
-    def getMessageKeys(self) -> MessageKeys:
-        if self.kdf.sessionVersion <= 3:
+    def get_message_keys(self) -> MessageKeys:
+        if self.kdf.session_version <= 3:
             domain_separator = "WhisperMessageKeys"
         else:
             domain_separator = "OMEMO Message Key Material"
 
-        inputKeyMaterial = self.getBaseMaterial(self.__class__.MESSAGE_KEY_SEED)
-        keyMaterialBytes = self.kdf.deriveSecrets(
-            inputKeyMaterial,
+        input_key_material = self.get_base_material(self.__class__.MESSAGE_KEY_SEED)
+        key_material_bytes = self.kdf.derive_secrets(
+            input_key_material,
             bytearray(domain_separator.encode()),
             DerivedMessageSecrets.SIZE,
         )
-        keyMaterial = DerivedMessageSecrets(keyMaterialBytes)
+        key_material = DerivedMessageSecrets(key_material_bytes)
         return MessageKeys(
-            keyMaterial.getCipherKey(),
-            keyMaterial.getMacKey(),
-            keyMaterial.getIv(),
+            key_material.get_cipher_key(),
+            key_material.get_mac_key(),
+            key_material.get_iv(),
             self.index,
         )
 
-    def getBaseMaterial(self, seedBytes: bytes) -> bytes:
+    def get_base_material(self, seedBytes: bytes) -> bytes:
         mac = hmac.new(bytes(self.key), digestmod=hashlib.sha256)
         mac.update(bytes(seedBytes))
         return mac.digest()
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/ratchet/ratchetingsession.py` & `omemo-dr-0.99.1/src/omemo_dr/ratchet/ratchetingsession.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,161 @@
 from __future__ import annotations
 
 from ..ecc.curve import Curve
 from ..ecc.ec import ECPublicKey
 from ..kdf.hkdf import HKDF
 from ..state.sessionstate import SessionState
 from ..util.byteutil import ByteUtil
-from .aliceaxolotlparameters import AliceAxolotlParameters
-from .bobaxolotlparamaters import BobAxolotlParameters
+from .aliceparameters import AliceParameters
+from .bobparameters import BobParameters
 from .chainkey import ChainKey
 from .rootkey import RootKey
 
 
 class RatchetingSession:
     @staticmethod
-    def initializeSessionAsAlice(
-        sessionState: SessionState,
-        sessionVersion: int,
-        parameters: AliceAxolotlParameters,
+    def initialize_session_as_alice(
+        session_state: SessionState,
+        session_version: int,
+        parameters: AliceParameters,
     ) -> None:
-        sessionState.setSessionVersion(sessionVersion)
-        sessionState.setRemoteIdentityKey(parameters.getTheirIdentityKey())
-        sessionState.setLocalIdentityKey(parameters.getOurIdentityKey().getPublicKey())
+        session_state.set_session_version(session_version)
+        session_state.set_remote_identity_key(parameters.get_their_identity_key())
+        session_state.set_local_identity_key(
+            parameters.get_our_identity_key().get_public_key()
+        )
 
-        sendingRatchetKey = Curve.generateKeyPair()
+        sending_ratchet_key = Curve.generate_key_pair()
         secrets = bytearray()
 
-        if sessionVersion >= 3:
-            secrets.extend(RatchetingSession.getDiscontinuityBytes())
+        if session_version >= 3:
+            secrets.extend(RatchetingSession.get_discontinuity_bytes())
 
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirSignedPreKey(),
-                parameters.getOurIdentityKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_signed_pre_key(),
+                parameters.get_our_identity_key().get_private_key(),
             )
         )
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirIdentityKey().getPublicKey(),
-                parameters.getOurBaseKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_identity_key().get_public_key(),
+                parameters.get_our_base_key().get_private_key(),
             )
         )
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirSignedPreKey(),
-                parameters.getOurBaseKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_signed_pre_key(),
+                parameters.get_our_base_key().get_private_key(),
             )
         )
 
-        if sessionVersion >= 3 and parameters.getTheirOneTimePreKey() is not None:
+        if session_version >= 3 and parameters.get_their_one_time_pre_key() is not None:
             secrets.extend(
-                Curve.calculateAgreement(
-                    parameters.getTheirOneTimePreKey(),
-                    parameters.getOurBaseKey().getPrivateKey(),
+                Curve.calculate_agreement(
+                    parameters.get_their_one_time_pre_key(),
+                    parameters.get_our_base_key().get_private_key(),
                 )
             )
 
-        derivedKeys = RatchetingSession.calculateDerivedKeys(sessionVersion, secrets)
-        sendingChain = derivedKeys.getRootKey().createChain(
-            parameters.getTheirRatchetKey(), sendingRatchetKey
+        derived_keys = RatchetingSession.calculate_derived_keys(
+            session_version, secrets
+        )
+        sending_chain = derived_keys.get_root_key().create_chain(
+            parameters.get_their_ratchet_key(), sending_ratchet_key
         )
 
-        sessionState.addReceiverChain(
-            parameters.getTheirRatchetKey(), derivedKeys.getChainKey()
+        session_state.add_receiver_chain(
+            parameters.get_their_ratchet_key(), derived_keys.get_chain_key()
         )
-        sessionState.setSenderChain(sendingRatchetKey, sendingChain[1])
-        sessionState.setRootKey(sendingChain[0])
+        session_state.set_sender_chain(sending_ratchet_key, sending_chain[1])
+        session_state.set_root_key(sending_chain[0])
 
     @staticmethod
-    def initializeSessionAsBob(
-        sessionState: SessionState,
-        sessionVersion: int,
-        parameters: BobAxolotlParameters,
+    def initialize_session_as_bob(
+        session_state: SessionState,
+        session_version: int,
+        parameters: BobParameters,
     ) -> None:
-        sessionState.setSessionVersion(sessionVersion)
-        sessionState.setRemoteIdentityKey(parameters.getTheirIdentityKey())
-        sessionState.setLocalIdentityKey(parameters.getOurIdentityKey().getPublicKey())
+        session_state.set_session_version(session_version)
+        session_state.set_remote_identity_key(parameters.get_their_identity_key())
+        session_state.set_local_identity_key(
+            parameters.get_our_identity_key().get_public_key()
+        )
 
         secrets = bytearray()
 
-        if sessionVersion >= 3:
-            secrets.extend(RatchetingSession.getDiscontinuityBytes())
+        if session_version >= 3:
+            secrets.extend(RatchetingSession.get_discontinuity_bytes())
 
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirIdentityKey().getPublicKey(),
-                parameters.getOurSignedPreKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_identity_key().get_public_key(),
+                parameters.get_our_signed_pre_key().get_private_key(),
             )
         )
 
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirBaseKey(),
-                parameters.getOurIdentityKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_base_key(),
+                parameters.get_our_identity_key().get_private_key(),
             )
         )
         secrets.extend(
-            Curve.calculateAgreement(
-                parameters.getTheirBaseKey(),
-                parameters.getOurSignedPreKey().getPrivateKey(),
+            Curve.calculate_agreement(
+                parameters.get_their_base_key(),
+                parameters.get_our_signed_pre_key().get_private_key(),
             )
         )
 
-        if sessionVersion >= 3 and parameters.getOurOneTimePreKey() is not None:
+        our_one_time_pre_key = parameters.get_our_one_time_pre_key()
+        if session_version >= 3 and our_one_time_pre_key is not None:
             secrets.extend(
-                Curve.calculateAgreement(
-                    parameters.getTheirBaseKey(),
-                    parameters.getOurOneTimePreKey().getPrivateKey(),
+                Curve.calculate_agreement(
+                    parameters.get_their_base_key(),
+                    our_one_time_pre_key.get_private_key(),
                 )
             )
 
-        derivedKeys = RatchetingSession.calculateDerivedKeys(sessionVersion, secrets)
-        sessionState.setSenderChain(
-            parameters.getOurRatchetKey(), derivedKeys.getChainKey()
+        derived_keys = RatchetingSession.calculate_derived_keys(
+            session_version, secrets
+        )
+        session_state.set_sender_chain(
+            parameters.get_our_ratchet_key(), derived_keys.get_chain_key()
         )
-        sessionState.setRootKey(derivedKeys.getRootKey())
+        session_state.set_root_key(derived_keys.get_root_key())
 
     @staticmethod
-    def getDiscontinuityBytes() -> bytearray:
+    def get_discontinuity_bytes() -> bytearray:
         return bytearray([0xFF] * 32)
 
     @staticmethod
-    def calculateDerivedKeys(sessionVersion: int, masterSecret: bytes) -> DerivedKeys:
-        if sessionVersion <= 3:
+    def calculate_derived_keys(
+        session_version: int, master_secret: bytes
+    ) -> DerivedKeys:
+        if session_version <= 3:
             domain_separator = "WhisperText"
         else:
             domain_separator = "OMEMO Payload"
-        kdf = HKDF(sessionVersion)
-        derivedSecretBytes = kdf.deriveSecrets(
-            masterSecret, bytearray(domain_separator.encode()), 64
+        kdf = HKDF(session_version)
+        derived_secret_bytes = kdf.derive_secrets(
+            master_secret, bytearray(domain_separator.encode()), 64
         )
-        derivedSecrets = ByteUtil.split(derivedSecretBytes, 32, 32)
+        derived_secrets = ByteUtil.split(derived_secret_bytes, 32, 32)
         return RatchetingSession.DerivedKeys(
-            RootKey(kdf, derivedSecrets[0]), ChainKey(kdf, derivedSecrets[1], 0)
+            RootKey(kdf, derived_secrets[0]), ChainKey(kdf, derived_secrets[1], 0)
         )
 
     @staticmethod
-    def isAlice(ourKey: ECPublicKey, theirKey: ECPublicKey) -> bool:
-        return ourKey < theirKey
+    def is_alice(our_key: ECPublicKey, their_key: ECPublicKey) -> bool:
+        return our_key < their_key
 
     class DerivedKeys:
-        def __init__(self, rootKey: RootKey, chainKey: ChainKey):
-            self.rootKey = rootKey
-            self.chainKey = chainKey
+        def __init__(self, root_key: RootKey, chain_key: ChainKey):
+            self._root_key = root_key
+            self._chain_key = chain_key
 
-        def getRootKey(self):
-            return self.rootKey
+        def get_root_key(self):
+            return self._root_key
 
-        def getChainKey(self):
-            return self.chainKey
+        def get_chain_key(self):
+            return self._chain_key
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/ratchet/rootkey.py` & `omemo-dr-0.99.1/src/omemo_dr/ratchet/rootkey.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,35 +9,36 @@
 
 
 class RootKey:
     def __init__(self, kdf: HKDF, key: bytes) -> None:
         self.kdf = kdf
         self.key = key
 
-    def getKeyBytes(self) -> bytes:
+    def get_key_bytes(self) -> bytes:
         return self.key
 
-    def createChain(
+    def create_chain(
         self,
-        ECPublicKey_theirRatchetKey: CurvePublicKey,
-        ECKeyPair_ourRatchetKey: ECKeyPair,
+        ec_public_key_their_ratchet_key: CurvePublicKey,
+        ec_key_pair_our_ratchet_key: ECKeyPair,
     ) -> tuple[RootKey, ChainKey]:
-        if self.kdf.sessionVersion <= 3:
+        if self.kdf.session_version <= 3:
             domain_separator = "WhisperRatchet"
         else:
             domain_separator = "OMEMO Root Chain"
 
-        sharedSecret = Curve.calculateAgreement(
-            ECPublicKey_theirRatchetKey, ECKeyPair_ourRatchetKey.getPrivateKey()
+        shared_secret = Curve.calculate_agreement(
+            ec_public_key_their_ratchet_key,
+            ec_key_pair_our_ratchet_key.get_private_key(),
         )
 
-        derivedSecretBytes = self.kdf.deriveSecrets(
-            sharedSecret,
+        derived_secret_bytes = self.kdf.derive_secrets(
+            shared_secret,
             domain_separator.encode(),
             DerivedRootSecrets.SIZE,
             salt=self.key,
         )
 
-        derivedSecrets = DerivedRootSecrets(derivedSecretBytes)
-        newRootKey = RootKey(self.kdf, derivedSecrets.getRootKey())
-        newChainKey = ChainKey(self.kdf, derivedSecrets.getChainKey(), 0)
-        return (newRootKey, newChainKey)
+        derived_secrets = DerivedRootSecrets(derived_secret_bytes)
+        new_root_key = RootKey(self.kdf, derived_secrets.get_root_key())
+        new_chain_key = ChainKey(self.kdf, derived_secrets.get_chain_key(), 0)
+        return (new_root_key, new_chain_key)
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/sessioncipher.py` & `omemo-dr-0.99.1/src/omemo_dr/sessioncipher.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,274 +15,267 @@
 from .exceptions import InvalidMessageException
 from .exceptions import NoSessionException
 from .kdf.messagekeys import MessageKeys
 from .protocol.prekeywhispermessage import PreKeyWhisperMessage
 from .protocol.whispermessage import WhisperMessage
 from .ratchet.chainkey import ChainKey
 from .sessionbuilder import SessionBuilder
-from .state.identitykeystore import IdentityKeyStore
-from .state.prekeystore import PreKeyStore
 from .state.sessionrecord import SessionRecord
 from .state.sessionstate import SessionState
-from .state.sessionstore import SessionStore
-from .state.signedprekeystore import SignedPreKeyStore
+from .state.store import Store
 
 logger = logging.getLogger(__name__)
 
 
 class SessionCipher:
-    def __init__(
-        self,
-        sessionStore: SessionStore,
-        preKeyStore: PreKeyStore,
-        signedPreKeyStore: SignedPreKeyStore,
-        identityKeyStore: IdentityKeyStore,
-        recipientId: str,
-        deviceId: int,
-    ) -> None:
-        self.sessionStore = sessionStore
-        self.preKeyStore = preKeyStore
-        self.recipientId = recipientId
-        self.deviceId = deviceId
-        self.sessionBuilder = SessionBuilder(
-            sessionStore,
-            preKeyStore,
-            signedPreKeyStore,
-            identityKeyStore,
-            recipientId,
-            deviceId,
+    def __init__(self, store: Store, recipient_id: str, device_id: int) -> None:
+        self._store = store
+        self.recipient_id = recipient_id
+        self.device_id = device_id
+        self.session_builder = SessionBuilder(
+            store,
+            recipient_id,
+            device_id,
         )
 
     def encrypt(
-        self, paddedMessage: Union[bytes, str]
+        self, padded_message: Union[bytes, str]
     ) -> Union[WhisperMessage, PreKeyWhisperMessage]:
-        if isinstance(paddedMessage, str):
-            paddedMessage = paddedMessage.encode()
+        if isinstance(padded_message, str):
+            padded_message = padded_message.encode()
+
+        padded_message = bytearray(padded_message)
 
-        paddedMessage = bytearray(paddedMessage)
+        session_record = self._store.load_session(self.recipient_id, self.device_id)
+        session_state = session_record.get_session_state()
+        chain_key = session_state.get_sender_chain_key()
+        message_keys = chain_key.get_message_keys()
+        sender_ephemeral = session_state.get_sender_ratchet_key()
+        previous_counter = session_state.get_previous_counter()
+        session_version = session_state.get_session_version()
+
+        ciphertext_body = self.get_ciphertext(
+            session_version, message_keys, padded_message
+        )
 
-        sessionRecord = self.sessionStore.loadSession(self.recipientId, self.deviceId)
-        sessionState = sessionRecord.getSessionState()
-        chainKey = sessionState.getSenderChainKey()
-        messageKeys = chainKey.getMessageKeys()
-        senderEphemeral = sessionState.getSenderRatchetKey()
-        previousCounter = sessionState.getPreviousCounter()
-        sessionVersion = sessionState.getSessionVersion()
-
-        ciphertextBody = self.getCiphertext(sessionVersion, messageKeys, paddedMessage)
-
-        ciphertextMessage = WhisperMessage.new(
-            sessionVersion,
-            messageKeys.getMacKey(),
-            senderEphemeral,
-            chainKey.getIndex(),
-            previousCounter,
-            ciphertextBody,
-            sessionState.getLocalIdentityKey(),
-            sessionState.getRemoteIdentityKey(),
+        ciphertext_message = WhisperMessage.new(
+            session_version,
+            message_keys.get_mac_key(),
+            sender_ephemeral,
+            chain_key.get_index(),
+            previous_counter,
+            ciphertext_body,
+            session_state.get_local_identity_key(),
+            session_state.get_remote_identity_key(),
         )
 
-        if sessionState.hasUnacknowledgedPreKeyMessage():
-            items = sessionState.getUnacknowledgedPreKeyMessageItems()
-            localRegistrationid = sessionState.getLocalRegistrationId()
-
-            ciphertextMessage = PreKeyWhisperMessage.new(
-                sessionVersion,
-                localRegistrationid,
-                items.getPreKeyId(),
-                items.getSignedPreKeyId(),
-                items.getBaseKey(),
-                sessionState.getLocalIdentityKey(),
-                ciphertextMessage,
+        if session_state.has_unacknowledged_pre_key_message():
+            items = session_state.get_unacknowledged_pre_key_message_items()
+            local_registrationid = session_state.get_local_registration_id()
+
+            ciphertext_message = PreKeyWhisperMessage.new(
+                session_version,
+                local_registrationid,
+                items.get_pre_key_id(),
+                items.get_signed_pre_key_id(),
+                items.get_base_key(),
+                session_state.get_local_identity_key(),
+                ciphertext_message,
             )
 
-        sessionState.setSenderChainKey(chainKey.getNextChainKey())
-        self.sessionStore.storeSession(self.recipientId, self.deviceId, sessionRecord)
+        session_state.set_sender_chain_key(chain_key.get_next_chain_key())
+        self._store.store_session(self.recipient_id, self.device_id, session_record)
 
-        return ciphertextMessage
+        return ciphertext_message
 
-    def decryptMsg(self, ciphertext: WhisperMessage) -> bytes:
-        if not self.sessionStore.containsSession(self.recipientId, self.deviceId):
+    def decrypt_msg(self, ciphertext: WhisperMessage) -> bytes:
+        if not self._store.contains_session(self.recipient_id, self.device_id):
             raise NoSessionException(
-                "No session for: %s, %s" % (self.recipientId, self.deviceId)
+                "No session for: %s, %s" % (self.recipient_id, self.device_id)
             )
 
-        sessionRecord = self.sessionStore.loadSession(self.recipientId, self.deviceId)
-        plaintext = self.decryptWithSessionRecord(sessionRecord, ciphertext)
+        session_record = self._store.load_session(self.recipient_id, self.device_id)
+        plaintext = self.decrypt_with_session_record(session_record, ciphertext)
 
-        self.sessionStore.storeSession(self.recipientId, self.deviceId, sessionRecord)
+        self._store.store_session(self.recipient_id, self.device_id, session_record)
 
         return plaintext
 
-    def decryptPkmsg(self, ciphertext: PreKeyWhisperMessage) -> bytes:
-        sessionRecord = self.sessionStore.loadSession(self.recipientId, self.deviceId)
-        unsignedPreKeyId = self.sessionBuilder.process(sessionRecord, ciphertext)
-        plaintext = self.decryptWithSessionRecord(
-            sessionRecord, ciphertext.getWhisperMessage()
+    def decrypt_pkmsg(self, ciphertext: PreKeyWhisperMessage) -> bytes:
+        session_record = self._store.load_session(self.recipient_id, self.device_id)
+        unsigned_pre_key_id = self.session_builder.process(session_record, ciphertext)
+        plaintext = self.decrypt_with_session_record(
+            session_record, ciphertext.get_whisper_message()
         )
 
-        self.sessionStore.storeSession(self.recipientId, self.deviceId, sessionRecord)
+        self._store.store_session(self.recipient_id, self.device_id, session_record)
 
-        if unsignedPreKeyId is not None:
-            self.preKeyStore.removePreKey(unsignedPreKeyId)
+        if unsigned_pre_key_id is not None:
+            self._store.remove_pre_key(unsigned_pre_key_id)
 
         return plaintext
 
-    def decryptWithSessionRecord(
-        self, sessionRecord: SessionRecord, cipherText: WhisperMessage
+    def decrypt_with_session_record(
+        self, session_record: SessionRecord, cipher_text: WhisperMessage
     ) -> bytes:
-        previousStates = sessionRecord.getPreviousSessionStates()
+        previous_states = session_record.get_previous_session_states()
         exceptions: list[Exception] = []
         try:
-            sessionState = SessionState(sessionRecord.getSessionState())
-            plaintext = self.decryptWithSessionState(sessionState, cipherText)
-            sessionRecord.setState(sessionState)
+            session_state = SessionState(session_record.get_session_state())
+            plaintext = self.decrypt_with_session_state(session_state, cipher_text)
+            session_record.set_state(session_state)
             return plaintext
         except InvalidMessageException as e:
             exceptions.append(e)
 
-        for i in range(0, len(previousStates)):
-            previousState = previousStates[i]
+        for i in range(0, len(previous_states)):
+            previous_state = previous_states[i]
             try:
-                promotedState = SessionState(previousState)
-                plaintext = self.decryptWithSessionState(promotedState, cipherText)
-                previousStates.pop(i)
-                sessionRecord.promoteState(promotedState)
+                promotedState = SessionState(previous_state)
+                plaintext = self.decrypt_with_session_state(promotedState, cipher_text)
+                previous_states.pop(i)
+                session_record.promote_state(promotedState)
                 return plaintext
             except InvalidMessageException as e:
                 exceptions.append(e)
 
         raise InvalidMessageException("No valid sessions", exceptions)
 
-    def decryptWithSessionState(
-        self, sessionState: SessionState, ciphertextMessage: WhisperMessage
+    def decrypt_with_session_state(
+        self, session_state: SessionState, ciphertext_message: WhisperMessage
     ) -> bytes:
-        if not sessionState.hasSenderChain():
+        if not session_state.has_sender_chain():
             raise InvalidMessageException("Uninitialized session!")
 
-        messageVersion = ciphertextMessage.getMessageVersion()
-        if messageVersion != sessionState.getSessionVersion():
+        message_version = ciphertext_message.get_message_version()
+        if message_version != session_state.get_session_version():
             raise InvalidMessageException(
                 "Message version %s, but session version %s"
                 % (
-                    ciphertextMessage.getMessageVersion,
-                    sessionState.getSessionVersion(),
+                    ciphertext_message.get_message_version,
+                    session_state.get_session_version(),
                 )
             )
 
-        theirEphemeral = ciphertextMessage.getSenderRatchetKey()
-        counter = ciphertextMessage.getCounter()
-        chainKey = self.getOrCreateChainKey(sessionState, theirEphemeral)
-        messageKeys = self.getOrCreateMessageKeys(
-            sessionState, theirEphemeral, chainKey, counter
+        their_ephemeral = ciphertext_message.get_sender_ratchet_key()
+        counter = ciphertext_message.get_counter()
+        chain_key = self.get_or_create_chain_key(session_state, their_ephemeral)
+        message_keys = self.get_or_create_message_keys(
+            session_state, their_ephemeral, chain_key, counter
         )
 
-        ciphertextMessage.verifyMac(
-            sessionState.getRemoteIdentityKey(),
-            sessionState.getLocalIdentityKey(),
-            messageKeys.getMacKey(),
+        ciphertext_message.verify_mac(
+            session_state.get_remote_identity_key(),
+            session_state.get_local_identity_key(),
+            message_keys.get_mac_key(),
         )
 
-        plaintext = self.getPlaintext(
-            messageVersion, messageKeys, ciphertextMessage.getBody()
+        plaintext = self.get_plaintext(
+            message_version, message_keys, ciphertext_message.get_body()
         )
-        sessionState.clearUnacknowledgedPreKeyMessage()
+        session_state.clear_unacknowledged_pre_key_message()
 
         return plaintext
 
-    def getOrCreateChainKey(
-        self, sessionState: SessionState, ECPublickKey_theirEphemeral: CurvePublicKey
+    def get_or_create_chain_key(
+        self,
+        session_state: SessionState,
+        ec_publick_key_their_ephemeral: CurvePublicKey,
     ) -> ChainKey:
-        theirEphemeral = ECPublickKey_theirEphemeral
-        if sessionState.hasReceiverChain(theirEphemeral):
-            return sessionState.getReceiverChainKey(theirEphemeral)
+        their_ephemeral = ec_publick_key_their_ephemeral
+        if session_state.has_receiver_chain(their_ephemeral):
+            return session_state.get_receiver_chain_key(their_ephemeral)
         else:
-            rootKey = sessionState.getRootKey()
-            ourEphemeral = sessionState.getSenderRatchetKeyPair()
-            receiverChain = rootKey.createChain(theirEphemeral, ourEphemeral)
-            ourNewEphemeral = Curve.generateKeyPair()
-            senderChain = receiverChain[0].createChain(theirEphemeral, ourNewEphemeral)
-
-            sessionState.setRootKey(senderChain[0])
-            sessionState.addReceiverChain(theirEphemeral, receiverChain[1])
-            sessionState.setPreviousCounter(
-                max(sessionState.getSenderChainKey().getIndex() - 1, 0)
+            root_key = session_state.get_root_key()
+            our_ephemeral = session_state.get_sender_ratchet_key_pair()
+            receiver_chain = root_key.create_chain(their_ephemeral, our_ephemeral)
+            our_new_ephemeral = Curve.generate_key_pair()
+            sender_chain = receiver_chain[0].create_chain(
+                their_ephemeral, our_new_ephemeral
+            )
+
+            session_state.set_root_key(sender_chain[0])
+            session_state.add_receiver_chain(their_ephemeral, receiver_chain[1])
+            session_state.set_previous_counter(
+                max(session_state.get_sender_chain_key().get_index() - 1, 0)
             )
-            sessionState.setSenderChain(ourNewEphemeral, senderChain[1])
-            return receiverChain[1]
+            session_state.set_sender_chain(our_new_ephemeral, sender_chain[1])
+            return receiver_chain[1]
 
-    def getOrCreateMessageKeys(
+    def get_or_create_message_keys(
         self,
-        sessionState: SessionState,
-        ECPublicKey_theirEphemeral: CurvePublicKey,
-        chainKey: ChainKey,
+        session_state: SessionState,
+        ec_public_key_their_ephemeral: CurvePublicKey,
+        chain_key: ChainKey,
         counter: int,
     ) -> MessageKeys:
-        theirEphemeral = ECPublicKey_theirEphemeral
-        if chainKey.getIndex() > counter:
-            if sessionState.hasMessageKeys(theirEphemeral, counter):
-                return sessionState.removeMessageKeys(theirEphemeral, counter)
+        their_ephemeral = ec_public_key_their_ephemeral
+        if chain_key.get_index() > counter:
+            if session_state.has_message_keys(their_ephemeral, counter):
+                return session_state.remove_message_keys(their_ephemeral, counter)
             else:
                 raise DuplicateMessageException(
                     "Received message with old counter: %s, %s"
-                    % (chainKey.getIndex(), counter)
+                    % (chain_key.get_index(), counter)
                 )
 
-        if counter - chainKey.getIndex() > 2000:
+        if counter - chain_key.get_index() > 2000:
             raise InvalidMessageException("Over 2000 messages into the future!")
 
-        while chainKey.getIndex() < counter:
-            messageKeys = chainKey.getMessageKeys()
-            sessionState.setMessageKeys(theirEphemeral, messageKeys)
-            chainKey = chainKey.getNextChainKey()
+        while chain_key.get_index() < counter:
+            message_keys = chain_key.get_message_keys()
+            session_state.set_message_keys(their_ephemeral, message_keys)
+            chain_key = chain_key.get_next_chain_key()
 
-        sessionState.setReceiverChainKey(theirEphemeral, chainKey.getNextChainKey())
-        return chainKey.getMessageKeys()
+        session_state.set_receiver_chain_key(
+            their_ephemeral, chain_key.get_next_chain_key()
+        )
+        return chain_key.get_message_keys()
 
-    def getCiphertext(
-        self, version: int, messageKeys: MessageKeys, plainText: bytearray
+    def get_ciphertext(
+        self, version: int, message_keys: MessageKeys, plain_text: bytearray
     ) -> bytes:
-        cipher = AESCipher(messageKeys.getCipherKey(), messageKeys.getIv())
-        return cipher.encrypt(bytes(plainText))
+        cipher = AESCipher(message_keys.get_cipher_key(), message_keys.get_iv())
+        return cipher.encrypt(bytes(plain_text))
 
-    def getPlaintext(
-        self, version: int, messageKeys: MessageKeys, cipherText: bytes
+    def get_plaintext(
+        self, version: int, message_keys: MessageKeys, cipher_text: bytes
     ) -> bytes:
-        cipher = AESCipher(messageKeys.getCipherKey(), messageKeys.getIv())
-        return cipher.decrypt(cipherText)
+        cipher = AESCipher(message_keys.get_cipher_key(), message_keys.get_iv())
+        return cipher.decrypt(cipher_text)
 
 
 class AESCipher:
     def __init__(self, key: bytes, iv: bytes) -> None:
         self.key = key
         self.iv = iv
         self.cipher = Cipher(
             algorithms.AES(key), modes.CBC(iv), backend=default_backend()
         )
 
     def unpad(self, data: bytes) -> bytes:
-        unpadLength = data[-1]
-        if isinstance(unpadLength, int):  # pyright: ignore
-            cmp = bytes([data[-unpadLength]] * unpadLength)
+        unpad_length = data[-1]
+        if isinstance(unpad_length, int):  # pyright: ignore
+            cmp = bytes([data[-unpad_length]] * unpad_length)
         else:
-            raise AssertionError("unpadLength is not integer")
-            # unpadLength = ord(unpadLength)
-            # cmp = data[-unpadLength] * unpadLength
-        if data[-unpadLength:] != cmp:
+            raise AssertionError("unpad_length is not integer")
+            # unpad_length = ord(unpad_length)
+            # cmp = data[-unpad_length] * unpad_length
+        if data[-unpad_length:] != cmp:
             raise ValueError("Data not properly padded \n %s" % data)
 
-        return data[0:-unpadLength]
+        return data[0:-unpad_length]
 
     def pad(self, s: bytes) -> bytes:
         return s + ((16 - len(s) % 16) * chr(16 - len(s) % 16)).encode()
 
     def encrypt(self, raw: bytes) -> bytes:
-        rawPadded = self.pad(raw)
+        raw_padded = self.pad(raw)
         encryptor = self.cipher.encryptor()
         try:
-            return encryptor.update(rawPadded) + encryptor.finalize()
+            return encryptor.update(raw_padded) + encryptor.finalize()
         except ValueError:
             raise
 
     def decrypt(self, enc: bytes) -> bytes:
         decryptor = self.cipher.decryptor()
         return self.unpad(decryptor.update(enc) + decryptor.finalize())
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/state/prekeybundle.py` & `omemo-dr-0.99.1/src/omemo_dr/state/prekeybundle.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,60 +5,60 @@
 from ..ecc.ec import ECPublicKey
 from ..identitykey import IdentityKey
 
 
 class PreKeyBundle:
     def __init__(
         self,
-        registrationId: int,
-        deviceId: int,
-        preKeyId: int,
-        ECPublicKey_preKeyPublic: ECPublicKey,
-        signedPreKeyId: int,
-        ECPublicKey_signedPreKeyPublic: ECPublicKey,
-        signedPreKeySignature: bytes,
-        identityKey: IdentityKey,
+        registration_id: int,
+        device_id: int,
+        pre_key_id: int,
+        ec_public_key_pre_key_public: ECPublicKey,
+        signed_pre_key_id: int,
+        ec_public_key_signed_pre_key_public: ECPublicKey,
+        signed_pre_key_signature: bytes,
+        identity_key: IdentityKey,
     ) -> None:
-        self.registrationId = registrationId
-        self.deviceId = deviceId
-        self.preKeyId = preKeyId
-        self.preKeyPublic = ECPublicKey_preKeyPublic
-        self.signedPreKeyId = signedPreKeyId
-        self.signedPreKeyPublic = ECPublicKey_signedPreKeyPublic
-        self.signedPreKeySignature = signedPreKeySignature
-        self.identityKey = identityKey
-
-    def getDeviceId(self) -> int:
-        return self.deviceId
-
-    def getPreKeyId(self) -> int:
-        return self.preKeyId
-
-    def getPreKey(self) -> ECPublicKey:
-        return self.preKeyPublic
-
-    def getSignedPreKeyId(self) -> int:
-        return self.signedPreKeyId
-
-    def getSignedPreKey(self) -> ECPublicKey:
-        return self.signedPreKeyPublic
-
-    def getSignedPreKeySignature(self) -> bytes:
-        return self.signedPreKeySignature
-
-    def getIdentityKey(self) -> IdentityKey:
-        return self.identityKey
-
-    def getRegistrationId(self) -> int:
-        return self.registrationId
-
-    def getSessionVersion(self) -> int:
-        publicKey = self.identityKey.getPublicKey()
-        if isinstance(publicKey, CurvePublicKey):
+        self.registration_id = registration_id
+        self.device_id = device_id
+        self.pre_key_id = pre_key_id
+        self.pre_key_public = ec_public_key_pre_key_public
+        self.signed_pre_key_id = signed_pre_key_id
+        self.signed_pre_key_public = ec_public_key_signed_pre_key_public
+        self.signed_pre_key_signature = signed_pre_key_signature
+        self.identity_key = identity_key
+
+    def get_device_id(self) -> int:
+        return self.device_id
+
+    def get_pre_key_id(self) -> int:
+        return self.pre_key_id
+
+    def get_pre_key(self) -> ECPublicKey:
+        return self.pre_key_public
+
+    def get_signed_pre_key_id(self) -> int:
+        return self.signed_pre_key_id
+
+    def get_signed_pre_key(self) -> ECPublicKey:
+        return self.signed_pre_key_public
+
+    def get_signed_pre_key_signature(self) -> bytes:
+        return self.signed_pre_key_signature
+
+    def get_identity_key(self) -> IdentityKey:
+        return self.identity_key
+
+    def get_registration_id(self) -> int:
+        return self.registration_id
+
+    def get_session_version(self) -> int:
+        public_key = self.identity_key.get_public_key()
+        if isinstance(public_key, CurvePublicKey):
             return 3
 
-        elif isinstance(publicKey, EdPublicKey):
+        elif isinstance(public_key, EdPublicKey):
             return 4
 
         else:
             breakpoint()
             raise AssertionError("Unknown session version")
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/state/prekeyrecord.py` & `omemo-dr-0.99.1/src/omemo_dr/state/signedprekeyrecord.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,48 +2,59 @@
 
 from typing import cast
 
 import google.protobuf.message
 
 from ..ecc.curve import Curve
 from ..ecc.eckeypair import ECKeyPair
-from .storageprotos_pb2 import PreKeyRecordStructure
+from .storageprotos_pb2 import SignedPreKeyRecordStructure
 
 
-class PreKeyRecord:
-    def __init__(self, structure: PreKeyRecordStructureProto) -> None:
+class SignedPreKeyRecord:
+    def __init__(self, structure: SignedPreKeyRecordStructureProto) -> None:
         self._structure = structure
 
     @classmethod
     def new(
-        cls,
-        _id: int,
-        ecKeyPair: ECKeyPair,
-    ) -> PreKeyRecord:
-        structure = cast(PreKeyRecordStructureProto, PreKeyRecordStructure())
-        structure.id = _id
-        structure.publicKey = ecKeyPair.getPublicKey().serialize()
-        structure.privateKey = ecKeyPair.getPrivateKey().serialize()
-        return cls(structure)
+        cls, _id: int, timestamp: int, ec_key_pair: ECKeyPair, signature: bytes
+    ) -> SignedPreKeyRecord:
+        record = cast(SignedPreKeyRecordStructureProto, SignedPreKeyRecordStructure())
+
+        record.id = _id
+        record.publicKey = ec_key_pair.get_public_key().serialize()
+        record.privateKey = ec_key_pair.get_private_key().serialize()
+        record.signature = signature
+        record.timestamp = timestamp
+
+        return cls(record)
 
     @classmethod
-    def from_bytes(cls, serialized: bytes) -> PreKeyRecord:
-        record = cast(PreKeyRecordStructureProto, PreKeyRecordStructure())
+    def from_bytes(cls, serialized: bytes) -> SignedPreKeyRecord:
+        record = cast(SignedPreKeyRecordStructureProto, SignedPreKeyRecordStructure())
         record.ParseFromString(serialized)
         return cls(record)
 
-    def getId(self) -> int:
+    def get_id(self) -> int:
         return self._structure.id
 
-    def getKeyPair(self):
-        publicKey = Curve.decodePoint(bytearray(self._structure.publicKey), 0)
-        privateKey = Curve.decodePrivatePoint(bytearray(self._structure.privateKey))
-        return ECKeyPair(publicKey, privateKey)
+    def get_timestamp(self) -> int:
+        return self._structure.timestamp
+
+    def get_key_pair(self) -> ECKeyPair:
+        public_key = Curve.decode_point(bytearray(self._structure.publicKey), 0)
+        private_key = Curve.decode_private_point(bytearray(self._structure.privateKey))
+
+        return ECKeyPair(public_key, private_key)
+
+    def get_signature(self) -> bytes:
+        return self._structure.signature
 
     def serialize(self) -> bytes:
         return self._structure.SerializeToString()
 
 
-class PreKeyRecordStructureProto(google.protobuf.message.Message):
+class SignedPreKeyRecordStructureProto(google.protobuf.message.Message):
     id: int
     publicKey: bytes
     privateKey: bytes
+    signature: bytes
+    timestamp: int
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/state/storageprotos_pb2.py` & `omemo-dr-0.99.1/src/omemo_dr/state/storageprotos_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.0/src/omemo_dr/util/byteutil.py` & `omemo-dr-0.99.1/src/omemo_dr/util/byteutil.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,33 +15,33 @@
                 baos.append(a)
 
         return baos
 
     @staticmethod
     def split(
         inp: bytes,
-        firstLength: int,
-        secondLength: int,
-        thirdLength: Optional[int] = None,
+        first_length: int,
+        second_length: int,
+        third_length: Optional[int] = None,
     ) -> list[bytes]:
         parts: list[bytes] = []
-        parts.append(inp[:firstLength])
-        parts.append(inp[firstLength : firstLength + secondLength])
-        if thirdLength is not None:
-            start = firstLength + secondLength
-            end = firstLength + secondLength + thirdLength
+        parts.append(inp[:first_length])
+        parts.append(inp[first_length : first_length + second_length])
+        if third_length is not None:
+            start = first_length + second_length
+            end = first_length + second_length + third_length
             parts.append(inp[start:end])
 
         return parts
 
     @staticmethod
     def trim(inp: bytes, length: int) -> bytes:
         return inp[:length]
 
     @staticmethod
-    def intsToByteHighAndLow(highValue: int, lowValue: int) -> int:
-        return ((highValue << 4 | lowValue) & 0xFF) % 256
+    def ints_to_byte_high_and_low(high_value: int, low_value: int) -> int:
+        return ((high_value << 4 | low_value) & 0xFF) % 256
 
     @staticmethod
-    def highBitsToInt(value: int) -> int:
+    def high_bits_to_int(value: int) -> int:
         bit = ord(value) if type(value) is str else value
         return (bit & 0xFF) >> 4
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr/util/keyhelper.py` & `omemo-dr-0.99.1/src/omemo_dr/util/keyhelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,85 +12,78 @@
 from ..state.prekeyrecord import PreKeyRecord
 from ..state.signedprekeyrecord import SignedPreKeyRecord
 from .medium import Medium
 
 
 class KeyHelper:
     @staticmethod
-    def generateIdentityKeyPair() -> IdentityKeyPair:
+    def generate_identity_key_pair() -> IdentityKeyPair:
         """
-        Generate an identity key pair.  Clients should only do this once,
+        Generate an identity key pair. Clients should only do this once,
         at install time.
         @return the generated IdentityKeyPair.
         """
-        keyPair = Curve.generateKeyPair()
-        publicKey = IdentityKey(keyPair.getPublicKey())
-        serialized = (
-            "0a21056e8936e8367f768a7bba008ade7cf58407bdc7a6aae293e2c"
-            "b7c06668dcd7d5e12205011524f0c15467100dd603e0d6020f4d293"
-            "edfbcd82129b14a88791ac81365c"
-        )
-        serialized = binascii.unhexlify(serialized.encode())
-        identityKeyPair = IdentityKeyPair.new(publicKey, keyPair.getPrivateKey())
-        return identityKeyPair
-        # return IdentityKeyPair.form_bytes(serialized)
+        key_pair = Curve.generate_key_pair()
+        public_key = IdentityKey(key_pair.get_public_key())
+        identity_key_pair = IdentityKeyPair.new(public_key, key_pair.get_private_key())
+        return identity_key_pair
 
     @staticmethod
-    def generateRegistrationId() -> int:
+    def generate_registration_id() -> int:
         """
         Generate a registration ID.  Clients should only do this once,
         at install time.
         """
-        regId = KeyHelper.getRandomSequence()
+        regId = KeyHelper.get_random_sequence()
         return regId
 
     @staticmethod
-    def getRandomSequence(max: int = 4294967296) -> int:
+    def get_random_sequence(max: int = 4294967296) -> int:
         size = int(math.log(max) / math.log(2)) / 8
         rand = os.urandom(int(size))
         randh = binascii.hexlify(rand)
         return int(randh, 16)
 
     @staticmethod
-    def generatePreKeys(start: int, count: int) -> list[PreKeyRecord]:
+    def generate_pre_keys(start: int, count: int) -> list[PreKeyRecord]:
         """
         Generate a list of PreKeys.  Clients should do this at install time, and
         subsequently any time the list of PreKeys stored on the server runs low.
 
         PreKey IDs are shorts, so they will eventually be repeated.
         Clients should store PreKeys in a circular buffer, so that they are
         repeated as infrequently as possible.
         """
         results: list[PreKeyRecord] = []
         start -= 1
         for i in range(0, count):
-            preKeyId = ((start + i) % (Medium.MAX_VALUE - 1)) + 1
-            results.append(PreKeyRecord.new(preKeyId, Curve.generateKeyPair()))
+            pre_key_id = ((start + i) % (Medium.MAX_VALUE - 1)) + 1
+            results.append(PreKeyRecord.new(pre_key_id, Curve.generate_key_pair()))
 
         return results
 
     @staticmethod
-    def generateSignedPreKey(
-        identityKeyPair: IdentityKeyPair, signedPreKeyId: int
+    def generate_signed_pre_key(
+        identity_key_pair: IdentityKeyPair, signed_pre_key_id: int
     ) -> SignedPreKeyRecord:
-        keyPair = Curve.generateKeyPair()
-        signature = Curve.calculateSignature(
-            identityKeyPair.getPrivateKey(), keyPair.getPublicKey().serialize()
+        key_pair = Curve.generate_key_pair()
+        signature = Curve.calculate_signature(
+            identity_key_pair.get_private_key(), key_pair.get_public_key().serialize()
         )
 
         spk = SignedPreKeyRecord.new(
-            signedPreKeyId, int(round(time.time() * 1000)), keyPair, signature
+            signed_pre_key_id, int(round(time.time() * 1000)), key_pair, signature
         )
 
         return spk
 
     @staticmethod
-    def generateSenderSigningKey() -> ECKeyPair:
-        return Curve.generateKeyPair()
+    def generate_sender_signing_key() -> ECKeyPair:
+        return Curve.generate_key_pair()
 
     @staticmethod
-    def generateSenderKey() -> bytes:
+    def generate_sender_key() -> bytes:
         return os.urandom(32)
 
     @staticmethod
-    def generateSenderKeyId() -> int:
-        return KeyHelper.getRandomSequence(2147483647)
+    def generate_sender_key_id() -> int:
+        return KeyHelper.get_random_sequence(2147483647)
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr.egg-info/PKG-INFO` & `omemo-dr-0.99.1/src/omemo_dr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.0
+Version: 0.99.1
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -712,50 +712,45 @@
 
 ## Install time
 
 At install time, a libaxolotl client needs to generate its identity keys, registration id, and
 prekeys.
 
 ```python
-    identityKeyPair = KeyHelper.generateIdentityKeyPair()
-    registrationId  = KeyHelper.generateRegistrationId()
-    preKeys         = KeyHelper.generatePreKeys(startId, 100)
-    lastResortKey   = KeyHelper.generateLastResortKey()
-    signedPreKey    = KeyHelper.generateSignedPreKey(identityKeyPair, 5)
+    identity_key_pair = KeyHelper.generate_identity_key_pair()
+    registration_id   = KeyHelper.generate_registration_id()
+    pre_keys          = KeyHelper.generate_pre_keys(start_id, 100)
+    last_resort_key   = KeyHelper.generate_last_resort_key()
+    signed_pre_key    = KeyHelper.generate_signed_pre_key(identity_key_pair, 5)
 
-    #Store identityKeyPair somewhere durable and safe.
-    #Store registrationId somewhere durable and safe.
+    #Store identity_key_pair somewhere durable and safe.
+    #Store registration_id somewhere durable and safe.
 
-    #Store preKeys in PreKeyStore.
+    #Store pre_keys in PreKeyStore.
     #Store signed prekey in SignedPreKeyStore.
 ```
 
 ## Building a session
 
-A libaxolotl client needs to implement four interfaces: IdentityKeyStore, PreKeyStore, 
-SignedPreKeyStore, and SessionStore.  These will manage loading and storing of identity, 
+A libaxolotl client needs to implement the Store interface. This will manage loading and storing of identity, 
 prekeys, signed prekeys, and session state.
 
-Once those are implemented, building a session is fairly straightforward:
+Once this is implemented, building a session is fairly straightforward:
 
 ```python
-sessionStore      = MySessionStore()
-preKeyStore       = MyPreKeyStore()
-signedPreKeyStore = MySignedPreKeyStore()
-identityStore     = MyIdentityKeyStore()
-
-# Instantiate a SessionBuilder for a remote recipientId + deviceId tuple.
-sessionBuilder = SessionBuilder(sessionStore, preKeyStore, signedPreKeyStore,
-                                                   identityStore, recipientId, deviceId)
+store      = MyStore()
+
+# Instantiate a SessionBuilder for a remote recipient_id + device_id tuple.
+session_builder = SessionBuilder(store, recipient_id, device_id)
 
 # Build a session with a PreKey retrieved from the server.
-sessionBuilder.process(retrievedPreKey)
+sessionBuilder.process(retrieved_pre_key)
 
-sessionCipher = SessionCipher(sessionStore, recipientId, deviceId)
-message       = sessionCipher.encrypt("Hello world!")
+session_cipher = SessionCipher(store, recipient_id, device_id)
+message        = session_cipher.encrypt("Hello world!")
 
 deliver(message.serialize())
 ```
 
 # Development
 
 ## Generating protobuf files
```

### Comparing `omemo-dr-0.99.0/src/omemo_dr.egg-info/SOURCES.txt` & `omemo-dr-0.99.1/src/omemo_dr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -109,20 +109,25 @@
 curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
 curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
 curve25519/curve/ed25519/nacl_sha512/blocks.c
 curve25519/curve/ed25519/nacl_sha512/hash.c
 curve25519/curve/ed25519/tests/internal_fast_tests.h
 curve25519/curve/ed25519/tests/internal_slow_tests.h
 src/omemo_dr/__init__.py
+src/omemo_dr/aes.py
+src/omemo_dr/const.py
 src/omemo_dr/exceptions.py
 src/omemo_dr/identitykey.py
 src/omemo_dr/identitykeypair.py
+src/omemo_dr/observable.py
 src/omemo_dr/py.typed
+src/omemo_dr/session.py
 src/omemo_dr/sessionbuilder.py
 src/omemo_dr/sessioncipher.py
+src/omemo_dr/structs.py
 src/omemo_dr.egg-info/PKG-INFO
 src/omemo_dr.egg-info/SOURCES.txt
 src/omemo_dr.egg-info/dependency_links.txt
 src/omemo_dr.egg-info/requires.txt
 src/omemo_dr.egg-info/top_level.txt
 src/omemo_dr/curve/__init__.py
 src/omemo_dr/ecc/__init__.py
@@ -140,41 +145,37 @@
 src/omemo_dr/protocol/omemo_keyexchange.py
 src/omemo_dr/protocol/omemo_message.py
 src/omemo_dr/protocol/omemo_pb2.py
 src/omemo_dr/protocol/prekeywhispermessage.py
 src/omemo_dr/protocol/whispermessage.py
 src/omemo_dr/protocol/whisperprotos_pb2.py
 src/omemo_dr/ratchet/__init__.py
-src/omemo_dr/ratchet/aliceaxolotlparameters.py
-src/omemo_dr/ratchet/bobaxolotlparamaters.py
+src/omemo_dr/ratchet/aliceparameters.py
+src/omemo_dr/ratchet/bobparameters.py
 src/omemo_dr/ratchet/chainkey.py
 src/omemo_dr/ratchet/ratchetingsession.py
 src/omemo_dr/ratchet/rootkey.py
 src/omemo_dr/state/__init__.py
-src/omemo_dr/state/axolotlstore.py
-src/omemo_dr/state/identitykeystore.py
 src/omemo_dr/state/prekeybundle.py
 src/omemo_dr/state/prekeyrecord.py
-src/omemo_dr/state/prekeystore.py
 src/omemo_dr/state/sessionrecord.py
 src/omemo_dr/state/sessionstate.py
-src/omemo_dr/state/sessionstore.py
 src/omemo_dr/state/signedprekeyrecord.py
-src/omemo_dr/state/signedprekeystore.py
 src/omemo_dr/state/storageprotos_pb2.py
+src/omemo_dr/state/store.py
 src/omemo_dr/util/__init__.py
 src/omemo_dr/util/byteutil.py
 src/omemo_dr/util/keyhelper.py
 src/omemo_dr/util/medium.py
 tests/__init__.py
-tests/inmemoryaxolotlstore.py
 tests/inmemoryidentitykeystore.py
 tests/inmemoryprekeystore.py
 tests/inmemorysessionstore.py
 tests/inmemorysignedprekeystore.py
+tests/inmemorystore.py
 tests/test_sessionbuilder.py
 tests/test_sessioncipher.py
 tests/test_sigs.py
 tests/kdf/__init__.py
 tests/kdf/test_hkdf.py
 tests/ratchet/__init__.py
 tests/ratchet/test_chainkey.py
```

### Comparing `omemo-dr-0.99.0/tests/inmemorysessionstore.py` & `omemo-dr-0.99.1/tests/inmemorysessionstore.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,30 @@
+from __future__ import annotations
+
 from omemo_dr.state.sessionrecord import SessionRecord
-from omemo_dr.state.sessionstore import SessionStore
 
 
-class InMemorySessionStore(SessionStore):
+class InMemorySessionStore:
     def __init__(self):
         self.sessions: dict[tuple[str, int], bytes] = {}
 
-    def loadSession(self, recipientId: str, deviceId: int) -> SessionRecord:
-        if self.containsSession(recipientId, deviceId):
-            return SessionRecord(serialized=self.sessions[(recipientId, deviceId)])
+    def load_session(self, recipient_id: str, device_id: int) -> SessionRecord:
+        if self.contains_session(recipient_id, device_id):
+            return SessionRecord(serialized=self.sessions[(recipient_id, device_id)])
         else:
             return SessionRecord()
 
-    def getSubDeviceSessions(self, recipientId: str) -> list[int]:
-        deviceIds: list[int] = []
-        for k in self.sessions.keys():
-            if k[0] == recipientId:
-                deviceIds.append(k[1])
-
-        return deviceIds
-
-    def storeSession(
-        self, recipientId: str, deviceId: int, sessionRecord: SessionRecord
+    def store_session(
+        self, recipient_id: str, device_id: int, session_record: SessionRecord
     ) -> None:
-        self.sessions[(recipientId, deviceId)] = sessionRecord.serialize()
+        self.sessions[(recipient_id, device_id)] = session_record.serialize()
 
-    def containsSession(self, recipientId: str, deviceId: int) -> bool:
-        return (recipientId, deviceId) in self.sessions
+    def contains_session(self, recipient_id: str, device_id: int) -> bool:
+        return (recipient_id, device_id) in self.sessions
 
-    def deleteSession(self, recipientId: str, deviceId: int) -> None:
-        del self.sessions[(recipientId, deviceId)]
+    def delete_session(self, recipient_id: str, device_id: int) -> None:
+        del self.sessions[(recipient_id, device_id)]
 
-    def deleteAllSessions(self, recipientId: str) -> None:
+    def delete_all_sessions(self, recipient_id: str) -> None:
         for k in self.sessions.keys():
-            if k[0] == recipientId:
+            if k[0] == recipient_id:
                 del self.sessions[k]
```

### Comparing `omemo-dr-0.99.0/tests/inmemorysignedprekeystore.py` & `omemo-dr-0.99.1/tests/inmemorysignedprekeystore.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+from __future__ import annotations
+
 from omemo_dr.exceptions import InvalidKeyIdException
 from omemo_dr.state.signedprekeyrecord import SignedPreKeyRecord
-from omemo_dr.state.signedprekeystore import SignedPreKeyStore
 
 
-class InMemorySignedPreKeyStore(SignedPreKeyStore):
+class InMemorySignedPreKeyStore:
     def __init__(self):
-        self.store = {}
+        self.store: dict[int, bytes] = {}
 
-    def loadSignedPreKey(self, signedPreKeyId):
-        if signedPreKeyId not in self.store:
+    def load_signed_pre_key(self, signed_pre_key_id: int) -> SignedPreKeyRecord:
+        if signed_pre_key_id not in self.store:
             raise InvalidKeyIdException(
-                "No such signedprekeyrecord! %s " % signedPreKeyId
+                "No such signedprekeyrecord! %s " % signed_pre_key_id
             )
 
-        return SignedPreKeyRecord.from_bytes(self.store[signedPreKeyId])
+        return SignedPreKeyRecord.from_bytes(self.store[signed_pre_key_id])
 
-    def loadSignedPreKeys(self):
-        results = []
+    def load_signed_pre_keys(self) -> list[SignedPreKeyRecord]:
+        results: list[SignedPreKeyRecord] = []
         for serialized in self.store.values():
             results.append(SignedPreKeyRecord.from_bytes(serialized))
 
         return results
 
-    def storeSignedPreKey(self, signedPreKeyId, signedPreKeyRecord):
-        self.store[signedPreKeyId] = signedPreKeyRecord.serialize()
+    def store_signed_pre_key(
+        self, signed_pre_key_id: int, signed_pre_key_record: SignedPreKeyRecord
+    ) -> None:
+        self.store[signed_pre_key_id] = signed_pre_key_record.serialize()
 
-    def containsSignedPreKey(self, signedPreKeyId):
-        return signedPreKeyId in self.store
+    def contains_signed_pre_key(self, signed_pre_key_id: int) -> bool:
+        return signed_pre_key_id in self.store
 
-    def removeSignedPreKey(self, signedPreKeyId):
-        del self.store[signedPreKeyId]
+    def remove_signed_pre_key(self, signed_pre_key_id: int) -> None:
+        del self.store[signed_pre_key_id]
```

### Comparing `omemo-dr-0.99.0/tests/kdf/test_hkdf.py` & `omemo-dr-0.99.1/tests/kdf/test_hkdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from omemo_dr.kdf.hkdf import HKDF
 
 
 class HKDFTest(unittest.TestCase):
-    def test_vectorV3(self):
+    def test_vector_v3(self):
         ikm = bytearray(
             [
                 0x0B,
                 0x0B,
                 0x0B,
                 0x0B,
                 0x0B,
@@ -95,18 +95,18 @@
                 0x87,
                 0x18,
                 0x58,
                 0x65,
             ]
         )
 
-        actualOutput = HKDF(3).deriveSecrets(ikm, info, 42, salt=salt)
-        self.assertEqual(okm, actualOutput)
+        actual_output = HKDF(3).derive_secrets(ikm, info, 42, salt=salt)
+        self.assertEqual(okm, actual_output)
 
-    def test_vectorLongV3(self):
+    def test_vector_long_v3(self):
         ikm = bytearray(
             [
                 0x00,
                 0x01,
                 0x02,
                 0x03,
                 0x04,
@@ -441,18 +441,18 @@
                 0x43,
                 0x4F,
                 0x1D,
                 0x87,
             ]
         )
 
-        actualOutput = HKDF(3).deriveSecrets(ikm, info, 82, salt=salt)
-        self.assertEqual(okm, actualOutput)
+        actual_output = HKDF(3).derive_secrets(ikm, info, 82, salt=salt)
+        self.assertEqual(okm, actual_output)
 
-    def test_vectorV3_(self):
+    def test_vector_v3_2(self):
         ikm = bytearray(
             [
                 0x0B,
                 0x0B,
                 0x0B,
                 0x0B,
                 0x0B,
@@ -561,9 +561,9 @@
                 0x99,
                 0xDA,
                 0xEB,
                 0xEC,
             ]
         )
 
-        actualOutput = HKDF(2).deriveSecrets(ikm, info, 64, salt=salt)
-        self.assertEqual(okm, actualOutput)
+        actual_output = HKDF(2).derive_secrets(ikm, info, 64, salt=salt)
+        self.assertEqual(okm, actual_output)
```

### Comparing `omemo-dr-0.99.0/tests/ratchet/test_chainkey.py` & `omemo-dr-0.99.1/tests/ratchet/test_chainkey.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from omemo_dr.kdf.hkdf import HKDF
 from omemo_dr.ratchet.chainkey import ChainKey
 
 
 class ChainKeyTest(unittest.TestCase):
-    def test_chainKeyDerivationV2(self):
+    def test_chain_key_derivation_v2(self):
         seed = bytearray(
             [
                 0x8A,
                 0xB7,
                 0x2D,
                 0x6F,
                 0x4C,
@@ -39,15 +39,15 @@
                 0x2E,
                 0x7A,
                 0xD4,
                 0x8F,
             ]
         )
 
-        messageKey = bytearray(
+        message_key = bytearray(
             [
                 0x02,
                 0xA9,
                 0xAA,
                 0x6C,
                 0x7D,
                 0xBD,
@@ -76,15 +76,15 @@
                 0x72,
                 0x4B,
                 0x84,
                 0xA7,
             ]
         )
 
-        macKey = bytearray(
+        mac_key = bytearray(
             [
                 0xBF,
                 0xBE,
                 0x5E,
                 0xFB,
                 0x60,
                 0x30,
@@ -113,15 +113,15 @@
                 0x4D,
                 0xEB,
                 0x7C,
                 0x83,
             ]
         )
 
-        nextChainKey = bytearray(
+        next_chain_key = bytearray(
             [
                 0x28,
                 0xE8,
                 0xF8,
                 0xFE,
                 0xE5,
                 0x4B,
@@ -150,16 +150,18 @@
                 0xA2,
                 0x46,
                 0xD1,
                 0x5D,
             ]
         )
 
-        chainKey = ChainKey(HKDF(2), seed, 0)
-        self.assertEqual(chainKey.getKey(), seed)
-        self.assertEqual(chainKey.getMessageKeys().getCipherKey(), messageKey)
-        self.assertEqual(chainKey.getMessageKeys().getMacKey(), macKey)
-        self.assertEqual(chainKey.getNextChainKey().getKey(), nextChainKey)
-        self.assertEqual(chainKey.getIndex(), 0)
-        self.assertEqual(chainKey.getMessageKeys().getCounter(), 0)
-        self.assertEqual(chainKey.getNextChainKey().getIndex(), 1)
-        self.assertEqual(chainKey.getNextChainKey().getMessageKeys().getCounter(), 1)
+        chain_key = ChainKey(HKDF(2), seed, 0)
+        self.assertEqual(chain_key.get_key(), seed)
+        self.assertEqual(chain_key.get_message_keys().get_cipher_key(), message_key)
+        self.assertEqual(chain_key.get_message_keys().get_mac_key(), mac_key)
+        self.assertEqual(chain_key.get_next_chain_key().get_key(), next_chain_key)
+        self.assertEqual(chain_key.get_index(), 0)
+        self.assertEqual(chain_key.get_message_keys().get_counter(), 0)
+        self.assertEqual(chain_key.get_next_chain_key().get_index(), 1)
+        self.assertEqual(
+            chain_key.get_next_chain_key().get_message_keys().get_counter(), 1
+        )
```

### Comparing `omemo-dr-0.99.0/tests/ratchet/test_ratchetingsession.py` & `omemo-dr-0.99.1/tests/test_sigs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,311 +1,388 @@
 import unittest
 
 from omemo_dr.ecc.curve import Curve
-from omemo_dr.ecc.eckeypair import ECKeyPair
-from omemo_dr.identitykey import IdentityKey
-from omemo_dr.identitykeypair import IdentityKeyPair
-from omemo_dr.ratchet.bobaxolotlparamaters import BobAxolotlParameters
-from omemo_dr.ratchet.ratchetingsession import RatchetingSession
-from omemo_dr.state.sessionstate import SessionState
+from omemo_dr.ecc.djbec import CurvePublicKey
+from omemo_dr.util.keyhelper import KeyHelper
 
 
-class RatchetingSessionTest(unittest.TestCase):
-    def test_ratchetingSessionAsBob(self):
-        bobPublic = bytearray(
+class Curve25519Test(unittest.TestCase):
+    def test_agreement(self):
+        alice_public = bytearray(
             [
                 0x05,
-                0x2C,
-                0xB4,
-                0x97,
-                0x76,
-                0xB8,
-                0x77,
-                0x02,
-                0x05,
-                0x74,
-                0x5A,
+                0x1B,
+                0xB7,
+                0x59,
+                0x66,
+                0xF2,
+                0xE9,
                 0x3A,
-                0x6E,
-                0x24,
-                0xF5,
-                0x79,
-                0xCD,
-                0xB4,
-                0xBA,
-                0x7A,
-                0x89,
-                0x04,
-                0x10,
-                0x05,
-                0x92,
-                0x8E,
-                0xBB,
-                0xAD,
-                0xC9,
+                0x36,
+                0x91,
+                0xDF,
+                0xFF,
+                0x94,
+                0x2B,
+                0xB2,
+                0xA4,
+                0x66,
+                0xA1,
                 0xC0,
-                0x5A,
-                0xD4,
-                0x58,
+                0x8B,
+                0x8D,
+                0x78,
+                0xCA,
+                0x3F,
+                0x4D,
+                0x6D,
+                0xF8,
+                0xB8,
+                0xBF,
+                0xA2,
+                0xE4,
+                0xEE,
+                0x28,
             ]
         )
-
-        bobPrivate = bytearray(
+        alice_private = bytearray(
             [
-                0xA1,
-                0xCA,
-                0xB4,
+                0xC8,
+                0x06,
+                0x43,
+                0x9D,
+                0xC9,
+                0xD2,
+                0xC4,
+                0x76,
+                0xFF,
+                0xED,
                 0x8F,
-                0x7C,
-                0x89,
-                0x3F,
-                0xAF,
-                0xA9,
+                0x25,
+                0x80,
+                0xC0,
                 0x88,
-                0x0A,
-                0x28,
-                0xC3,
+                0x8D,
+                0x58,
+                0xAB,
+                0x40,
+                0x6B,
+                0xF7,
+                0xAE,
+                0x36,
+                0x98,
+                0x87,
+                0x90,
+                0x21,
+                0xB9,
+                0x6B,
                 0xB4,
-                0x99,
-                0x9D,
-                0x28,
-                0xD6,
-                0x32,
-                0x95,
-                0x62,
-                0xD2,
-                0x7A,
-                0x4E,
-                0xA4,
-                0xE2,
-                0x2E,
-                0x9F,
-                0xF1,
-                0xBD,
-                0xD6,
-                0x5A,
+                0xBF,
+                0x59,
             ]
         )
 
-        bobIdentityPublic = bytearray(
+        bob_public = bytearray(
             [
                 0x05,
-                0xF1,
-                0xF4,
-                0x38,
-                0x74,
-                0xF6,
-                0x96,
-                0x69,
-                0x56,
-                0xC2,
-                0xDD,
-                0x47,
+                0x65,
+                0x36,
+                0x14,
+                0x99,
+                0x3D,
+                0x2B,
+                0x15,
+                0xEE,
+                0x9E,
+                0x5F,
+                0xD3,
+                0xD8,
+                0x6C,
+                0xE7,
+                0x19,
+                0xEF,
+                0x4E,
+                0xC1,
+                0xDA,
+                0xAE,
+                0x18,
+                0x86,
+                0xA8,
+                0x7B,
                 0x3F,
-                0x8F,
-                0xA1,
+                0x5F,
+                0xA9,
+                0x56,
                 0x5A,
-                0xDE,
-                0xB7,
-                0x1D,
-                0x1C,
-                0xB9,
-                0x91,
-                0xB2,
-                0x34,
-                0x16,
-                0x92,
-                0x32,
-                0x4C,
-                0xEF,
-                0xB1,
-                0xC5,
-                0xE6,
-                0x26,
+                0x27,
+                0xA2,
+                0x2F,
             ]
         )
 
-        bobIdentityPrivate = bytearray(
+        bob_private = bytearray(
             [
+                0xB0,
+                0x3B,
+                0x34,
+                0xC3,
+                0x3A,
+                0x1C,
+                0x44,
+                0xF2,
+                0x25,
+                0xB6,
+                0x62,
+                0xD2,
+                0xBF,
                 0x48,
-                0x75,
-                0xCC,
-                0x69,
-                0xDD,
-                0xF8,
-                0xEA,
-                0x07,
-                0x19,
-                0xEC,
-                0x94,
-                0x7D,
-                0x61,
-                0x08,
+                0x59,
+                0xB8,
+                0x13,
+                0x54,
                 0x11,
-                0x35,
+                0xFA,
+                0x7B,
+                0x03,
                 0x86,
-                0x8D,
+                0xD4,
                 0x5F,
-                0xD8,
-                0x01,
-                0xF0,
-                0x2C,
-                0x02,
-                0x25,
-                0xE5,
-                0x16,
-                0xDF,
-                0x21,
-                0x56,
-                0x60,
-                0x5E,
+                0xB7,
+                0x5D,
+                0xC5,
+                0xB9,
+                0x1B,
+                0x44,
+                0x66,
             ]
         )
 
-        aliceBasePublic = bytearray(
+        shared = bytearray(
             [
-                0x05,
-                0x47,
-                0x2D,
-                0x1F,
-                0xB1,
-                0xA9,
+                0x32,
+                0x5F,
+                0x23,
+                0x93,
+                0x28,
+                0x94,
+                0x1C,
+                0xED,
+                0x6E,
+                0x67,
+                0x3B,
                 0x86,
-                0x2C,
-                0x3A,
-                0xF6,
-                0xBE,
-                0xAC,
-                0xA8,
-                0x92,
-                0x02,
-                0x77,
-                0xE2,
-                0xB2,
-                0x6F,
-                0x4A,
-                0x79,
-                0x21,
-                0x3E,
-                0xC7,
-                0xC9,
+                0xBA,
+                0x41,
+                0x01,
+                0x74,
+                0x48,
+                0xE9,
+                0x9B,
+                0x64,
+                0x9A,
+                0x9C,
+                0x38,
                 0x06,
-                0xAE,
-                0xB3,
-                0x5E,
-                0x03,
-                0xCF,
-                0x89,
-                0x50,
+                0xC1,
+                0xDD,
+                0x7C,
+                0xA4,
+                0xC4,
+                0x77,
+                0xE6,
+                0x29,
             ]
         )
 
-        # aliceEphemeralPublic = bytearray([0x05, 0x6c, 0x3e, 0x0d, 0x1f, 0x52, 0x02, 0x83, 0xef, 0xcc, 0x55, 0xfc,
-        #                                   0xa5, 0xe6, 0x70, 0x75, 0xb9, 0x04, 0x00, 0x7f, 0x18, 0x81, 0xd1, 0x51,
-        #                                   0xaf, 0x76, 0xdf, 0x18, 0xc5, 0x1d, 0x29, 0xd3, 0x4b])
+        alice_public_key = Curve.decode_point(alice_public, 0)
+        assert isinstance(alice_public_key, CurvePublicKey)
+
+        alice_private_key = Curve.decode_private_point(alice_private)
 
-        aliceIdentityPublic = bytearray(
+        bob_public_key = Curve.decode_point(bob_public, 0)
+        assert isinstance(bob_public_key, CurvePublicKey)
+
+        bob_private_key = Curve.decode_private_point(bob_private)
+
+        shared_one = Curve.calculate_agreement(alice_public_key, bob_private_key)
+        shared_two = Curve.calculate_agreement(bob_public_key, alice_private_key)
+
+        self.assertEqual(shared_one, shared)
+        self.assertEqual(shared_two, shared)
+
+    def test_random_agreements(self):
+        for _i in range(0, 50):
+            alice = Curve.generate_key_pair()
+            bob = Curve.generate_key_pair()
+            shared_alice = Curve.calculate_agreement(
+                bob.get_public_key(), alice.get_private_key()
+            )
+            shared_bob = Curve.calculate_agreement(
+                alice.get_public_key(), bob.get_private_key()
+            )
+            self.assertEqual(shared_alice, shared_bob)
+
+    def test_gensig(self):
+        identity_key_pair = KeyHelper.generate_identity_key_pair()
+        KeyHelper.generate_signed_pre_key(identity_key_pair, 0)
+
+    def test_signature(self):
+        # aliceIdentityPrivate = bytearray([0xc0, 0x97, 0x24, 0x84, 0x12, 0xe5, 0x8b, 0xf0, 0x5d, 0xf4, 0x87, 0x96,
+        #                                   0x82, 0x05, 0x13, 0x27, 0x94, 0x17, 0x8e, 0x36, 0x76, 0x37, 0xf5, 0x81,
+        #                                   0x8f, 0x81, 0xe0, 0xe6, 0xce, 0x73, 0xe8, 0x65])
+
+        alice_identity_public = bytearray(
             [
                 0x05,
-                0xB4,
-                0xA8,
-                0x45,
-                0x56,
-                0x60,
-                0xAD,
-                0xA6,
-                0x5B,
-                0x40,
-                0x10,
-                0x07,
-                0xF6,
-                0x15,
-                0xE6,
-                0x54,
-                0x04,
-                0x17,
-                0x46,
-                0x43,
-                0x2E,
+                0xAB,
+                0x7E,
+                0x71,
+                0x7D,
+                0x4A,
+                0x16,
+                0x3B,
+                0x7D,
+                0x9A,
+                0x1D,
+                0x80,
+                0x71,
+                0xDF,
+                0xE9,
+                0xDC,
+                0xF8,
+                0xCD,
+                0xCD,
+                0x1C,
+                0xEA,
                 0x33,
                 0x39,
-                0xC6,
-                0x87,
-                0x51,
-                0x49,
-                0xBC,
-                0xEE,
-                0xFC,
-                0xB4,
-                0x2B,
-                0x4A,
+                0xB6,
+                0x35,
+                0x6B,
+                0xE8,
+                0x4D,
+                0x88,
+                0x7E,
+                0x32,
+                0x2C,
+                0x64,
             ]
         )
 
-        senderChain = bytearray(
+        alice_ephemeral_public = bytearray(
             [
-                0xD2,
-                0x2F,
-                0xD5,
-                0x6D,
-                0x3F,
-                0xEC,
-                0x81,
-                0x9C,
-                0xF4,
-                0xC3,
-                0xD5,
-                0x0C,
-                0x56,
+                0x05,
                 0xED,
-                0xFB,
-                0x1C,
-                0x28,
-                0x0A,
-                0x1B,
+                0xCE,
+                0x9D,
+                0x9C,
+                0x41,
+                0x5C,
+                0xA7,
+                0x8C,
+                0xB7,
+                0x25,
+                0x2E,
+                0x72,
+                0xC2,
+                0xC4,
+                0xA5,
+                0x54,
+                0xD3,
+                0xEB,
+                0x29,
+                0x48,
+                0x5A,
+                0x0E,
+                0x1D,
+                0x50,
                 0x31,
-                0x96,
-                0x45,
-                0x37,
-                0xF1,
+                0x18,
                 0xD1,
-                0x61,
-                0xE1,
-                0xC9,
-                0x31,
-                0x48,
-                0xE3,
-                0x6B,
+                0xA8,
+                0x2D,
+                0x99,
+                0xFB,
+                0x4A,
             ]
         )
 
-        bobIdentityKeyPublic = IdentityKey(bobIdentityPublic, 0)
-        bobIdentityKeyPrivate = Curve.decodePrivatePoint(bobIdentityPrivate)
-        bobIdentityKey = IdentityKeyPair.new(
-            bobIdentityKeyPublic, bobIdentityKeyPrivate
-        )
-        bobEphemeralPublicKey = Curve.decodePoint(bobPublic, 0)
-        bobEphemeralPrivateKey = Curve.decodePrivatePoint(bobPrivate)
-        bobEphemeralKey = ECKeyPair(bobEphemeralPublicKey, bobEphemeralPrivateKey)
-        bobBaseKey = bobEphemeralKey
-
-        aliceBasePublicKey = Curve.decodePoint(aliceBasePublic, 0)
-        # aliceEphemeralPublicKey = Curve.decodePoint(aliceEphemeralPublic, 0)
-        aliceIdentityPublicKey = IdentityKey(aliceIdentityPublic, 0)
-
-        parameters = (
-            BobAxolotlParameters.newBuilder()
-            .setOurIdentityKey(bobIdentityKey)
-            .setOurSignedPreKey(bobBaseKey)
-            .setOurRatchetKey(bobEphemeralKey)
-            .setOurOneTimePreKey(None)
-            .setTheirIdentityKey(aliceIdentityPublicKey)
-            .setTheirBaseKey(aliceBasePublicKey)
-            .create()
+        alice_signature = bytearray(
+            [
+                0x5D,
+                0xE8,
+                0x8C,
+                0xA9,
+                0xA8,
+                0x9B,
+                0x4A,
+                0x11,
+                0x5D,
+                0xA7,
+                0x91,
+                0x09,
+                0xC6,
+                0x7C,
+                0x9C,
+                0x74,
+                0x64,
+                0xA3,
+                0xE4,
+                0x18,
+                0x02,
+                0x74,
+                0xF1,
+                0xCB,
+                0x8C,
+                0x63,
+                0xC2,
+                0x98,
+                0x4E,
+                0x28,
+                0x6D,
+                0xFB,
+                0xED,
+                0xE8,
+                0x2D,
+                0xEB,
+                0x9D,
+                0xCD,
+                0x9F,
+                0xAE,
+                0x0B,
+                0xFB,
+                0xB8,
+                0x21,
+                0x56,
+                0x9B,
+                0x3D,
+                0x90,
+                0x01,
+                0xBD,
+                0x81,
+                0x30,
+                0xCD,
+                0x11,
+                0xD4,
+                0x86,
+                0xCE,
+                0xF0,
+                0x47,
+                0xBD,
+                0x60,
+                0xB8,
+                0x6E,
+                0x88,
+            ]
         )
 
-        session = SessionState()
+        # alice_private_key = Curve.decode_private_point(alice_identity_private)
+        alice_public_key = Curve.decode_point(alice_identity_public, 0)
+        assert isinstance(alice_public_key, CurvePublicKey)
 
-        RatchetingSession.initializeSessionAsBob(session, 2, parameters)
-        self.assertEqual(session.getLocalIdentityKey(), bobIdentityKey.getPublicKey())
-        self.assertEqual(session.getRemoteIdentityKey(), aliceIdentityPublicKey)
-        self.assertEqual(session.getSenderChainKey().getKey(), senderChain)
+        alice_ephemeral = Curve.decode_point(alice_ephemeral_public, 0)
+        assert isinstance(alice_ephemeral, CurvePublicKey)
+
+        res = Curve.verify_signature(
+            alice_public_key, alice_ephemeral.serialize(), bytes(alice_signature)
+        )
+        self.assertTrue(res)
```

### Comparing `omemo-dr-0.99.0/tests/ratchet/test_rootkey.py` & `omemo-dr-0.99.1/tests/ratchet/test_rootkey.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from omemo_dr.ecc.djbec import CurvePublicKey
 from omemo_dr.ecc.eckeypair import ECKeyPair
 from omemo_dr.kdf.hkdf import HKDF
 from omemo_dr.ratchet.rootkey import RootKey
 
 
 class RootKeyTest(unittest.TestCase):
-    def test_rootKeyDerivationV2(self):
-        rootKeySeed = bytearray(
+    def test_root_key_derivation_v2(self):
+        root_key_seed = bytearray(
             [
                 0x7B,
                 0xA6,
                 0xDE,
                 0xBC,
                 0x2B,
                 0xC1,
@@ -42,15 +42,15 @@
                 0x38,
                 0x94,
                 0x2D,
                 0xCC,
             ]
         )
 
-        alicePublic = bytearray(
+        alice_public = bytearray(
             [
                 0x05,
                 0xEE,
                 0x4F,
                 0xA6,
                 0xCD,
                 0xC0,
@@ -80,15 +80,15 @@
                 0x62,
                 0x22,
                 0xE1,
                 0x3A,
             ]
         )
 
-        alicePrivate = bytearray(
+        alice_private = bytearray(
             [
                 0x21,
                 0x68,
                 0x22,
                 0xEC,
                 0x67,
                 0xEB,
@@ -117,15 +117,15 @@
                 0x7A,
                 0x94,
                 0x8E,
                 0x50,
             ]
         )
 
-        bobPublic = bytearray(
+        bob_public = bytearray(
             [
                 0x05,
                 0xAB,
                 0xB8,
                 0xEB,
                 0x29,
                 0xCC,
@@ -155,15 +155,15 @@
                 0x57,
                 0x70,
                 0x8A,
                 0x30,
             ]
         )
 
-        nextRoot = bytearray(
+        next_root = bytearray(
             [
                 0xB1,
                 0x14,
                 0xF5,
                 0xDE,
                 0x28,
                 0x01,
@@ -192,15 +192,15 @@
                 0x12,
                 0xA2,
                 0xF7,
                 0x31,
             ]
         )
 
-        nextChain = bytearray(
+        next_chain = bytearray(
             [
                 0x9D,
                 0x7D,
                 0x24,
                 0x69,
                 0xBC,
                 0x9A,
@@ -229,24 +229,24 @@
                 0x55,
                 0xB5,
                 0xCA,
                 0x5F,
             ]
         )
 
-        alicePublicKey = Curve.decodePoint(alicePublic, 0)
-        assert isinstance(alicePublicKey, CurvePublicKey)
+        alice_public_key = Curve.decode_point(alice_public, 0)
+        assert isinstance(alice_public_key, CurvePublicKey)
 
-        alicePrivateKey = Curve.decodePrivatePoint(alicePrivate)
-        aliceKeyPair = ECKeyPair(alicePublicKey, alicePrivateKey)
-        bobPublicKey = Curve.decodePoint(bobPublic, 0)
-        assert isinstance(bobPublicKey, CurvePublicKey)
-
-        rootKey = RootKey(HKDF(2), rootKeySeed)
-        rootKeyChainKeyPair = rootKey.createChain(bobPublicKey, aliceKeyPair)
-
-        nextRootKey = rootKeyChainKeyPair[0]
-        nextChainKey = rootKeyChainKeyPair[1]
-
-        self.assertEqual(rootKey.getKeyBytes(), rootKeySeed)
-        self.assertEqual(nextRootKey.getKeyBytes(), nextRoot)
-        self.assertEqual(nextChainKey.getKey(), nextChain)
+        alice_private_key = Curve.decode_private_point(alice_private)
+        alice_key_pair = ECKeyPair(alice_public_key, alice_private_key)
+        bob_public_key = Curve.decode_point(bob_public, 0)
+        assert isinstance(bob_public_key, CurvePublicKey)
+
+        root_key = RootKey(HKDF(2), root_key_seed)
+        root_key_chain_key_pair = root_key.create_chain(bob_public_key, alice_key_pair)
+
+        next_root_key = root_key_chain_key_pair[0]
+        next_chain_key = root_key_chain_key_pair[1]
+
+        self.assertEqual(root_key.get_key_bytes(), root_key_seed)
+        self.assertEqual(next_root_key.get_key_bytes(), next_root)
+        self.assertEqual(next_chain_key.get_key(), next_chain)
```

