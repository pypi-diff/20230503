# Comparing `tmp/tomcli-0.1.0.tar.gz` & `tmp/tomcli-0.1.1.tar.gz`

## Comparing `tomcli-0.1.0.tar` & `tomcli-0.1.1.tar`

### file list

```diff
@@ -1,161 +1,467 @@
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomcli-0.1.0/NEWS.md
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 tomcli-0.1.0/noxfile.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 tomcli-0.1.0/ruff.toml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 tomcli-0.1.0/tomcli.spec
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-lint.yml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-mockbuild-36.yml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox-mockbuild.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomcli-0.1.0/.builds/nox.yml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomcli-0.1.0/.copr/Makefile
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/102ae904ce423ecb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/132a3334bcb697d4
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/138cd2ffd9a72fa1
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/16cf683684086e42
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/17032b34c3539c33
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/182adab4e5a8e026
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/191bd3e667e65878
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/195fac077159fecb
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/1cae0246f47a51e6
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/1ed1e9bc14a8e947
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/21b095e72d064d0b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/228428ef6c55f9b4
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/242872c45603caf
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/25f3447aeaf90609
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/26fd5f1a8357f894
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/2b63439cd5af3054
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/33669fbc3402d0a1
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/343c17d86941be6d
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/34e1ab478d40a9f3
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3622d24d03165106
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3bd00a94f33fcfb6
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3c9f99f371b068bd
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/3f58ceb8ff490785
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4053dc61d6f25547
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/41414cb33223f426
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4308237c7c08ba51
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4553072f09555c43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/47990969b0816c19
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4888e119c62fc817
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4a7642a70dda40d5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4d0ebeb74dea6e4b
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4dbd6c78c25046fa
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/4ee7b8cdcbae7088
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/51d60f70e1c125ab
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/52052331ac998de4
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/53b770c79f3eb823
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/550a149458063685
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/567b69da99e997a2
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/597c305794afb3f8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/60cd4b8318ff3584
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/657ba086a2498dbf
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6746594f55461582
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/674c74015bfddf43
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6786b37a5221b5ca
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6b2cd9174eb27a0b
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6b3a3867f95ee3d2
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6c2e1ccb7af019ae
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6ca2f2fc9012834d
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6e1805a0b2587263
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6e75d02f45e0b6fb
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/6fe881ef0238e47f
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/72b1b7c696d63174
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7504488c70d0af41
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/76586ca86e26121c
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/78d76edde2035610
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7a8936c6cc6300fc
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7c61d90fd1d2157e
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/7daa321bf9a53c19
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/868e7acfe2fb4ddd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8a402591edeaa7cd
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8c07c91f8542951d
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8cbb3cc218d2ac4e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/8f65f16675aa2609
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9077c3459649e893
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9121b1d341614163
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/92cc94298f42a9ca
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/92dba4109cb7630e
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/937b28c1e8bec5db
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/997ed1b7b1b436bc
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/99d43425a9401b4
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9a95a18da5948a17
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9d5dbdd0a8f1e60
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/9fb39b3a808d7699
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a27d76782310c1d1
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a29416463f58d4c8
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a86f2775c1a8a107
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/a893c04545a27cb5
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ac3bb96a02e8e6e
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b0498287d2c842b7
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b3930246cf024275
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b5d7fd139b8e8a0e
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/b92653f4ad1ae939
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bab378b835e02eca
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bb5da1dd2b74eb4a
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bbbc901adcc3cdce
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/bca2376011140193
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/c5e9cf82f769cc55
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/d16f80d852d45e0f
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/d605b54ed8ac564b
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/db1c6b1a34a124cf
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dc0a1dabe7469cc9
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dc597330036fdb6b
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/dccc2bf75292b03c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/de5d7f1c9f277e6e
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/defb66c7533f1af0
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e4f9058a88b51681
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e86563f1db503e0a
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e9947e79394d7105
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/e9a66483d5236f84
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ebc4eaabfb6b1a87
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ebc90afe0dc2f9c9
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ee43000363d5572
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ee5eab6a18e8f319
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/ef2b9c6d0e28e698
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f14acfbd1d4b990e
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f24f2f95e29bfcd4
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f4fbc527411366a3
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f7ab763b6cbfb8c
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/f91fb7119f181aad
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/fc383bcf580fd858
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.0/.ruff_cache/content/fcc03fa280ebd898
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 tomcli-0.1.0/contrib/fedoraify.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
--rw-r--r--   0        0        0    57283 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960___init___py.html
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960__util_py.html
--rw-r--r--   0        0        0    19997 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_get_py.html
--rw-r--r--   0        0        0    34226 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_set_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.1.0/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/__init__.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/toml.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/_util.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/get.py
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 tomcli-0.1.0/src/tomcli/cli/set.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_tomcli_get.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_tomcli_set.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_data/pyproject.toml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tomcli-0.1.0/tests/test_data/test1.toml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tomcli-0.1.0/.gitignore
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tomcli-0.1.0/README.md
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 tomcli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomcli-0.1.1/NEWS.md
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 tomcli-0.1.1/noxfile.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 tomcli-0.1.1/ruff.toml
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 tomcli-0.1.1/tomcli.spec
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-lint.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-mockbuild-36.yml
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-mockbuild.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomcli-0.1.1/.copr/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180407 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52439 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171970 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113968 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27348 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50468 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23375 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60715 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130451 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    57784 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   141567 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58330 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62945 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90162 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27315 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   130394 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46229 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0   322714 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85376 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266348 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0    52550 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28806 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    79021 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49237 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87503 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75236 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    40067 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167584 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71151 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28519 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49780 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27787 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   162203 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   142491 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   140364 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49134 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64754 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43644 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57057 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239671 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432441 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57905 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142967 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24308 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    89093 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47214 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    44790 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   180689 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    55966 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17583 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    33794 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    23327 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32015 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   408027 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129022 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79309 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30896 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70618 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64610 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91158 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11974 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350782 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.data.json
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.meta.json
+-rw-r--r--   0        0        0    12001 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.meta.json
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.data.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.meta.json
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.meta.json
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.meta.json
+-rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.data.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.meta.json
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.meta.json
+-rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.meta.json
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    47564 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    32954 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   220449 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    33483 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    22675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    34961 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    47747 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    56992 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    36082 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    17477 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   182183 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/102ae904ce423ecb
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/12dc023d4eeb0e37
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/132a3334bcb697d4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/138cd2ffd9a72fa1
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/16cf683684086e42
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/17032b34c3539c33
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/182adab4e5a8e026
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/191bd3e667e65878
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/195fac077159fecb
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/1cae0246f47a51e6
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/1ed1e9bc14a8e947
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/21b095e72d064d0b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/228428ef6c55f9b4
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/242872c45603caf
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/25f3447aeaf90609
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/26fd5f1a8357f894
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2b63439cd5af3054
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2b7341a8921547bd
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2ff578dfeee119ca
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/33669fbc3402d0a1
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/343c17d86941be6d
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/346d839a0caccf20
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/34e1ab478d40a9f3
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3622d24d03165106
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3bd00a94f33fcfb6
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3c9f99f371b068bd
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3f58ceb8ff490785
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4053dc61d6f25547
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/41414cb33223f426
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4308237c7c08ba51
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4553072f09555c43
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/46998819e6ff077f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/47990969b0816c19
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4888e119c62fc817
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4a7642a70dda40d5
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4cd0cccf6ffbd37f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4d0ebeb74dea6e4b
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4dbd6c78c25046fa
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4ee7b8cdcbae7088
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/50fbcc50cbc6963e
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/51d60f70e1c125ab
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/52052331ac998de4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/53b770c79f3eb823
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/550a149458063685
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/558db8308279fc8
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/567b69da99e997a2
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/597c305794afb3f8
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/59e5ebb72bd3ba47
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/5c0560476bf0f9ad
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/60cd4b8318ff3584
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/657ba086a2498dbf
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6746594f55461582
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/674c74015bfddf43
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6786b37a5221b5ca
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/68c3bf3fc39850ae
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/69bb70c63199ed7e
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6b2cd9174eb27a0b
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6b3a3867f95ee3d2
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6c2e1ccb7af019ae
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6ca2f2fc9012834d
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e1805a0b2587263
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e75d02f45e0b6fb
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e8ccc9f8483820
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6fe881ef0238e47f
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/72b1b7c696d63174
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7504488c70d0af41
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/76586ca86e26121c
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/774d1d87720a5875
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/78d76edde2035610
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7a8936c6cc6300fc
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7c61d90fd1d2157e
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7daa321bf9a53c19
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/868e7acfe2fb4ddd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8a402591edeaa7cd
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8c07c91f8542951d
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8cbb3cc218d2ac4e
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8ee62ebec18533c6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8f65f16675aa2609
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9077c3459649e893
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9121b1d341614163
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92cc94298f42a9ca
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92dba4109cb7630e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92ef05225680b6d9
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/937b28c1e8bec5db
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/997ed1b7b1b436bc
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/99c02b984716f598
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/99d43425a9401b4
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9a95a18da5948a17
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9d5dbdd0a8f1e60
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9fb39b3a808d7699
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a27d76782310c1d1
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a29416463f58d4c8
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a443eb5443fdca85
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a86f2775c1a8a107
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a893c04545a27cb5
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ac3bb96a02e8e6e
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ae8098d6ad3ba72c
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b0498287d2c842b7
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b3930246cf024275
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b5d7fd139b8e8a0e
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b92653f4ad1ae939
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bab378b835e02eca
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bb5da1dd2b74eb4a
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bbbc901adcc3cdce
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bca2376011140193
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/c5e9cf82f769cc55
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/c95bdd44d51da69b
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/cf0c578ec805a96d
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d16f80d852d45e0f
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d3122b9270693438
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d605b54ed8ac564b
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/db1c6b1a34a124cf
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/db3b51a62df336a
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dc0a1dabe7469cc9
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dc597330036fdb6b
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dca3ff05fc9331c1
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dccc2bf75292b03c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/de5d7f1c9f277e6e
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/de7a47327060d771
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/defb66c7533f1af0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e0d6034af33a507f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e41759e40bb12348
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e4f9058a88b51681
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e86563f1db503e0a
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e9947e79394d7105
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e9a66483d5236f84
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ebc4eaabfb6b1a87
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ebc90afe0dc2f9c9
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ee43000363d5572
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ee5eab6a18e8f319
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ef2b9c6d0e28e698
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f03dc93d3317a16d
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f14acfbd1d4b990e
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f24f2f95e29bfcd4
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f4fbc527411366a3
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f7743eea7895cd9a
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f7ab763b6cbfb8c
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f91fb7119f181aad
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/fc383bcf580fd858
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/fcc03fa280ebd898
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 tomcli-0.1.1/contrib/fedoraify.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
+-rw-r--r--   0        0        0    57283 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960___init___py.html
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960__util_py.html
+-rw-r--r--   0        0        0    19997 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_get_py.html
+-rw-r--r--   0        0        0    34226 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_set_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/toml.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/_util.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/get.py
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/set.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_tomcli_get.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_tomcli_set.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_data/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_data/test1.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomcli-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tomcli-0.1.1/README.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tomcli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.1.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 tomcli-0.1.1/PKG-INFO
```

### Comparing `tomcli-0.1.0/CONTRIBUTING.md` & `tomcli-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/NEWS.md` & `tomcli-0.1.1/NEWS.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/noxfile.py` & `tomcli-0.1.1/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import argparse
 import datetime
 import os
 from pathlib import Path
-from shutil import copy2
+from shutil import copy2, rmtree
 from textwrap import dedent
 
 import nox
 
 nox.options.sessions = ("formatters", "codeqa", "typing", "test")
 nox.options.error_on_external_run = True
 
@@ -70,14 +70,15 @@
     install(session, ".[all,tomli,test]", editable=True)
     session.run("pytest", "tests", *session.posargs)
 
 
 @nox.session
 def typing(session: nox.Session):
     install(session, ".[typing]", editable=True)
+    session.run("mypy", "src")
 
 
 @nox.session
 def lint(session: nox.Session):
     session.notify("formatters")
     session.notify("codeqa")
     session.notify("typing")
@@ -143,14 +144,15 @@
         session.error(f"{tag} is already tagged")
 
 
 @nox.session
 def bump(session: nox.Session):
     ensure_clean(session)
     install(session, "hatch")
+    rmtree("dist", ignore_errors=True)
 
     session.run("hatch", "version", *session.posargs)
     version = session.run("hatch", "version", silent=True).strip()
     _check_git_tag(session, version)
 
     session.run(
         "rpmdev-bumpspec",
@@ -159,14 +161,15 @@
         "--comment",
         f"Release {version}.",
         f"{PROJECT}.spec",
         external=True,
     )
 
     session.run("hatch", "build", "--clean")
+    _sign_artifacts(session)
 
     _, raw_frag_lines = add_frag(session, "FRAG.md", "NEWS.md", version)
     git_msg_file = _msg_tempfile(session, version, raw_frag_lines)
 
     session.run(
         "git",
         "add",
@@ -178,43 +181,62 @@
     session.run("git", "commit", "-S", "-m", f"Release {version}", external=True)
     ensure_clean(session)
     session.run(
         "git", "tag", "-s", "-F", git_msg_file, "--edit", f"v{version}", external=True
     )
 
 
-def _sign_artifacts(session: nox.Session) -> list[str]:
+def _sign_artifacts(session: nox.Session) -> None:
     uid = session.run("git", "config", "user.email", external=True, silent=True).strip()
     dist = Path("dist")
     artifacts = [str(p) for p in (*dist.glob("*.whl"), *dist.glob("*.tar.gz"))]
-    for path in tuple(artifacts):
-        session.run("gpg", "-u", uid, "--clearsign", path, external=True)
-        artifacts.append(f"{path}.asc")
-    return artifacts
+    for path in artifacts:
+        if Path(path + ".asc").exists():
+            session.warn(f"{path}.asc already exists. Not signing it.")
+            continue
+        session.run(
+            "gpg", "--local-user", uid, "--armor", "--detach-sign", path, external=True
+        )
 
 
 @nox.session
 def publish(session: nox.Session):
+    # Setup
     ensure_clean(session)
-    install(session, "copr", "hatch", "specfile")
-    session.run("hatch", "build", "--clean")
-    artifacts = _sign_artifacts(session)
+    install(session, "hatch")
     session.run("hatch", "publish", *session.posargs)
-    session.run("git", "push", "--follow-tags", external=True)
-    session.run("hut", "git", "artifact", "upload", *artifacts, external=True)
 
+    # Copr build
+    copr_release.func(session)
+
+    # Push to git
+    if session.interactive and input("Push to Sourcehut (Y/n)").lower() != "n":
+        git(session, "push", "--follow-tags")
+        srht_artifacts.func(session)
+
+    # Post-release bump
+    session.run("hatch", "version", "post")
+    git(session, "add", f"src/{PROJECT}/__init__.py")
+    git(session, "commit", "-S", "-m", "Post release version bump")
+
+
+@nox.session
+def copr_release(session: nox.Session):
+    install(session, "copr-cli", "requests-gssapi", "specfile")
     tmp = Path(session.create_tmp())
     dest = tmp / "tomcli.spec"
     copy2("tomcli.spec", dest)
     session.run("python", "contrib/fedoraify.py", dest)
-    session.run("copr", "build", "--nowait", "gotmax23/tomcli", str(dest))
+    session.run("copr-cli", "build", "--nowait", "gotmax23/tomcli", str(dest))
 
-    session.run("hatch", "version", "post")
-    session.run("git", "add", f"src/{PROJECT}/__init__.py", external=True)
-    session.run("git", "commit", "-S", "-m", "Post release version bump", external=True)
+
+@nox.session
+def srht_artifacts(session: nox.Session):
+    artifacts = map(str, Path("dist").glob("*"))
+    session.run("hut", "git", "artifact", "upload", *artifacts, external=True)
 
 
 @nox.session
 def srpm(session: nox.Session, posargs=None):
     posargs = posargs or session.posargs
     install_fclogr(session)
     session.run("fclogr", "--debug", "dev-srpm", *posargs)
```

### Comparing `tomcli-0.1.0/ruff.toml` & `tomcli-0.1.1/ruff.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.builds/nox-mockbuild-36.yml` & `tomcli-0.1.1/.builds/nox-mockbuild-36.yml`

 * *Files 22% similar despite different names*

```diff
@@ -15,12 +15,12 @@
   - "https://git.sr.ht/~gotmax23/tomcli"
 tasks:
   - setup: |
       pipx install nox
       sudo usermod -aG mock $USER
   - mockbuild-f36: |
       cd tomcli
-      nox -e mockbuild -- --resultdir results_tomcli -r fedora-36-x86_64
+      nox -e mockbuild -- --resultdir results_tomcli --postinstall -r fedora-36-x86_64
       tar cvf results_tomcli.tar.gz results_tomcli
   - rpmlint: |
       cd tomcli
       rpmlint results_tomcli/*.rpm
```

### Comparing `tomcli-0.1.0/.builds/nox-mockbuild.yml` & `tomcli-0.1.1/.builds/nox-mockbuild.yml`

 * *Files 3% similar despite different names*

```diff
@@ -15,12 +15,12 @@
   - "https://git.sr.ht/~gotmax23/tomcli"
 tasks:
   - setup: |
       pipx install nox
       sudo usermod -aG mock $USER
   - mockbuild-rawhide: |
       cd tomcli
-      nox -e mockbuild -- --resultdir results_tomcli -r fedora-rawhide-x86_64
+      nox -e mockbuild -- --resultdir results_tomcli --postinstall -r fedora-rawhide-x86_64
       tar cvf results_tomcli.tar.gz results_tomcli
   - rpmlint: |
       cd tomcli
       rpmlint results_tomcli/*.rpm
```

### Comparing `tomcli-0.1.0/.builds/nox.yml` & `tomcli-0.1.1/.builds/nox.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.pytest_cache/v/cache/nodeids` & `tomcli-0.1.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/17032b34c3539c33` & `tomcli-0.1.1/.ruff_cache/content/17032b34c3539c33`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/182adab4e5a8e026` & `tomcli-0.1.1/.ruff_cache/content/182adab4e5a8e026`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/191bd3e667e65878` & `tomcli-0.1.1/.ruff_cache/content/191bd3e667e65878`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/195fac077159fecb` & `tomcli-0.1.1/.ruff_cache/content/195fac077159fecb`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/1ed1e9bc14a8e947` & `tomcli-0.1.1/.ruff_cache/content/1ed1e9bc14a8e947`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/242872c45603caf` & `tomcli-0.1.1/.ruff_cache/content/242872c45603caf`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/26fd5f1a8357f894` & `tomcli-0.1.1/.ruff_cache/content/26fd5f1a8357f894`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/2b63439cd5af3054` & `tomcli-0.1.1/.ruff_cache/content/2b63439cd5af3054`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/343c17d86941be6d` & `tomcli-0.1.1/.ruff_cache/content/343c17d86941be6d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/41414cb33223f426` & `tomcli-0.1.1/.ruff_cache/content/41414cb33223f426`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/4a7642a70dda40d5` & `tomcli-0.1.1/.ruff_cache/content/4a7642a70dda40d5`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/4dbd6c78c25046fa` & `tomcli-0.1.1/.ruff_cache/content/4dbd6c78c25046fa`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/567b69da99e997a2` & `tomcli-0.1.1/.ruff_cache/content/567b69da99e997a2`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/6786b37a5221b5ca` & `tomcli-0.1.1/.ruff_cache/content/6786b37a5221b5ca`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/6ca2f2fc9012834d` & `tomcli-0.1.1/.ruff_cache/content/6ca2f2fc9012834d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/6e75d02f45e0b6fb` & `tomcli-0.1.1/.ruff_cache/content/6e75d02f45e0b6fb`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/78d76edde2035610` & `tomcli-0.1.1/.ruff_cache/content/78d76edde2035610`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/7c61d90fd1d2157e` & `tomcli-0.1.1/.ruff_cache/content/7c61d90fd1d2157e`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/7daa321bf9a53c19` & `tomcli-0.1.1/.ruff_cache/content/7daa321bf9a53c19`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/937b28c1e8bec5db` & `tomcli-0.1.1/.ruff_cache/content/937b28c1e8bec5db`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/99d43425a9401b4` & `tomcli-0.1.1/.ruff_cache/content/99c02b984716f598`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/9a95a18da5948a17` & `tomcli-0.1.1/.ruff_cache/content/9a95a18da5948a17`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/9d5dbdd0a8f1e60` & `tomcli-0.1.1/.ruff_cache/content/9d5dbdd0a8f1e60`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/a27d76782310c1d1` & `tomcli-0.1.1/.ruff_cache/content/a27d76782310c1d1`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/a86f2775c1a8a107` & `tomcli-0.1.1/.ruff_cache/content/a86f2775c1a8a107`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/a893c04545a27cb5` & `tomcli-0.1.1/.ruff_cache/content/a893c04545a27cb5`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/b3930246cf024275` & `tomcli-0.1.1/.ruff_cache/content/b3930246cf024275`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/bab378b835e02eca` & `tomcli-0.1.1/.ruff_cache/content/99d43425a9401b4`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/defb66c7533f1af0` & `tomcli-0.1.1/.ruff_cache/content/defb66c7533f1af0`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/ee5eab6a18e8f319` & `tomcli-0.1.1/.ruff_cache/content/ee5eab6a18e8f319`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/f91fb7119f181aad` & `tomcli-0.1.1/.ruff_cache/content/f03dc93d3317a16d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/.ruff_cache/content/fcc03fa280ebd898` & `tomcli-0.1.1/.ruff_cache/content/fcc03fa280ebd898`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/contrib/fedoraify.py` & `tomcli-0.1.1/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/coverage_html.js` & `tomcli-0.1.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777___init___py.html` & `tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777___init___py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html` & `tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960___init___py.html` & `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960___init___py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960__util_py.html` & `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960__util_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_get_py.html` & `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_get_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/d_1f8b6c189908f960_set_py.html` & `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_set_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/favicon_32.png` & `tomcli-0.1.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/index.html` & `tomcli-0.1.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/keybd_closed.png` & `tomcli-0.1.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/keybd_open.png` & `tomcli-0.1.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/status.json` & `tomcli-0.1.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/htmlcov/style.css` & `tomcli-0.1.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/src/tomcli/toml.py` & `tomcli-0.1.1/src/tomcli/toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import enum
 import io
 import sys
 from collections.abc import Iterator, Mapping, MutableMapping
 from contextlib import contextmanager
 from types import ModuleType
-from typing import IO, Any, BinaryIO
+from typing import IO, Any
 
 
 class Reader(enum.Enum):
     """
     Libraries to use for deserializing TOML
     """
 
@@ -29,15 +29,15 @@
 
     TOMLI_W = "tomli_w"
     TOMLKIT = "tomlkit"
 
 
 DEFAULT_READER = Reader.TOMLKIT
 DEFAULT_WRITER = Writer.TOMLKIT
-NEEDS_STR: tuple[Writer | Reader] = [Writer.TOMLKIT]
+NEEDS_STR: tuple[Writer | Reader, ...] = (Writer.TOMLKIT,)
 
 AVAILABLE_READERS: dict[Reader, ModuleType] = {}
 AVAILABLE_WRITERS: dict[Writer, ModuleType] = {}
 
 if sys.version_info[:2] >= (3, 11):
     import tomllib
 
@@ -63,29 +63,29 @@
     pass
 else:
     AVAILABLE_READERS[Reader.TOMLKIT] = tomlkit
     AVAILABLE_WRITERS[Writer.TOMLKIT] = tomlkit
 
 
 @contextmanager
-def _get_stream(fp: BinaryIO, backend: Reader | Writer) -> Iterator[IO[Any]]:
+def _get_stream(fp: IO[bytes], backend: Reader | Writer) -> Iterator[IO[Any]]:
     if backend in NEEDS_STR:
         fp.flush()
         wrapper = io.TextIOWrapper(fp, "utf-8")
         try:
             yield wrapper
         finally:
             wrapper.flush()
             wrapper.detach()
     else:
         yield fp
 
 
 def load(
-    __fp: BinaryIO,
+    __fp: IO[bytes],
     prefered_reader: Reader | None = None,
     allow_fallback: bool = True,
 ) -> MutableMapping[str, Any]:
     """
     Parse a bytes stream containing TOML data
 
     Parameters:
@@ -116,15 +116,15 @@
     else:
         txt = __fp.read().decode("utf-8")
         return mod.loads(txt)
 
 
 def dump(
     __data: Mapping[str, Any],
-    __fp: BinaryIO,
+    __fp: IO[bytes],
     prefered_writer: Writer | None = None,
     allow_fallback: bool = True,
 ) -> None:
     """
     Serialize an object to TOML and write it to a binary stream
 
     Parameters:
```

### Comparing `tomcli-0.1.0/src/tomcli/cli/get.py` & `tomcli-0.1.1/src/tomcli/cli/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 import sys
 from collections.abc import Mapping, MutableMapping
 from typing import Any, Optional
 
-from typer import Argument, Exit, Typer
+from typer import Argument, Typer
 
 from tomcli.cli._util import _std_cm
 from tomcli.toml import Reader, Writer, dump, load
 
 app = Typer(context_settings=dict(help_option_names=["-h", "--help"]))
 
 
@@ -27,27 +27,28 @@
     idx = 0
     try:
         for idx, part in enumerate(parts):  # noqa: B007
             cur = cur[part]
     except (IndexError, KeyError):
         up_to = ".".join(parts[: idx + 1])
         msg = f"Invalid selector {selector!r}: could not find {up_to!r}"
-        raise Exit(msg) from None
+        sys.exit(msg)
     return cur
 
 
 @app.command()
 def get(
     path: str = Argument(...),
     selector: str = Argument("."),
     reader: Optional[Reader] = None,
     writer: Optional[Writer] = None,
 ):
-    allow_fallback_r = bool(reader)
-    allow_fallback_w = bool(writer)
+    # Allow fallback if options are not passed
+    allow_fallback_r = not bool(reader)
+    allow_fallback_w = not bool(writer)
     reader = reader or Reader.TOMLKIT
     writer = writer or Writer.TOMLKIT
     with _std_cm(path, sys.stdin.buffer, "rb") as fp:
         data = load(fp, reader, allow_fallback_r)
     selected = get_part(data, selector)
     if isinstance(selected, Mapping):
         dump(selected, sys.stdout.buffer, writer, allow_fallback_w)
```

### Comparing `tomcli-0.1.0/src/tomcli/cli/set.py` & `tomcli-0.1.1/src/tomcli/cli/set.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 
 import dataclasses
 import operator
 import sys
 from collections.abc import Callable, Mapping, MutableMapping, MutableSequence
 from typing import Any, List, Optional, TypeVar
 
-from typer import Argument, Context, Exit, Option, Typer
+if sys.version_info >= (3, 10):
+    from types import EllipsisType
+else:
+    EllipsisType = type(Ellipsis)
+
+from typer import Argument, Context, Option, Typer
 
 from tomcli.cli._util import _std_cm
 from tomcli.toml import Reader, Writer, dump, load
 
 app = Typer(context_settings=dict(help_option_names=["-h", "--help"]))
 
 SELECTOR_HELP = (
@@ -25,16 +30,16 @@
 )
 
 
 @dataclasses.dataclass()
 class ModderCtx:
     path: str
     out: str
-    reader: str | None = None
-    writer: str | None = None
+    reader: Reader | None = None
+    writer: Writer | None = None
     allow_fallback_r: bool = True
     allow_fallback_w: bool = True
 
     def set_default_rw(self, reader: Reader, writer: Writer):
         if self.reader is None:
             self.reader = reader
         else:
@@ -77,15 +82,15 @@
 def delete(
     ctx: Context,
     selector: str = Argument(..., help=SELECTOR_HELP),
 ):
     """
     Delete a value from a TOML file.
     """
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     fun_msg = "Thank you for your patronage, but we won't delete the whole file."
     set_type(
         callback=operator.delitem, fun_msg=fun_msg, modder=modder, selector=selector
     )
 
 
@@ -94,23 +99,22 @@
     ctx: Context,
     selector: str = Argument(..., help=SELECTOR_HELP),
     value: str = Argument(...),
 ):
     """
     Set a string value in a TOML file
     """
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     fun_msg = (
         "Your heart is in the right place,"
         " but we can't replace the whole file with a string"
     )
     return set_type(
         typ=str,
-        callback=operator.setitem,
         default=dict,
         fun_msg=fun_msg,
         modder=modder,
         selector=selector,
         value=value,
     )
 
@@ -124,38 +128,39 @@
     """
     Set an integer value in a TOML file
     """
     fun_msg = (
         "Go outside and contemplate your choice"
         " to replace the whole file with integer."
     )
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
+    final: Any = value
     if "." in value:
-        value = round(float(value))
+        final = round(float(value))
     return set_type(
         typ=int,
         default=dict,
         fun_msg=fun_msg,
         modder=modder,
         selector=selector,
-        value=value,
+        value=final,
     )
 
 
 @app.command(name="float")
 def float_(ctx: Context, selector: str = Argument(...), value: float = Argument(...)):
     """
     Set a float value in a TOML file
     """
     fun_msg = (
         "I'll be very sad if you replace the whole TOML file with a string."
         " Computers have feelings too, ya know."
     )
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     return set_type(
         typ=float,
         default=dict,
         fun_msg=fun_msg,
         modder=modder,
         selector=selector,
@@ -164,15 +169,15 @@
 
 
 @app.command(name="list")
 def lst(ctx: Context, selector: str = Argument(...), value: List[str] = Argument(...)):
     """
     Create a list of strings in a TOML file
     """
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     fun_msg = (
         "A list is not a Mapping and therefore can't be the root."
         " Better luck next time!"
     )
     return set_type(
         # `value` should be a List[str], but typer passes a Tuple[str] :shrug:
@@ -188,48 +193,48 @@
 @app.command()
 def append(
     ctx: Context, selector: str = Argument(...), value: List[str] = Argument(...)
 ):
     """
     Append strings to an existing list in a TOML file
     """
-    modder: ModderCtx = ctx.find_object(ModderCtx)
+    modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     return set_type(
         fun_msg=None,
         modder=modder,
         selector=selector,
         value=value,
         callback=_append_callback,
     )
 
 
 def _append_callback(cur: MutableMapping[str, Any], part: str, value: list[Any]):
     lst = cur.get(part)
     if not isinstance(lst, MutableSequence):
-        raise Exit(
+        sys.exit(
             "You can only append values to an existing list."
             " Use the 'list' subcommand to create a new list"
         )
     lst.extend(value)
 
 
 T = TypeVar("T")
 
 
 def set_type(
     *,
     typ: Callable[[Any], T] = lambda x: x,
     callback: Callable[[MutableMapping[str, Any], str, T], Any]
     | Callable[[MutableMapping[str, Any], str], Any] = operator.setitem,
-    default: Callable[[], Any] | Ellipsis = ...,
+    default: Callable[[], Any] | EllipsisType = ...,
     fun_msg: str | None = "Invalid selector: '.'",
     modder: ModderCtx,
     selector: str,
-    value: str | Ellipsis = ...,
+    value: Any = ...,
 ):
     """
     Iterate over a TOML file based on a dot-separated selector and preform on
     operation.
 
     Parameters:
         typ:
@@ -258,26 +263,26 @@
 
     """
     data = modder.load()
     cur = data
     parts = selector.split(".")
     if selector == ".":
         if fun_msg:
-            raise Exit(fun_msg)
+            sys.exit(fun_msg)
         else:
             cur = {"data": cur}
             parts = ["data"]
     idx = 0
     for idx, part in enumerate(parts):
         if idx + 1 == len(parts):
             break
         if part not in cur and default is not ...:
             cur[part] = default()
         else:
             cur = cur[part]
     if value is ...:
-        callback(cur, part)
+        callback(cur, part)  # type: ignore[call-arg]
     else:
-        callback(cur, part, typ(value))
+        callback(cur, part, typ(value))  # type: ignore[call-arg]
     if selector == ".":
         data = data["data"]
     modder.dump(data)
```

### Comparing `tomcli-0.1.0/tests/conftest.py` & `tomcli-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/tests/test_tomcli_get.py` & `tomcli-0.1.1/tests/test_tomcli_get.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/tests/test_tomcli_set.py` & `tomcli-0.1.1/tests/test_tomcli_set.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/tests/test_data/pyproject.toml` & `tomcli-0.1.1/tests/test_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/README.md` & `tomcli-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/tomcli/commits/main.svg)](https://builds.sr.ht/~gotmax23/tomcli/commits/main?)
 
 [![copr build status][badge-copr]][link-copr] (gotmax23/tomcli)
 
 [![copr build status][badge-copr-dev]][link-copr-dev] (gotmax23/tomcli-dev)
 
 
-CLI for modifying toml files. Pronounced "tohm-clee."
+CLI for modifying toml files. Pronounced "tom clee."
 
 ## Links
 
 - [tomcli project hub](https://sr.ht/~gotmax23/tomcli)
 - [tomcli git.sr.ht repo](https://git.sr.ht/~gotmax23/tomcli)
 - [tomcli tracker](https://todo.sr.ht/~gotmax23/tomcli)
 - [tomcli mailing list][archives] ([~gotmax/tomcli@lists.sr.ht][mailto])
```

### Comparing `tomcli-0.1.0/pyproject.toml` & `tomcli-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tomcli"
 dynamic = ["version"]
-description = 'CLI for working with TOML files. Pronounced "tohm-clee."'
+description = 'CLI for working with TOML files. Pronounced "tom clee."'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 license-files.globs = ["LICENSES/*.txt"]
 authors = [
   { name = "Maxwell G", email = "maxwell@gtmx.me" },
 ]
@@ -54,14 +54,16 @@
     "reuse",
 ]
 formatters = [
     "black",
     "ruff",
 ]
 typing = [
+    "tomcli[tomli]",
+    "tomcli[tomlkit]",
     "mypy",
 ]
 test = [
     "pytest",
 ]
 dev = [
     "tomcli[all]",
```

### Comparing `tomcli-0.1.0/LICENSES/MIT.txt` & `tomcli-0.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.0/PKG-INFO` & `tomcli-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tomcli
-Version: 0.1.0
-Summary: CLI for working with TOML files. Pronounced "tohm-clee."
+Version: 0.1.1
+Summary: CLI for working with TOML files. Pronounced "tom clee."
 Project-URL: Source code, https://git.sr.ht/~gotmax23/tomcli
 Project-URL: Mailing list, https://lists.sr.ht/~gotmax23/tomcli
 Author-email: Maxwell G <maxwell@gtmx.me>
 License-Expression: MIT
 License-File: LICENSES/MIT.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -40,14 +40,16 @@
 Provides-Extra: tomli
 Requires-Dist: tomli-w; extra == 'tomli'
 Requires-Dist: tomli; python_version < '3.11' and extra == 'tomli'
 Provides-Extra: tomlkit
 Requires-Dist: tomlkit; extra == 'tomlkit'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
+Requires-Dist: tomcli[tomli]; extra == 'typing'
+Requires-Dist: tomcli[tomlkit]; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 
 SPDX-License-Identifier: MIT
 -->
@@ -57,15 +59,15 @@
 [![builds.sr.ht status](https://builds.sr.ht/~gotmax23/tomcli/commits/main.svg)](https://builds.sr.ht/~gotmax23/tomcli/commits/main?)
 
 [![copr build status][badge-copr]][link-copr] (gotmax23/tomcli)
 
 [![copr build status][badge-copr-dev]][link-copr-dev] (gotmax23/tomcli-dev)
 
 
-CLI for modifying toml files. Pronounced "tohm-clee."
+CLI for modifying toml files. Pronounced "tom clee."
 
 ## Links
 
 - [tomcli project hub](https://sr.ht/~gotmax23/tomcli)
 - [tomcli git.sr.ht repo](https://git.sr.ht/~gotmax23/tomcli)
 - [tomcli tracker](https://todo.sr.ht/~gotmax23/tomcli)
 - [tomcli mailing list][archives] ([~gotmax/tomcli@lists.sr.ht][mailto])
```

