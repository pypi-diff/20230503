# Comparing `tmp/autobisect-7.0.0.tar.gz` & `tmp/autobisect-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobisect-7.0.0.tar", max compression
+gzip compressed data, was "autobisect-7.0.1.tar", max compression
```

## Comparing `autobisect-7.0.0.tar` & `autobisect-7.0.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     4521 2023-04-25 18:11:34.125100 autobisect-7.0.0/README.md
--rw-r--r--   0        0        0      299 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/__init__.py
--rw-r--r--   0        0        0      277 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/__main__.py
--rw-r--r--   0        0        0     7153 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/args.py
--rw-r--r--   0        0        0    13922 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/bisect.py
--rw-r--r--   0        0        0     5959 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/build_manager.py
--rw-r--r--   0        0        0     3249 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/builds.py
--rw-r--r--   0        0        0     2226 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/config.py
--rw-r--r--   0        0        0      463 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/__init__.py
--rw-r--r--   0        0        0      815 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/base.py
--rw-r--r--   0        0        0      326 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/browser/__init__.py
--rw-r--r--   0        0        0     2192 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/browser/args.py
--rw-r--r--   0        0        0     6681 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/browser/browser.py
--rw-r--r--   0        0        0     4006 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/browser/tests/test_browser.py
--rw-r--r--   0        0        0      301 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/js/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/js/args.py
--rw-r--r--   0        0        0     5698 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/evaluators/js/js.py
--rw-r--r--   0        0        0     2532 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/main.py
--rw-r--r--   0        0        0        0 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/py.typed
--rw-r--r--   0        0        0        0 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/__init__.py
--rw-r--r--   0        0        0     4260 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/conftest.py
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.008852b3720d717dbb5c2c3268837e003baf72cf.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.09417381f879bb25928ca2e3bddfde157666a722.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.155e5d7c120c3e7b48685d24816bd92908014613.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.18efdddf6b5ade243f120487fe0a9375f75b2a48.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.2ad74aa6c596c2584a31dd3e502c91a2c200c23f.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.3c2625208e78720b39f2400f8e52820c1af9f507.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.42a4d256fbaa5b2dfccdc80e49f8862f5eeff8c8.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.66a1c07a8f48c5129aa3867813bacb6e7ef22d8c.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.67c8a4956e065a37ea85a504927e0e2037a7a454.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.74409a2d82fcf72799767766b758e9a28b0eaa5e.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.7e9830f213c8606a30d7c4f6cdc248e1e1041a39.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.8797c178f38e76de44782ec64f92e6ea3ff9bd49.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.963bed108e6206bf23b4d27d5bd029b1a6160c81.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.97679241a74427fed1303acde9202aaa7919a23b.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.9900a5f694580852cc09cfd516055a6337a25acc.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.a1266665b89b04eaa8c146d0bc91b512945423cb.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.cc25ed1a4d2156de782901bb85ffebb94176fc52.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.d33c1e0b18ab78924d4d74cf4fd72459faafb6d3.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.d9b16aa53c9caa4fbb3d6f9db0e375c34af212ea.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.dc4b649e269db28071eca9c885fc60cef07af585.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.ea5efd3adfb30d7db5520a67cdf6a097621df091.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.f6cf3ca2de50275ee4c885d85ae49a5e82419370.firefox.linux64-opt
--rw-r--r--   0        0        0      223 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.f7760b1404451ec4a3565c57d4e238e01c0db4b2.firefox.linux64-opt
--rw-r--r--   0        0        0      197 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.125100 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     7688 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/.get
--rw-r--r--   0        0        0     1013 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.json
--rw-r--r--   0        0        0      908 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     6731 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/.get
--rw-r--r--   0        0        0      981 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.json
--rw-r--r--   0        0        0      958 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.mozinfo.json
--rw-r--r--   0        0        0     1310 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=03ed5ed6cba7&tochange=a1266665b89b
--rw-r--r--   0        0        0     9353 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=385f49adaf00&tochange=590613078c74
--rw-r--r--   0        0        0     8675 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/test_bisect.py
--rw-r--r--   0        0        0     5574 2023-04-25 18:11:34.129101 autobisect-7.0.0/autobisect/tests/test_build_manager.py
--rw-r--r--   0        0        0     2143 2023-04-25 18:11:34.133101 autobisect-7.0.0/autobisect/tests/test_builds.py
--rw-r--r--   0        0        0     1930 2023-04-25 18:11:34.133101 autobisect-7.0.0/autobisect/tests/test_config.py
--rw-r--r--   0        0        0     3023 2023-04-25 18:11:46.265997 autobisect-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 autobisect-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4521 2023-05-03 15:04:01.865329 autobisect-7.0.1/README.md
+-rw-r--r--   0        0        0      299 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/__main__.py
+-rw-r--r--   0        0        0     7153 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/args.py
+-rw-r--r--   0        0        0    13922 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/bisect.py
+-rw-r--r--   0        0        0     5959 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/build_manager.py
+-rw-r--r--   0        0        0     3249 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/builds.py
+-rw-r--r--   0        0        0     2226 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/config.py
+-rw-r--r--   0        0        0      463 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/__init__.py
+-rw-r--r--   0        0        0      815 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/base.py
+-rw-r--r--   0        0        0      326 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/browser/__init__.py
+-rw-r--r--   0        0        0     2192 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/browser/args.py
+-rw-r--r--   0        0        0     6681 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/browser/browser.py
+-rw-r--r--   0        0        0     4006 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/browser/tests/test_browser.py
+-rw-r--r--   0        0        0      301 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/js/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/js/args.py
+-rw-r--r--   0        0        0     5698 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/evaluators/js/js.py
+-rw-r--r--   0        0        0     2532 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/main.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/py.typed
+-rw-r--r--   0        0        0        0 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/__init__.py
+-rw-r--r--   0        0        0     4260 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/conftest.py
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.008852b3720d717dbb5c2c3268837e003baf72cf.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.09417381f879bb25928ca2e3bddfde157666a722.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.155e5d7c120c3e7b48685d24816bd92908014613.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.18efdddf6b5ade243f120487fe0a9375f75b2a48.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.2ad74aa6c596c2584a31dd3e502c91a2c200c23f.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.3c2625208e78720b39f2400f8e52820c1af9f507.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.42a4d256fbaa5b2dfccdc80e49f8862f5eeff8c8.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.66a1c07a8f48c5129aa3867813bacb6e7ef22d8c.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.67c8a4956e065a37ea85a504927e0e2037a7a454.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.74409a2d82fcf72799767766b758e9a28b0eaa5e.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.7e9830f213c8606a30d7c4f6cdc248e1e1041a39.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.8797c178f38e76de44782ec64f92e6ea3ff9bd49.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.963bed108e6206bf23b4d27d5bd029b1a6160c81.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.97679241a74427fed1303acde9202aaa7919a23b.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.9900a5f694580852cc09cfd516055a6337a25acc.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.a1266665b89b04eaa8c146d0bc91b512945423cb.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.cc25ed1a4d2156de782901bb85ffebb94176fc52.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.d33c1e0b18ab78924d4d74cf4fd72459faafb6d3.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.d9b16aa53c9caa4fbb3d6f9db0e375c34af212ea.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.dc4b649e269db28071eca9c885fc60cef07af585.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.ea5efd3adfb30d7db5520a67cdf6a097621df091.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.f6cf3ca2de50275ee4c885d85ae49a5e82419370.firefox.linux64-opt
+-rw-r--r--   0        0        0      223 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.autoland.revision.f7760b1404451ec4a3565c57d4e238e01c0db4b2.firefox.linux64-opt
+-rw-r--r--   0        0        0      197 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.865329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     7688 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/.get
+-rw-r--r--   0        0        0     1013 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      908 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     6731 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/.get
+-rw-r--r--   0        0        0      981 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.json
+-rw-r--r--   0        0        0      958 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.mozinfo.json
+-rw-r--r--   0        0        0     1310 2023-05-03 15:04:01.869329 autobisect-7.0.1/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=03ed5ed6cba7&tochange=a1266665b89b
+-rw-r--r--   0        0        0     9353 2023-05-03 15:04:01.873329 autobisect-7.0.1/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=385f49adaf00&tochange=590613078c74
+-rw-r--r--   0        0        0     8675 2023-05-03 15:04:01.873329 autobisect-7.0.1/autobisect/tests/test_bisect.py
+-rw-r--r--   0        0        0     5574 2023-05-03 15:04:01.873329 autobisect-7.0.1/autobisect/tests/test_build_manager.py
+-rw-r--r--   0        0        0     2143 2023-05-03 15:04:01.873329 autobisect-7.0.1/autobisect/tests/test_builds.py
+-rw-r--r--   0        0        0     1930 2023-05-03 15:04:01.873329 autobisect-7.0.1/autobisect/tests/test_config.py
+-rw-r--r--   0        0        0     3023 2023-05-03 15:04:12.158326 autobisect-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 autobisect-7.0.1/PKG-INFO
```

### Comparing `autobisect-7.0.0/README.md` & `autobisect-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/args.py` & `autobisect-7.0.1/autobisect/args.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/bisect.py` & `autobisect-7.0.1/autobisect/bisect.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/build_manager.py` & `autobisect-7.0.1/autobisect/build_manager.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/builds.py` & `autobisect-7.0.1/autobisect/builds.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/config.py` & `autobisect-7.0.1/autobisect/config.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/base.py` & `autobisect-7.0.1/autobisect/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/browser/args.py` & `autobisect-7.0.1/autobisect/evaluators/browser/args.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/browser/browser.py` & `autobisect-7.0.1/autobisect/evaluators/browser/browser.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/browser/tests/test_browser.py` & `autobisect-7.0.1/autobisect/evaluators/browser/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/js/args.py` & `autobisect-7.0.1/autobisect/evaluators/js/args.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/evaluators/js/js.py` & `autobisect-7.0.1/autobisect/evaluators/js/js.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/main.py` & `autobisect-7.0.1/autobisect/main.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/conftest.py` & `autobisect-7.0.1/autobisect/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/BfFeMY14Qyu_rMA2pxfZZg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/DYaFBxzITgCwBUp48Bugtw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/EYhOnvRFQd-rMlW2oAl10A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/FnPonlT1QVSw-B0M0KcotQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/H5Dl5ijpSpOPwMLEEWx_bA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HFsFsbogQ0O-sFZoYDmAZw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HNaxi6w_RQeXGb4fYQFtwA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HPE2LlTUQU62unXX8GvNGA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/HX3oSg_SRTq5-Mc5D0PPHg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Hq2DMUk6QP26axMV8fDi9w/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/JucwusRxQHKQwDUPoOJIhQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/NKFp2FPpQ06E8C7N30JPdw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/O1Sh28LhQC62SfLAi0orxg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/R2zRDt-ATf-zE-hYXR8kEw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/SDAzDRggRPOPYHEQC4WDEw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Tp5LesydQWyPNqpMThZLyg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/TxMd0rIfQKucR6p0gkaMSw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/UXVT--1qQfeaGtNICDKx3w/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/WLcjhVjtTLW0A_ued1Io-Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/YDdWsEINSIyrct5ZV_nGzQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/Zb_1byPDSTyhUkZeCg-PZg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cRT3ROAzReG2wv7PW08JMg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/cSP0vuVWTX6JspZ2VTtDdg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/.get` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.mozinfo.json` & `autobisect-7.0.1/autobisect/tests/mock-firefoxci/api/queue/v1/task/fXYHDLC_RkWNtOv01aB8wQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=03ed5ed6cba7&tochange=a1266665b89b` & `autobisect-7.0.1/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=03ed5ed6cba7&tochange=a1266665b89b`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=385f49adaf00&tochange=590613078c74` & `autobisect-7.0.1/autobisect/tests/mock-hg/mozilla-central/json-pushes?fromchange=385f49adaf00&tochange=590613078c74`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/test_bisect.py` & `autobisect-7.0.1/autobisect/tests/test_bisect.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/test_build_manager.py` & `autobisect-7.0.1/autobisect/tests/test_build_manager.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/test_builds.py` & `autobisect-7.0.1/autobisect/tests/test_builds.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/autobisect/tests/test_config.py` & `autobisect-7.0.1/autobisect/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `autobisect-7.0.0/pyproject.toml` & `autobisect-7.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 license = "MPL-2.0"
 maintainers = [
     "Mozilla Fuzzing Team <fuzzing@mozilla.com>"
 ]
 name = "autobisect"
 readme = "README.md"
 repository = "https://github.com/MozillaSecurity/autobisect"
-version = "7.0.0"
+version = "7.0.1"
 
 [tool.poetry.dependencies]
 fuzzfetch = "^2.0.0"
 grizzly-framework = "^0.16.5"
 lithium-reducer = "^0.6.2"
 python = "^3.8"
```

### Comparing `autobisect-7.0.0/PKG-INFO` & `autobisect-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobisect
-Version: 7.0.0
+Version: 7.0.1
 Summary: Automatic bisection utility for Mozilla Firefox and SpiderMonkey
 Home-page: https://github.com/MozillaSecurity/autobisect
 License: MPL-2.0
 Keywords: fuzz,fuzzing,security,test,testing,bisection
 Author: Jason Kratzer
 Author-email: jkratzer@mozilla.com
 Maintainer: Mozilla Fuzzing Team
```

