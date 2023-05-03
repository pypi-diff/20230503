# Comparing `tmp/qcs_sdk_python-0.5.0rc5.tar.gz` & `tmp/qcs_sdk_python-0.5.0rc6.tar.gz`

## Comparing `qcs_sdk_python-0.5.0rc5.tar` & `qcs_sdk_python-0.5.0rc6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/Cargo.toml
--rw-r--r--   0      501       20    13160 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/CHANGELOG.md
--rw-r--r--   0      501       20      629 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/Makefile.toml
--rw-r--r--   0      501       20     2186 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/README.md
--rw-r--r--   0      501       20      562 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/delayed_job_retrieval.rs
--rw-r--r--   0      501       20      444 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/execute.rs
--rw-r--r--   0      501       20      459 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/local.rs
--rw-r--r--   0      501       20     2140 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/parametric_compilation.rs
--rw-r--r--   0      501       20     1135 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/quil_t.rs
--rw-r--r--   0      501       20    13410 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/api.rs
--rw-r--r--   0      501       20    27184 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/executable.rs
--rw-r--r--   0      501       20     7451 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/execution_data.rs
--rw-r--r--   0      501       20     1707 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/lib.rs
--rw-r--r--   0      501       20     7619 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/client.rs
--rw-r--r--   0      501       20     8497 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/execution.rs
--rw-r--r--   0      501       20     1195 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/mod.rs
--rw-r--r--   0      501       20     8348 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/edge.rs
--rw-r--r--   0      501       20     6825 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/mod.rs
--rw-r--r--   0      501       20     8419 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/operator.rs
--rw-r--r--   0      501       20    11917 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/qubit.rs
--rw-r--r--   0      501       20     9358 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/mod.rs
--rw-r--r--   0      501       20    16899 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/rewrite_arithmetic.rs
--rw-r--r--   0      501       20     7240 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/rpcq.rs
--rw-r--r--   0      501       20     8231 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/runner.rs
--rw-r--r--   0      501       20     1399 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/translation.rs
--rw-r--r--   0      501       20     6987 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qvm/execution.rs
--rw-r--r--   0      501       20     2355 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qvm/mod.rs
--rw-r--r--   0      501       20     1504 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/register_data.rs
--rw-r--r--   0      501       20   104426 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/aspen_9_isa.json
--rw-r--r--   0      501       20     1246 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/basic_qvm.rs
--rw-r--r--   0      501       20      558 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/bell_state_response_data.hex
--rw-r--r--   0      501       20    81629 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/compiler-isa-Aspen-8.json
--rw-r--r--   0      501       20    11089 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/mocked_qpu.rs
--rw-r--r--   0      501       20     1433 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/parametric_compilation.rs
--rw-r--r--   0      501       20    71490 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/qcs-isa-Aspen-8.json
--rw-r--r--   0      501       20     2275 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/qvm_isa.json
--rw-r--r--   0      501       20      148 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/secrets.toml
--rw-r--r--   0      501       20      298 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/settings.toml
--rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc5/Cargo.toml
--rw-r--r--   0      501       20    10939 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/CHANGELOG.md
--rw-r--r--   0      501       20      539 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/Makefile.toml
--rw-r--r--   0      501       20      613 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/README.md
--rw-r--r--   0      501       20       71 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/build.rs
--rw-r--r--   0      501       20     6538 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/poetry.lock
--rw-r--r--   0      501       20     1643 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/pyproject.toml
--rw-r--r--   0      501       20      155 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/__init__.py
--rw-r--r--   0      501       20      527 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/__init__.pyi
--rw-r--r--   0      501       20     2636 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/_executable.pyi
--rw-r--r--   0      501       20     2065 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/_execution_data.pyi
--rw-r--r--   0      501       20     1783 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/_register_data.pyi
--rw-r--r--   0      501       20    12838 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/api.pyi
--rw-r--r--   0      501       20        0 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/py.typed
--rw-r--r--   0      501       20       41 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/__init__.pyi
--rw-r--r--   0      501       20     2129 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/client.pyi
--rw-r--r--   0      501       20    10811 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/isa.pyi
--rw-r--r--   0      501       20      601 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/quilc.pyi
--rw-r--r--   0      501       20     9215 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/api.rs
--rw-r--r--   0      501       20     4540 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/executable.rs
--rw-r--r--   0      501       20     1708 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/execution_data.rs
--rw-r--r--   0      501       20       16 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/grpc/mod.rs
--rw-r--r--   0      501       20     2040 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/grpc/models/controller.rs
--rw-r--r--   0      501       20       20 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/grpc/models/mod.rs
--rw-r--r--   0      501       20     1125 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/lib.rs
--rw-r--r--   0      501       20     6143 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/qpu/client.rs
--rw-r--r--   0      501       20     4441 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/qpu/isa.rs
--rw-r--r--   0      501       20      462 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/qpu/mod.rs
--rw-r--r--   0      501       20     1028 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/qpu/quilc/mod.rs
--rw-r--r--   0      501       20      387 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/src/register_data.rs
--rw-r--r--   0      501       20     7895 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/conftest.py
--rw-r--r--   0      501       20   410675 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/fixtures/aspen-m-3.json
--rw-r--r--   0      501       20      190 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/qcs_config/secrets.toml
--rw-r--r--   0      501       20      605 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/qcs_config/settings.toml
--rw-r--r--   0      501       20     2155 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/test_api.py
--rw-r--r--   0      501       20     1550 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/test_client.py
--rw-r--r--   0      501       20     1315 2023-02-08 14:49:19.000000 qcs_sdk_python-0.5.0rc5/tests/test_isa.py
--rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/Cargo.toml
+-rw-r--r--   0      501       20    13410 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/CHANGELOG.md
+-rw-r--r--   0      501       20      629 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/Makefile.toml
+-rw-r--r--   0      501       20     2186 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/README.md
+-rw-r--r--   0      501       20      562 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/delayed_job_retrieval.rs
+-rw-r--r--   0      501       20      444 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/execute.rs
+-rw-r--r--   0      501       20      459 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/local.rs
+-rw-r--r--   0      501       20     2140 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/parametric_compilation.rs
+-rw-r--r--   0      501       20     1135 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/quil_t.rs
+-rw-r--r--   0      501       20    13410 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/api.rs
+-rw-r--r--   0      501       20    27184 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/executable.rs
+-rw-r--r--   0      501       20     7451 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/execution_data.rs
+-rw-r--r--   0      501       20     1707 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/lib.rs
+-rw-r--r--   0      501       20     7714 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/client.rs
+-rw-r--r--   0      501       20     8497 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/execution.rs
+-rw-r--r--   0      501       20     1195 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/mod.rs
+-rw-r--r--   0      501       20     8348 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/edge.rs
+-rw-r--r--   0      501       20     6825 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/mod.rs
+-rw-r--r--   0      501       20     8419 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/operator.rs
+-rw-r--r--   0      501       20    11917 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/qubit.rs
+-rw-r--r--   0      501       20     9358 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/mod.rs
+-rw-r--r--   0      501       20    16899 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/rewrite_arithmetic.rs
+-rw-r--r--   0      501       20     7240 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/rpcq.rs
+-rw-r--r--   0      501       20     8231 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/runner.rs
+-rw-r--r--   0      501       20     1399 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/translation.rs
+-rw-r--r--   0      501       20     6987 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qvm/execution.rs
+-rw-r--r--   0      501       20     2355 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qvm/mod.rs
+-rw-r--r--   0      501       20     1504 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/register_data.rs
+-rw-r--r--   0      501       20   104426 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/aspen_9_isa.json
+-rw-r--r--   0      501       20     1246 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/basic_qvm.rs
+-rw-r--r--   0      501       20      558 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/bell_state_response_data.hex
+-rw-r--r--   0      501       20    81629 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/compiler-isa-Aspen-8.json
+-rw-r--r--   0      501       20    11089 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/mocked_qpu.rs
+-rw-r--r--   0      501       20     1433 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/parametric_compilation.rs
+-rw-r--r--   0      501       20    71490 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/qcs-isa-Aspen-8.json
+-rw-r--r--   0      501       20     2275 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/qvm_isa.json
+-rw-r--r--   0      501       20      148 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/secrets.toml
+-rw-r--r--   0      501       20      298 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/settings.toml
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc6/Cargo.toml
+-rw-r--r--   0      501       20    11240 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/CHANGELOG.md
+-rw-r--r--   0      501       20      539 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/Makefile.toml
+-rw-r--r--   0      501       20      613 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/README.md
+-rw-r--r--   0      501       20       71 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/build.rs
+-rw-r--r--   0      501       20     6538 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/poetry.lock
+-rw-r--r--   0      501       20     1643 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/pyproject.toml
+-rw-r--r--   0      501       20      155 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/__init__.py
+-rw-r--r--   0      501       20      527 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/__init__.pyi
+-rw-r--r--   0      501       20     2636 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/_executable.pyi
+-rw-r--r--   0      501       20     2065 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/_execution_data.pyi
+-rw-r--r--   0      501       20     1783 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/_register_data.pyi
+-rw-r--r--   0      501       20    12838 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/api.pyi
+-rw-r--r--   0      501       20        0 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/py.typed
+-rw-r--r--   0      501       20       41 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/__init__.pyi
+-rw-r--r--   0      501       20     2540 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/client.pyi
+-rw-r--r--   0      501       20    10811 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/isa.pyi
+-rw-r--r--   0      501       20      601 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/quilc.pyi
+-rw-r--r--   0      501       20     9215 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/api.rs
+-rw-r--r--   0      501       20     4540 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/executable.rs
+-rw-r--r--   0      501       20     1708 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/execution_data.rs
+-rw-r--r--   0      501       20       16 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/grpc/mod.rs
+-rw-r--r--   0      501       20     2040 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/grpc/models/controller.rs
+-rw-r--r--   0      501       20       20 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/grpc/models/mod.rs
+-rw-r--r--   0      501       20     1125 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/lib.rs
+-rw-r--r--   0      501       20     6621 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/qpu/client.rs
+-rw-r--r--   0      501       20     4441 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/qpu/isa.rs
+-rw-r--r--   0      501       20      462 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/qpu/mod.rs
+-rw-r--r--   0      501       20     1028 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/qpu/quilc/mod.rs
+-rw-r--r--   0      501       20      387 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/src/register_data.rs
+-rw-r--r--   0      501       20     7895 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/conftest.py
+-rw-r--r--   0      501       20   410675 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/fixtures/aspen-m-3.json
+-rw-r--r--   0      501       20      190 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/qcs_config/secrets.toml
+-rw-r--r--   0      501       20      605 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/qcs_config/settings.toml
+-rw-r--r--   0      501       20     2155 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/test_api.py
+-rw-r--r--   0      501       20     1976 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/test_client.py
+-rw-r--r--   0      501       20     1315 2023-02-08 20:14:17.000000 qcs_sdk_python-0.5.0rc6/tests/test_isa.py
+-rw-r--r--   0        0        0     1398 1970-01-01 00:00:00.000000 qcs_sdk_python-0.5.0rc6/PKG-INFO
```

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/Cargo.toml` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs"
 description = "High level interface for running Quil on a QPU"
-version = "0.10.0-rc.5"
+version = "0.10.0-rc.6"
 edition = "2018"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "compilers", "science", "emulators"]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/CHANGELOG.md` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.10.0-rc.6
+
+### Breaking Changes
+
+- implement Python wrappers for the full Rust API (#230)
+
+### Features
+
+- export qcs client url settings (#249)
+- support protoquil flag in compilation (rebase fix) (#243)
+- export get_quilt_calibrations (#247)
+
 ## 0.10.0-rc.5
 
 ### Breaking Changes
 
 - implement Python wrappers for the full Rust API (#230)
 
 ### Features
```

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/Makefile.toml` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/README.md` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/delayed_job_retrieval.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/delayed_job_retrieval.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/parametric_compilation.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/examples/quil_t.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/examples/quil_t.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/api.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/executable.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/execution_data.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/lib.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/client.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/client.rs`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     /// Enable or disable the use of Gateway service for execution
     #[must_use]
     pub fn with_use_gateway(mut self, use_gateway: bool) -> Self {
         self.use_gateway = use_gateway;
         self
     }
 
-    pub(crate) fn get_config(&self) -> ClientConfiguration {
+    /// Return a copy of all settings parsed and resolved from configuration sources.
+    #[must_use]
+    pub fn get_config(&self) -> ClientConfiguration {
         self.config.clone()
     }
 
     pub(crate) async fn get_controller_client(
         &self,
         quantum_processor_id: &str,
     ) -> Result<ControllerClient<RefreshService<Channel>>, GrpcEndpointError> {
```

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/execution.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/mod.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/edge.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/edge.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/mod.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/operator.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/operator.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/isa/qubit.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/isa/qubit.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/quilc/mod.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/quilc/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/rewrite_arithmetic.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/rewrite_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/rpcq.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/rpcq.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/runner.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/runner.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qpu/translation.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qpu/translation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qvm/execution.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qvm/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/qvm/mod.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/qvm/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/src/register_data.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/src/register_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/aspen_9_isa.json` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/aspen_9_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/basic_qvm.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/basic_qvm.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/bell_state_response_data.hex` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/bell_state_response_data.hex`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/compiler-isa-Aspen-8.json` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/compiler-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/mocked_qpu.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/mocked_qpu.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/parametric_compilation.rs` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/qcs-isa-Aspen-8.json` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/qcs-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/local_dependencies/qcs/tests/qvm_isa.json` & `qcs_sdk_python-0.5.0rc6/local_dependencies/qcs/tests/qvm_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/Cargo.toml` & `qcs_sdk_python-0.5.0rc6/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs-sdk-python"
 description = "Python bindings to qcs-sdk-rust"
-version = "0.5.0-rc.5"
+version = "0.5.0-rc.6"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "compilers", "science", "emulators"]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python-0.5.0rc5/CHANGELOG.md` & `qcs_sdk_python-0.5.0rc6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## 0.5.0-rc.6
+
+### Breaking Changes
+
+- implement Python wrappers for the full Rust API (#230)
+
+### Features
+
+- export qcs client url settings (#249)
+- support protoquil flag in compilation (rebase fix) (#243)
+- export get_quilt_calibrations (#247)
+- implement get_instruction_set_architecture (#240)
+
 ## 0.5.0-rc.5
 
 ### Breaking Changes
 
 - implement Python wrappers for the full Rust API (#230)
 
 ### Features
```

### Comparing `qcs_sdk_python-0.5.0rc5/Makefile.toml` & `qcs_sdk_python-0.5.0rc6/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/README.md` & `qcs_sdk_python-0.5.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/poetry.lock` & `qcs_sdk_python-0.5.0rc6/poetry.lock`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/pyproject.toml` & `qcs_sdk_python-0.5.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This is the metadata Maturin uploads to PyPI on publish
 [project]
 name = "qcs-sdk-python"
-version = "0.5.0-rc.5"
+version = "0.5.0-rc.6"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 authors = [
 	{ name = "Rigetti Computing", email = "softapps@rigetti.com" },
 	{ name = "Mark Skilbeck", email = "mark.skilbeck@rigetti.com" },
 	{ name = "Marquess Valdez", email = "mvaldez@rigetti.com" },
@@ -20,15 +20,15 @@
 	"Operating System :: OS Independent",
 ]
 
 # PEP 621 specifies the [project] table as the source for project metadata. However, Poetry only supports [tool.poetry]
 # We can remove this table once this issue is resolved: https://github.com/python-poetry/poetry/issues/3332
 [tool.poetry]
 name = "qcs-sdk-python"
-version = "0.5.0-rc.5"
+version = "0.5.0-rc.6"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 authors = [
 	"Rigetti Computing <softapps@rigetti.com>",
 	"Mark Skilbeck <mark.skilbeck@rigetti.com>",
 	"Marquess Valdez <mvaldez@rigetti.com>",
 	"Randall Fulton <rfulton@rigetti.com>",
```

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/__init__.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/_executable.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/_executable.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/_execution_data.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/_execution_data.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/_register_data.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/_register_data.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/api.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/client.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -19,25 +19,45 @@
         Construct a client from scratch.
         
         Use ``QcsClient.load`` to construct an environment-based profile.
         """
         ...
     
     @staticmethod
-    def load(
+    async def load(
         profile_name: Optional[str] = None,
         use_gateway: Optional[bool] = None,
     ) -> "QcsClient":
         """
         Load a QcsClient configuration using an environment-based configuration.
 
         See for details: https://docs.rigetti.com/qcs/references/qcs-client-configuration#environment-variables-and-configuration-files
         """
         ...
 
+    @property
+    def api_url(self) -> str:
+        """URL to access the QCS API."""
+        ...
+
+    @property
+    def grpc_api_url(self) -> str:
+        """URL to access the gRPC API."""
+        ...
+
+    @property
+    def quilc_url(self) -> str:
+        """URL to access the `quilc` compiler."""
+        ...
+
+    @property
+    def qvm_url(self) -> str:
+        """URL to access the QVM."""
+        ...
+
 
 class QcsClientAuthServer:
     """Authentication server configuration for the QCS API."""
 
     @property
     def client_id(self) -> str: ...
     @client_id.setter
```

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/isa.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/isa.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/qcs_sdk/qpu/quilc.pyi` & `qcs_sdk_python-0.5.0rc6/qcs_sdk/qpu/quilc.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/api.rs` & `qcs_sdk_python-0.5.0rc6/src/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/executable.rs` & `qcs_sdk_python-0.5.0rc6/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/execution_data.rs` & `qcs_sdk_python-0.5.0rc6/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/grpc/models/controller.rs` & `qcs_sdk_python-0.5.0rc6/src/grpc/models/controller.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/lib.rs` & `qcs_sdk_python-0.5.0rc6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/qpu/client.rs` & `qcs_sdk_python-0.5.0rc6/src/qpu/client.rs`

 * *Files 10% similar despite different names*

```diff
@@ -206,14 +206,34 @@
                 Some(use_gateway) => client.with_use_gateway(use_gateway),
             };
 
             Ok(Self(client))
         })
     }
 
+    #[getter]
+    pub fn api_url(&self) -> String {
+        self.as_ref().get_config().api_url().to_string()
+    }
+
+    #[getter]
+    pub fn grpc_api_url(&self) -> String {
+        self.as_ref().get_config().grpc_api_url().to_string()
+    }
+
+    #[getter]
+    pub fn quilc_url(&self) -> String {
+        self.as_ref().get_config().quilc_url().to_string()
+    }
+
+    #[getter]
+    pub fn qvm_url(&self) -> String {
+        self.as_ref().get_config().qvm_url().to_string()
+    }
+
     fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
         match op {
             CompareOp::Eq => (self == other).into_py(py),
             CompareOp::Ne => (self != other).into_py(py),
             _ => py.NotImplemented(),
         }
     }
```

### Comparing `qcs_sdk_python-0.5.0rc5/src/qpu/isa.rs` & `qcs_sdk_python-0.5.0rc6/src/qpu/isa.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/src/qpu/quilc/mod.rs` & `qcs_sdk_python-0.5.0rc6/src/qpu/quilc/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/tests/conftest.py` & `qcs_sdk_python-0.5.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/tests/fixtures/aspen-m-3.json` & `qcs_sdk_python-0.5.0rc6/tests/fixtures/aspen-m-3.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/tests/qcs_config/settings.toml` & `qcs_sdk_python-0.5.0rc6/tests/qcs_config/settings.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/tests/test_api.py` & `qcs_sdk_python-0.5.0rc6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/tests/test_client.py` & `qcs_sdk_python-0.5.0rc6/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import pytest
+from urllib.parse import urlparse
 
 from qcs_sdk import QcsClient
 from qcs_sdk.qpu.client import QcsLoadError, QcsClientAuthServer, QcsClientTokens
 
 @pytest.fixture
 def default_client():
     return QcsClient()
 
+@pytest.mark.asyncio
+async def test_client_has_url_from_env(default_client: QcsClient):
+    """The default client is configured with valid urls."""
+    assert urlparse(default_client.api_url).geturl() != ""
+    assert urlparse(default_client.grpc_api_url).geturl() != ""
+    assert urlparse(default_client.quilc_url).geturl() != ""
+    assert urlparse(default_client.qvm_url).geturl() != ""
+
 
 @pytest.mark.asyncio
 async def test_client_empty_profile_is_default(default_client: QcsClient):
     """The profile "empty" is configured to be similar to a default client."""
     client = await QcsClient.load(profile_name="empty")
 
     assert client == default_client
```

### Comparing `qcs_sdk_python-0.5.0rc5/tests/test_isa.py` & `qcs_sdk_python-0.5.0rc6/tests/test_isa.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python-0.5.0rc5/PKG-INFO` & `qcs_sdk_python-0.5.0rc6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs-sdk-python
-Version: 0.5.0rc5
+Version: 0.5.0rc6
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Summary: Python interface for the QCS Rust SDK
```

