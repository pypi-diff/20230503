# Comparing `tmp/jq-1.4.1.tar.gz` & `tmp/jq-1.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jq.py/jq.py/dist/.tmp-7vljnf8z/jq-1.4.1.tar", last modified: Thu Mar 16 16:00:28 2023, max compression
+gzip compressed data, was "jq-1.5.0a1.tar", last modified: Tue May  2 20:59:13 2023, max compression
```

## Comparing `jq-1.4.1.tar` & `jq-1.5.0a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:00:28.000000 jq-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-16 15:59:41.000000 jq-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-16 15:59:41.000000 jq-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-16 16:00:28.000000 jq-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-16 15:59:41.000000 jq-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:00:28.000000 jq-1.4.1/deps/
--rw-r--r--   0 runner    (1001) docker     (123)  1750584 2023-03-16 15:59:41.000000 jq-1.4.1/deps/jq-1.6.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908702 2023-03-16 15:59:41.000000 jq-1.4.1/deps/onig-6.9.4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   520016 2023-03-16 16:00:06.000000 jq-1.4.1/jq.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:00:28.000000 jq-1.4.1/jq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-16 16:00:28.000000 jq-1.4.1/jq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-16 16:00:28.000000 jq-1.4.1/jq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:00:28.000000 jq-1.4.1/jq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 16:00:28.000000 jq-1.4.1/jq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-16 15:59:41.000000 jq-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:00:28.000000 jq-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-16 15:59:41.000000 jq-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:13.325148 jq-1.5.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-02 20:58:41.000000 jq-1.5.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 20:58:41.000000 jq-1.5.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-02 20:59:13.325148 jq-1.5.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-02 20:58:41.000000 jq-1.5.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:13.325148 jq-1.5.0a1/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)  1750584 2023-05-02 20:58:41.000000 jq-1.5.0a1/deps/jq-1.6.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908702 2023-05-02 20:58:41.000000 jq-1.5.0a1/deps/onig-6.9.4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   552542 2023-05-02 20:58:56.000000 jq-1.5.0a1/jq.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:59:13.325148 jq-1.5.0a1/jq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-02 20:59:13.000000 jq-1.5.0a1/jq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-02 20:59:13.000000 jq-1.5.0a1/jq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:59:13.000000 jq-1.5.0a1/jq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-02 20:59:13.000000 jq-1.5.0a1/jq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 20:58:41.000000 jq-1.5.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:59:13.325148 jq-1.5.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-02 20:58:41.000000 jq-1.5.0a1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jq-1.4.1/LICENSE` & `jq-1.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jq-1.4.1/deps/jq-1.6.tar.gz` & `jq-1.5.0a1/deps/jq-1.6.tar.gz`

 * *Files identical despite different names*

### Comparing `jq-1.4.1/deps/onig-6.9.4.tar.gz` & `jq-1.5.0a1/deps/onig-6.9.4.tar.gz`

 * *Files identical despite different names*

### Comparing `jq-1.4.1/jq.c` & `jq-1.5.0a1/jq.c`

 * *Files 2% similar despite different names*

```diff
@@ -954,41 +954,41 @@
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "jq.pyx",
   "stringsource",
-  "_virtualenv/lib/python3.7/site-packages/Cython/Includes/cpython/type.pxd",
+  "_virtualenv/lib/python3.11/site-packages/Cython/Includes/cpython/type.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_2jq__ErrorStore;
 struct __pyx_obj_2jq__JqStatePool;
 struct __pyx_obj_2jq__Program;
 struct __pyx_obj_2jq__ProgramWithInput;
 struct __pyx_obj_2jq__ResultIterator;
 struct __pyx_obj_2jq___pyx_scope_struct__text;
 struct __pyx_obj_2jq___pyx_scope_struct_1_genexpr;
 
-/* "jq.pyx":181
+/* "jq.pyx":184
  * 
  * 
  * cdef class _ErrorStore(object):             # <<<<<<<<<<<<<<
  *     cdef object _errors
  * 
  */
 struct __pyx_obj_2jq__ErrorStore {
   PyObject_HEAD
   struct __pyx_vtabstruct_2jq__ErrorStore *__pyx_vtab;
   PyObject *_errors;
 };
 
 
-/* "jq.pyx":206
+/* "jq.pyx":209
  * 
  * 
  * cdef class _JqStatePool(object):             # <<<<<<<<<<<<<<
  *     cdef jq_state* _jq_state
  *     cdef object _program_bytes
  */
 struct __pyx_obj_2jq__JqStatePool {
@@ -997,75 +997,77 @@
   jq_state *_jq_state;
   PyObject *_program_bytes;
   PyObject *_args;
   PyObject *_lock;
 };
 
 
-/* "jq.pyx":238
+/* "jq.pyx":241
  * 
  * 
  * cdef class _Program(object):             # <<<<<<<<<<<<<<
  *     cdef object _program_bytes
  *     cdef _JqStatePool _jq_state_pool
  */
 struct __pyx_obj_2jq__Program {
   PyObject_HEAD
   PyObject *_program_bytes;
   struct __pyx_obj_2jq__JqStatePool *_jq_state_pool;
 };
 
 
-/* "jq.pyx":271
+/* "jq.pyx":289
  * 
  * 
  * cdef class _ProgramWithInput(object):             # <<<<<<<<<<<<<<
  *     cdef _JqStatePool _jq_state_pool
  *     cdef object _bytes_input
  */
 struct __pyx_obj_2jq__ProgramWithInput {
   PyObject_HEAD
   struct __pyx_vtabstruct_2jq__ProgramWithInput *__pyx_vtab;
   struct __pyx_obj_2jq__JqStatePool *_jq_state_pool;
   PyObject *_bytes_input;
+  int _slurp;
 };
 
 
-/* "jq.pyx":299
+/* "jq.pyx":319
  * 
  * 
  * cdef class _ResultIterator(object):             # <<<<<<<<<<<<<<
  *     cdef _JqStatePool _jq_state_pool
  *     cdef jq_state* _jq
  */
 struct __pyx_obj_2jq__ResultIterator {
   PyObject_HEAD
   struct __pyx_vtabstruct_2jq__ResultIterator *__pyx_vtab;
   struct __pyx_obj_2jq__JqStatePool *_jq_state_pool;
   jq_state *_jq;
   struct jv_parser *_parser;
   PyObject *_bytes_input;
+  int _slurp;
   int _ready;
 };
 
 
-/* "jq.pyx":285
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+/* "jq.pyx":305
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  *     def text(self):             # <<<<<<<<<<<<<<
  *         # Performance testing suggests that using _jv_to_python (within the
  *         # result iterator) followed by json.dumps is faster than using
  */
 struct __pyx_obj_2jq___pyx_scope_struct__text {
   PyObject_HEAD
   struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self;
 };
 
 
-/* "jq.pyx":290
+/* "jq.pyx":310
  *         # jv_dump_string to generate the string directly from the jv values.
  *         # See: https://github.com/mwilliamson/jq.py/pull/50
  *         return "\n".join(json.dumps(v) for v in self)             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
 struct __pyx_obj_2jq___pyx_scope_struct_1_genexpr {
@@ -1075,15 +1077,15 @@
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
 
-/* "jq.pyx":181
+/* "jq.pyx":184
  * 
  * 
  * cdef class _ErrorStore(object):             # <<<<<<<<<<<<<<
  *     cdef object _errors
  * 
  */
 
@@ -1092,55 +1094,57 @@
   PyObject *(*error_string)(struct __pyx_obj_2jq__ErrorStore *);
   void (*store_error)(struct __pyx_obj_2jq__ErrorStore *, PyObject *);
   void (*clear)(struct __pyx_obj_2jq__ErrorStore *);
 };
 static struct __pyx_vtabstruct_2jq__ErrorStore *__pyx_vtabptr_2jq__ErrorStore;
 
 
-/* "jq.pyx":206
+/* "jq.pyx":209
  * 
  * 
  * cdef class _JqStatePool(object):             # <<<<<<<<<<<<<<
  *     cdef jq_state* _jq_state
  *     cdef object _program_bytes
  */
 
 struct __pyx_vtabstruct_2jq__JqStatePool {
   jq_state *(*acquire)(struct __pyx_obj_2jq__JqStatePool *);
   void (*release)(struct __pyx_obj_2jq__JqStatePool *, jq_state *);
 };
 static struct __pyx_vtabstruct_2jq__JqStatePool *__pyx_vtabptr_2jq__JqStatePool;
 
 
-/* "jq.pyx":271
+/* "jq.pyx":289
  * 
  * 
  * cdef class _ProgramWithInput(object):             # <<<<<<<<<<<<<<
  *     cdef _JqStatePool _jq_state_pool
  *     cdef object _bytes_input
  */
 
 struct __pyx_vtabstruct_2jq__ProgramWithInput {
   struct __pyx_obj_2jq__ResultIterator *(*_make_iterator)(struct __pyx_obj_2jq__ProgramWithInput *);
 };
 static struct __pyx_vtabstruct_2jq__ProgramWithInput *__pyx_vtabptr_2jq__ProgramWithInput;
 
 
-/* "jq.pyx":299
+/* "jq.pyx":319
  * 
  * 
  * cdef class _ResultIterator(object):             # <<<<<<<<<<<<<<
  *     cdef _JqStatePool _jq_state_pool
  *     cdef jq_state* _jq
  */
 
 struct __pyx_vtabstruct_2jq__ResultIterator {
   int (*_ready_next_input)(struct __pyx_obj_2jq__ResultIterator *);
+  jv (*_parse_next_input)(struct __pyx_obj_2jq__ResultIterator *);
 };
 static struct __pyx_vtabstruct_2jq__ResultIterator *__pyx_vtabptr_2jq__ResultIterator;
+static CYTHON_INLINE jv __pyx_f_2jq_15_ResultIterator__parse_next_input(struct __pyx_obj_2jq__ResultIterator *);
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1486,14 +1490,17 @@
     #else
     #define __Pyx_PyBytes_Join _PyBytes_Join
     #endif
 #else
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values);
 #endif
 
+/* RaiseKeywordRequired.proto */
+static void __Pyx_RaiseKeywordRequired(const char* func_name, PyObject* kw_name);
+
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
 
 /* IterNext.proto */
@@ -1502,14 +1509,22 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
@@ -1542,22 +1557,14 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
@@ -1731,14 +1738,15 @@
 static PyObject *__pyx_f_2jq_11_ErrorStore_error_string(struct __pyx_obj_2jq__ErrorStore *__pyx_v_self); /* proto*/
 static void __pyx_f_2jq_11_ErrorStore_store_error(struct __pyx_obj_2jq__ErrorStore *__pyx_v_self, PyObject *__pyx_v_error); /* proto*/
 static void __pyx_f_2jq_11_ErrorStore_clear(struct __pyx_obj_2jq__ErrorStore *__pyx_v_self); /* proto*/
 static jq_state *__pyx_f_2jq_12_JqStatePool_acquire(struct __pyx_obj_2jq__JqStatePool *__pyx_v_self); /* proto*/
 static void __pyx_f_2jq_12_JqStatePool_release(struct __pyx_obj_2jq__JqStatePool *__pyx_v_self, jq_state *__pyx_v_state); /* proto*/
 static struct __pyx_obj_2jq__ResultIterator *__pyx_f_2jq_17_ProgramWithInput__make_iterator(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto*/
 static int __pyx_f_2jq_15_ResultIterator__ready_next_input(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto*/
+static CYTHON_INLINE jv __pyx_f_2jq_15_ResultIterator__parse_next_input(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto*/
 
 /* Module declarations from 'libc.string' */
 
 /* Module declarations from 'libc.stdio' */
 
 /* Module declarations from '__builtin__' */
 
@@ -1775,19 +1783,21 @@
 /* Implementation of 'jq' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_StopIteration;
 static const char __pyx_k__5[] = "\n";
+static const char __pyx_k_io[] = "io";
 static const char __pyx_k_jq[] = "jq";
 static const char __pyx_k_all[] = "all";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_Lock[] = "Lock";
 static const char __pyx_k_args[] = "args";
+static const char __pyx_k_dump[] = "dump";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_iter[] = "_iter";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_send[] = "send";
@@ -1796,17 +1806,19 @@
 static const char __pyx_k_utf8[] = "utf8";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_dumps[] = "dumps";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_first[] = "first";
 static const char __pyx_k_input[] = "input";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_slurp[] = "slurp";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
+static const char __pyx_k_write[] = "write";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_iter_2[] = "iter";
 static const char __pyx_k_jq_pyx[] = "jq.pyx";
@@ -1815,27 +1827,31 @@
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_Program[] = "_Program";
 static const char __pyx_k_compile[] = "compile";
 static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_program[] = "program";
 static const char __pyx_k_NO_VALUE[] = "_NO_VALUE";
+static const char __pyx_k_StringIO[] = "StringIO";
 static const char __pyx_k_getstate[] = "__getstate__";
+static const char __pyx_k_getvalue[] = "getvalue";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_threading[] = "threading";
 static const char __pyx_k_EmptyValue[] = "_EmptyValue";
 static const char __pyx_k_ErrorStore[] = "_ErrorStore";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_input_text[] = "input_text";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_JqStatePool[] = "_JqStatePool";
 static const char __pyx_k_bytes_input[] = "bytes_input";
+static const char __pyx_k_input_value[] = "input_value";
 static const char __pyx_k_parse_error[] = "parse error: ";
 static const char __pyx_k_text_output[] = "text_output";
 static const char __pyx_k_jq_compile_r[] = "jq.compile({!r})";
 static const char __pyx_k_Invalid_value[] = "Invalid value";
 static const char __pyx_k_StopIteration[] = "StopIteration";
 static const char __pyx_k_jq_state_pool[] = "jq_state_pool";
 static const char __pyx_k_program_bytes[] = "program_bytes";
@@ -1861,37 +1877,43 @@
 static PyObject *__pyx_n_s_JqStatePool;
 static PyObject *__pyx_n_s_Lock;
 static PyObject *__pyx_n_s_NO_VALUE;
 static PyObject *__pyx_n_s_Program;
 static PyObject *__pyx_n_s_ProgramWithInput;
 static PyObject *__pyx_n_s_ResultIterator;
 static PyObject *__pyx_n_s_StopIteration;
+static PyObject *__pyx_n_s_StringIO;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_s__5;
 static PyObject *__pyx_n_s_all;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_bytes_input;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_compilation_lock;
 static PyObject *__pyx_n_s_compile;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_doc;
+static PyObject *__pyx_n_s_dump;
 static PyObject *__pyx_n_s_dumps;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_exit;
 static PyObject *__pyx_n_s_first;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_n_s_getvalue;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_input;
+static PyObject *__pyx_n_s_input_text;
+static PyObject *__pyx_n_s_input_value;
+static PyObject *__pyx_n_s_io;
 static PyObject *__pyx_n_s_iter;
 static PyObject *__pyx_n_s_iter_2;
 static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_jq;
 static PyObject *__pyx_kp_s_jq_compile_r;
 static PyObject *__pyx_kp_s_jq_init_failed;
 static PyObject *__pyx_kp_s_jq_pyx;
@@ -1915,48 +1937,53 @@
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_slurp;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_text;
 static PyObject *__pyx_n_s_text_locals_genexpr;
 static PyObject *__pyx_n_s_text_output;
 static PyObject *__pyx_n_s_threading;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_utf8;
 static PyObject *__pyx_kp_s_utf_8;
 static PyObject *__pyx_n_s_value;
+static PyObject *__pyx_n_s_write;
 static PyObject *__pyx_pf_2jq_compile(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_program, PyObject *__pyx_v_args); /* proto */
 static int __pyx_pf_2jq_11_ErrorStore___cinit__(struct __pyx_obj_2jq__ErrorStore *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_11_ErrorStore_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ErrorStore *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_11_ErrorStore_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ErrorStore *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_2jq_12_JqStatePool___cinit__(struct __pyx_obj_2jq__JqStatePool *__pyx_v_self, PyObject *__pyx_v_program_bytes, PyObject *__pyx_v_args); /* proto */
 static void __pyx_pf_2jq_12_JqStatePool_2__dealloc__(struct __pyx_obj_2jq__JqStatePool *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_12_JqStatePool_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__JqStatePool *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_12_JqStatePool_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__JqStatePool *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_2jq_8_Program___cinit__(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_program_bytes, PyObject *__pyx_v_args); /* proto */
 static PyObject *__pyx_pf_2jq_8_Program_2input(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_4input_value(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_6input_values(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_values); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_8input_text(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_slurp); /* proto */
 static PyObject *__pyx_pf_2jq_8_Program_14program_string___get__(struct __pyx_obj_2jq__Program *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2jq_8_Program_4__repr__(struct __pyx_obj_2jq__Program *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2jq_8_Program_6transform(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text, PyObject *__pyx_v_text_output, PyObject *__pyx_v_multiple_output); /* proto */
-static PyObject *__pyx_pf_2jq_8_Program_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2jq_8_Program_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_2jq_17_ProgramWithInput___cinit__(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self, PyObject *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_10__repr__(struct __pyx_obj_2jq__Program *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_12transform(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text, PyObject *__pyx_v_text_output, PyObject *__pyx_v_multiple_output); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_2jq_8_Program_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_2jq_17_ProgramWithInput___cinit__(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self, PyObject *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input, int __pyx_v_slurp); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_2__iter__(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_4text_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_4text(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_6all(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_8first(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_pf_2jq_15_ResultIterator___dealloc__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto */
-static int __pyx_pf_2jq_15_ResultIterator_2__cinit__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self, struct __pyx_obj_2jq__JqStatePool *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input); /* proto */
+static int __pyx_pf_2jq_15_ResultIterator_2__cinit__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self, struct __pyx_obj_2jq__JqStatePool *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input, int __pyx_v_slurp); /* proto */
 static PyObject *__pyx_pf_2jq_15_ResultIterator_4__iter__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_15_ResultIterator_6__next__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_15_ResultIterator_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ResultIterator *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2jq_15_ResultIterator_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__ResultIterator *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_2jq_2all(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_program, PyObject *__pyx_v_value, PyObject *__pyx_v_text); /* proto */
 static PyObject *__pyx_pf_2jq_4first(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_program, PyObject *__pyx_v_value, PyObject *__pyx_v_text); /* proto */
 static PyObject *__pyx_pf_2jq_6iter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_program, PyObject *__pyx_v_value, PyObject *__pyx_v_text); /* proto */
@@ -2007,15 +2034,15 @@
 static PyObject *__pyx_codeobj__33;
 static PyObject *__pyx_codeobj__35;
 static PyObject *__pyx_codeobj__37;
 static PyObject *__pyx_codeobj__39;
 static PyObject *__pyx_codeobj__41;
 /* Late includes */
 
-/* "jq.pyx":69
+/* "jq.pyx":72
  * 
  * 
  * cdef object _jv_to_python(jv value):             # <<<<<<<<<<<<<<
  *     """Unpack a jv value into a Python value"""
  *     cdef jv_kind kind = jv_get_kind(value)
  */
 
@@ -2043,438 +2070,438 @@
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_jv_to_python", 0);
 
-  /* "jq.pyx":71
+  /* "jq.pyx":74
  * cdef object _jv_to_python(jv value):
  *     """Unpack a jv value into a Python value"""
  *     cdef jv_kind kind = jv_get_kind(value)             # <<<<<<<<<<<<<<
  *     cdef int idx
  *     cdef jv property_key
  */
   __pyx_v_kind = jv_get_kind(__pyx_v_value);
 
-  /* "jq.pyx":78
+  /* "jq.pyx":81
  *     cdef double number_value
  * 
  *     if kind == JV_KIND_INVALID:             # <<<<<<<<<<<<<<
  *         raise ValueError("Invalid value")
  *     elif kind == JV_KIND_NULL:
  */
   switch (__pyx_v_kind) {
     case JV_KIND_INVALID:
 
-    /* "jq.pyx":79
+    /* "jq.pyx":82
  * 
  *     if kind == JV_KIND_INVALID:
  *         raise ValueError("Invalid value")             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_NULL:
  *         python_value = None
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 79, __pyx_L1_error)
+    __PYX_ERR(0, 82, __pyx_L1_error)
 
-    /* "jq.pyx":78
+    /* "jq.pyx":81
  *     cdef double number_value
  * 
  *     if kind == JV_KIND_INVALID:             # <<<<<<<<<<<<<<
  *         raise ValueError("Invalid value")
  *     elif kind == JV_KIND_NULL:
  */
     break;
     case JV_KIND_NULL:
 
-    /* "jq.pyx":81
+    /* "jq.pyx":84
  *         raise ValueError("Invalid value")
  *     elif kind == JV_KIND_NULL:
  *         python_value = None             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_FALSE:
  *         python_value = False
  */
     __Pyx_INCREF(Py_None);
     __pyx_v_python_value = Py_None;
 
-    /* "jq.pyx":80
+    /* "jq.pyx":83
  *     if kind == JV_KIND_INVALID:
  *         raise ValueError("Invalid value")
  *     elif kind == JV_KIND_NULL:             # <<<<<<<<<<<<<<
  *         python_value = None
  *     elif kind == JV_KIND_FALSE:
  */
     break;
     case JV_KIND_FALSE:
 
-    /* "jq.pyx":83
+    /* "jq.pyx":86
  *         python_value = None
  *     elif kind == JV_KIND_FALSE:
  *         python_value = False             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_TRUE:
  *         python_value = True
  */
     __Pyx_INCREF(Py_False);
     __pyx_v_python_value = Py_False;
 
-    /* "jq.pyx":82
+    /* "jq.pyx":85
  *     elif kind == JV_KIND_NULL:
  *         python_value = None
  *     elif kind == JV_KIND_FALSE:             # <<<<<<<<<<<<<<
  *         python_value = False
  *     elif kind == JV_KIND_TRUE:
  */
     break;
     case JV_KIND_TRUE:
 
-    /* "jq.pyx":85
+    /* "jq.pyx":88
  *         python_value = False
  *     elif kind == JV_KIND_TRUE:
  *         python_value = True             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_NUMBER:
  *         number_value = jv_number_value(value)
  */
     __Pyx_INCREF(Py_True);
     __pyx_v_python_value = Py_True;
 
-    /* "jq.pyx":84
+    /* "jq.pyx":87
  *     elif kind == JV_KIND_FALSE:
  *         python_value = False
  *     elif kind == JV_KIND_TRUE:             # <<<<<<<<<<<<<<
  *         python_value = True
  *     elif kind == JV_KIND_NUMBER:
  */
     break;
     case JV_KIND_NUMBER:
 
-    /* "jq.pyx":87
+    /* "jq.pyx":90
  *         python_value = True
  *     elif kind == JV_KIND_NUMBER:
  *         number_value = jv_number_value(value)             # <<<<<<<<<<<<<<
  *         if number_value == INFINITY:
  *             python_value = DBL_MAX
  */
     __pyx_v_number_value = jv_number_value(__pyx_v_value);
 
-    /* "jq.pyx":88
+    /* "jq.pyx":91
  *     elif kind == JV_KIND_NUMBER:
  *         number_value = jv_number_value(value)
  *         if number_value == INFINITY:             # <<<<<<<<<<<<<<
  *             python_value = DBL_MAX
  *         elif number_value == -INFINITY:
  */
     __pyx_t_2 = ((__pyx_v_number_value == INFINITY) != 0);
     if (__pyx_t_2) {
 
-      /* "jq.pyx":89
+      /* "jq.pyx":92
  *         number_value = jv_number_value(value)
  *         if number_value == INFINITY:
  *             python_value = DBL_MAX             # <<<<<<<<<<<<<<
  *         elif number_value == -INFINITY:
  *             python_value = -DBL_MAX
  */
-      __pyx_t_1 = PyFloat_FromDouble(DBL_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble(DBL_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_python_value = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "jq.pyx":88
+      /* "jq.pyx":91
  *     elif kind == JV_KIND_NUMBER:
  *         number_value = jv_number_value(value)
  *         if number_value == INFINITY:             # <<<<<<<<<<<<<<
  *             python_value = DBL_MAX
  *         elif number_value == -INFINITY:
  */
       goto __pyx_L3;
     }
 
-    /* "jq.pyx":90
+    /* "jq.pyx":93
  *         if number_value == INFINITY:
  *             python_value = DBL_MAX
  *         elif number_value == -INFINITY:             # <<<<<<<<<<<<<<
  *             python_value = -DBL_MAX
  *         elif number_value != number_value:
  */
     __pyx_t_2 = ((__pyx_v_number_value == (-INFINITY)) != 0);
     if (__pyx_t_2) {
 
-      /* "jq.pyx":91
+      /* "jq.pyx":94
  *             python_value = DBL_MAX
  *         elif number_value == -INFINITY:
  *             python_value = -DBL_MAX             # <<<<<<<<<<<<<<
  *         elif number_value != number_value:
  *             python_value = None
  */
-      __pyx_t_1 = PyFloat_FromDouble((-DBL_MAX)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble((-DBL_MAX)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_python_value = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "jq.pyx":90
+      /* "jq.pyx":93
  *         if number_value == INFINITY:
  *             python_value = DBL_MAX
  *         elif number_value == -INFINITY:             # <<<<<<<<<<<<<<
  *             python_value = -DBL_MAX
  *         elif number_value != number_value:
  */
       goto __pyx_L3;
     }
 
-    /* "jq.pyx":92
+    /* "jq.pyx":95
  *         elif number_value == -INFINITY:
  *             python_value = -DBL_MAX
  *         elif number_value != number_value:             # <<<<<<<<<<<<<<
  *             python_value = None
  *         elif _is_integer(number_value):
  */
     __pyx_t_2 = ((__pyx_v_number_value != __pyx_v_number_value) != 0);
     if (__pyx_t_2) {
 
-      /* "jq.pyx":93
+      /* "jq.pyx":96
  *             python_value = -DBL_MAX
  *         elif number_value != number_value:
  *             python_value = None             # <<<<<<<<<<<<<<
  *         elif _is_integer(number_value):
  *             python_value = int(number_value)
  */
       __Pyx_INCREF(Py_None);
       __pyx_v_python_value = Py_None;
 
-      /* "jq.pyx":92
+      /* "jq.pyx":95
  *         elif number_value == -INFINITY:
  *             python_value = -DBL_MAX
  *         elif number_value != number_value:             # <<<<<<<<<<<<<<
  *             python_value = None
  *         elif _is_integer(number_value):
  */
       goto __pyx_L3;
     }
 
-    /* "jq.pyx":94
+    /* "jq.pyx":97
  *         elif number_value != number_value:
  *             python_value = None
  *         elif _is_integer(number_value):             # <<<<<<<<<<<<<<
  *             python_value = int(number_value)
  *         else:
  */
     __pyx_t_2 = (__pyx_f_2jq__is_integer(__pyx_v_number_value) != 0);
     if (__pyx_t_2) {
 
-      /* "jq.pyx":95
+      /* "jq.pyx":98
  *             python_value = None
  *         elif _is_integer(number_value):
  *             python_value = int(number_value)             # <<<<<<<<<<<<<<
  *         else:
  *             python_value = number_value
  */
-      __pyx_t_1 = __Pyx_PyInt_FromDouble(__pyx_v_number_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_FromDouble(__pyx_v_number_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_python_value = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "jq.pyx":94
+      /* "jq.pyx":97
  *         elif number_value != number_value:
  *             python_value = None
  *         elif _is_integer(number_value):             # <<<<<<<<<<<<<<
  *             python_value = int(number_value)
  *         else:
  */
       goto __pyx_L3;
     }
 
-    /* "jq.pyx":97
+    /* "jq.pyx":100
  *             python_value = int(number_value)
  *         else:
  *             python_value = number_value             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_STRING:
  *         python_value = jv_string_to_py_string(value)
  */
     /*else*/ {
-      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_number_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_number_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_python_value = __pyx_t_1;
       __pyx_t_1 = 0;
     }
     __pyx_L3:;
 
-    /* "jq.pyx":86
+    /* "jq.pyx":89
  *     elif kind == JV_KIND_TRUE:
  *         python_value = True
  *     elif kind == JV_KIND_NUMBER:             # <<<<<<<<<<<<<<
  *         number_value = jv_number_value(value)
  *         if number_value == INFINITY:
  */
     break;
     case JV_KIND_STRING:
 
-    /* "jq.pyx":99
+    /* "jq.pyx":102
  *             python_value = number_value
  *     elif kind == JV_KIND_STRING:
  *         python_value = jv_string_to_py_string(value)             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_ARRAY:
  *         python_value = []
  */
-    __pyx_t_1 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_python_value = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "jq.pyx":98
+    /* "jq.pyx":101
  *         else:
  *             python_value = number_value
  *     elif kind == JV_KIND_STRING:             # <<<<<<<<<<<<<<
  *         python_value = jv_string_to_py_string(value)
  *     elif kind == JV_KIND_ARRAY:
  */
     break;
     case JV_KIND_ARRAY:
 
-    /* "jq.pyx":101
+    /* "jq.pyx":104
  *         python_value = jv_string_to_py_string(value)
  *     elif kind == JV_KIND_ARRAY:
  *         python_value = []             # <<<<<<<<<<<<<<
  *         for idx in range(0, jv_array_length(jv_copy(value))):
  *             property_value = jv_array_get(jv_copy(value), idx)
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_python_value = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "jq.pyx":102
+    /* "jq.pyx":105
  *     elif kind == JV_KIND_ARRAY:
  *         python_value = []
  *         for idx in range(0, jv_array_length(jv_copy(value))):             # <<<<<<<<<<<<<<
  *             property_value = jv_array_get(jv_copy(value), idx)
  *             python_value.append(_jv_to_python(property_value))
  */
     __pyx_t_3 = jv_array_length(jv_copy(__pyx_v_value));
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_idx = __pyx_t_5;
 
-      /* "jq.pyx":103
+      /* "jq.pyx":106
  *         python_value = []
  *         for idx in range(0, jv_array_length(jv_copy(value))):
  *             property_value = jv_array_get(jv_copy(value), idx)             # <<<<<<<<<<<<<<
  *             python_value.append(_jv_to_python(property_value))
  *     elif kind == JV_KIND_OBJECT:
  */
       __pyx_v_property_value = jv_array_get(jv_copy(__pyx_v_value), __pyx_v_idx);
 
-      /* "jq.pyx":104
+      /* "jq.pyx":107
  *         for idx in range(0, jv_array_length(jv_copy(value))):
  *             property_value = jv_array_get(jv_copy(value), idx)
  *             python_value.append(_jv_to_python(property_value))             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_OBJECT:
  *         python_value = {}
  */
-      __pyx_t_1 = __pyx_f_2jq__jv_to_python(__pyx_v_property_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_2jq__jv_to_python(__pyx_v_property_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_python_value, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_python_value, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 107, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "jq.pyx":100
+    /* "jq.pyx":103
  *     elif kind == JV_KIND_STRING:
  *         python_value = jv_string_to_py_string(value)
  *     elif kind == JV_KIND_ARRAY:             # <<<<<<<<<<<<<<
  *         python_value = []
  *         for idx in range(0, jv_array_length(jv_copy(value))):
  */
     break;
     case JV_KIND_OBJECT:
 
-    /* "jq.pyx":106
+    /* "jq.pyx":109
  *             python_value.append(_jv_to_python(property_value))
  *     elif kind == JV_KIND_OBJECT:
  *         python_value = {}             # <<<<<<<<<<<<<<
  *         idx = jv_object_iter(value)
  *         while jv_object_iter_valid(value, idx):
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_python_value = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "jq.pyx":107
+    /* "jq.pyx":110
  *     elif kind == JV_KIND_OBJECT:
  *         python_value = {}
  *         idx = jv_object_iter(value)             # <<<<<<<<<<<<<<
  *         while jv_object_iter_valid(value, idx):
  *             property_key = jv_object_iter_key(value, idx)
  */
     __pyx_v_idx = jv_object_iter(__pyx_v_value);
 
-    /* "jq.pyx":108
+    /* "jq.pyx":111
  *         python_value = {}
  *         idx = jv_object_iter(value)
  *         while jv_object_iter_valid(value, idx):             # <<<<<<<<<<<<<<
  *             property_key = jv_object_iter_key(value, idx)
  *             property_value = jv_object_iter_value(value, idx)
  */
     while (1) {
       __pyx_t_2 = (jv_object_iter_valid(__pyx_v_value, __pyx_v_idx) != 0);
       if (!__pyx_t_2) break;
 
-      /* "jq.pyx":109
+      /* "jq.pyx":112
  *         idx = jv_object_iter(value)
  *         while jv_object_iter_valid(value, idx):
  *             property_key = jv_object_iter_key(value, idx)             # <<<<<<<<<<<<<<
  *             property_value = jv_object_iter_value(value, idx)
  *             try:
  */
       __pyx_v_property_key = jv_object_iter_key(__pyx_v_value, __pyx_v_idx);
 
-      /* "jq.pyx":110
+      /* "jq.pyx":113
  *         while jv_object_iter_valid(value, idx):
  *             property_key = jv_object_iter_key(value, idx)
  *             property_value = jv_object_iter_value(value, idx)             # <<<<<<<<<<<<<<
  *             try:
  *                 python_value[jv_string_to_py_string(property_key)] = \
  */
       __pyx_v_property_value = jv_object_iter_value(__pyx_v_value, __pyx_v_idx);
 
-      /* "jq.pyx":111
+      /* "jq.pyx":114
  *             property_key = jv_object_iter_key(value, idx)
  *             property_value = jv_object_iter_value(value, idx)
  *             try:             # <<<<<<<<<<<<<<
  *                 python_value[jv_string_to_py_string(property_key)] = \
  *                     _jv_to_python(property_value)
  */
       /*try:*/ {
 
-        /* "jq.pyx":113
+        /* "jq.pyx":116
  *             try:
  *                 python_value[jv_string_to_py_string(property_key)] = \
  *                     _jv_to_python(property_value)             # <<<<<<<<<<<<<<
  *             finally:
  *                 jv_free(property_key)
  */
-        __pyx_t_1 = __pyx_f_2jq__jv_to_python(__pyx_v_property_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L11_error)
+        __pyx_t_1 = __pyx_f_2jq__jv_to_python(__pyx_v_property_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L11_error)
         __Pyx_GOTREF(__pyx_t_1);
 
-        /* "jq.pyx":112
+        /* "jq.pyx":115
  *             property_value = jv_object_iter_value(value, idx)
  *             try:
  *                 python_value[jv_string_to_py_string(property_key)] = \             # <<<<<<<<<<<<<<
  *                     _jv_to_python(property_value)
  *             finally:
  */
-        __pyx_t_7 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_property_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L11_error)
+        __pyx_t_7 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_property_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 115, __pyx_L11_error)
         __Pyx_GOTREF(__pyx_t_7);
-        if (unlikely(PyObject_SetItem(__pyx_v_python_value, __pyx_t_7, __pyx_t_1) < 0)) __PYX_ERR(0, 112, __pyx_L11_error)
+        if (unlikely(PyObject_SetItem(__pyx_v_python_value, __pyx_t_7, __pyx_t_1) < 0)) __PYX_ERR(0, 115, __pyx_L11_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
 
-      /* "jq.pyx":115
+      /* "jq.pyx":118
  *                     _jv_to_python(property_value)
  *             finally:
  *                 jv_free(property_key)             # <<<<<<<<<<<<<<
  *             idx = jv_object_iter_next(value, idx)
  *     else:
  */
       /*finally:*/ {
@@ -2514,80 +2541,80 @@
           __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0;
           __pyx_lineno = __pyx_t_3; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_8;
           goto __pyx_L1_error;
         }
         __pyx_L12:;
       }
 
-      /* "jq.pyx":116
+      /* "jq.pyx":119
  *             finally:
  *                 jv_free(property_key)
  *             idx = jv_object_iter_next(value, idx)             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError("Invalid value kind: " + str(kind))
  */
       __pyx_v_idx = jv_object_iter_next(__pyx_v_value, __pyx_v_idx);
     }
 
-    /* "jq.pyx":105
+    /* "jq.pyx":108
  *             property_value = jv_array_get(jv_copy(value), idx)
  *             python_value.append(_jv_to_python(property_value))
  *     elif kind == JV_KIND_OBJECT:             # <<<<<<<<<<<<<<
  *         python_value = {}
  *         idx = jv_object_iter(value)
  */
     break;
     default:
 
-    /* "jq.pyx":118
+    /* "jq.pyx":121
  *             idx = jv_object_iter_next(value, idx)
  *     else:
  *         raise ValueError("Invalid value kind: " + str(kind))             # <<<<<<<<<<<<<<
  *     jv_free(value)
  *     return python_value
  */
-    __pyx_t_1 = __Pyx_PyInt_From_jv_kind(__pyx_v_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_jv_kind(__pyx_v_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_s_Invalid_value_kind, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_s_Invalid_value_kind, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 118, __pyx_L1_error)
+    __PYX_ERR(0, 121, __pyx_L1_error)
     break;
   }
 
-  /* "jq.pyx":119
+  /* "jq.pyx":122
  *     else:
  *         raise ValueError("Invalid value kind: " + str(kind))
  *     jv_free(value)             # <<<<<<<<<<<<<<
  *     return python_value
  * 
  */
   jv_free(__pyx_v_value);
 
-  /* "jq.pyx":120
+  /* "jq.pyx":123
  *         raise ValueError("Invalid value kind: " + str(kind))
  *     jv_free(value)
  *     return python_value             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_python_value);
   __pyx_r = __pyx_v_python_value;
   goto __pyx_L0;
 
-  /* "jq.pyx":69
+  /* "jq.pyx":72
  * 
  * 
  * cdef object _jv_to_python(jv value):             # <<<<<<<<<<<<<<
  *     """Unpack a jv value into a Python value"""
  *     cdef jv_kind kind = jv_get_kind(value)
  */
 
@@ -2600,63 +2627,63 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_python_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":123
+/* "jq.pyx":126
  * 
  * 
  * cdef int _is_integer(double value):             # <<<<<<<<<<<<<<
  *     cdef double integral_part
  *     cdef double fractional_part = modf(value, &integral_part)
  */
 
 static int __pyx_f_2jq__is_integer(double __pyx_v_value) {
   double __pyx_v_integral_part;
   double __pyx_v_fractional_part;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_is_integer", 0);
 
-  /* "jq.pyx":125
+  /* "jq.pyx":128
  * cdef int _is_integer(double value):
  *     cdef double integral_part
  *     cdef double fractional_part = modf(value, &integral_part)             # <<<<<<<<<<<<<<
  * 
  *     return fractional_part == 0
  */
   __pyx_v_fractional_part = modf(__pyx_v_value, (&__pyx_v_integral_part));
 
-  /* "jq.pyx":127
+  /* "jq.pyx":130
  *     cdef double fractional_part = modf(value, &integral_part)
  * 
  *     return fractional_part == 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = (__pyx_v_fractional_part == 0.0);
   goto __pyx_L0;
 
-  /* "jq.pyx":123
+  /* "jq.pyx":126
  * 
  * 
  * cdef int _is_integer(double value):             # <<<<<<<<<<<<<<
  *     cdef double integral_part
  *     cdef double fractional_part = modf(value, &integral_part)
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":130
+/* "jq.pyx":133
  * 
  * 
  * def compile(object program, args=None):             # <<<<<<<<<<<<<<
  *     cdef object program_bytes = program.encode("utf8")
  *     return _Program(program_bytes, args=args)
  */
 
@@ -2696,15 +2723,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compile") < 0)) __PYX_ERR(0, 130, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compile") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -2712,15 +2739,15 @@
       }
     }
     __pyx_v_program = values[0];
     __pyx_v_args = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compile", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 130, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compile", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 133, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq.compile", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_compile(__pyx_self, __pyx_v_program, __pyx_v_args);
 
@@ -2737,66 +2764,66 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compile", 0);
 
-  /* "jq.pyx":131
+  /* "jq.pyx":134
  * 
  * def compile(object program, args=None):
  *     cdef object program_bytes = program.encode("utf8")             # <<<<<<<<<<<<<<
  *     return _Program(program_bytes, args=args)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_program, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_program, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_program_bytes = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "jq.pyx":132
+  /* "jq.pyx":135
  * def compile(object program, args=None):
  *     cdef object program_bytes = program.encode("utf8")
  *     return _Program(program_bytes, args=args)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_program_bytes);
   __Pyx_GIVEREF(__pyx_v_program_bytes);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_program_bytes);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_args, __pyx_v_args) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__Program), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_args, __pyx_v_args) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__Program), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":130
+  /* "jq.pyx":133
  * 
  * 
  * def compile(object program, args=None):             # <<<<<<<<<<<<<<
  *     cdef object program_bytes = program.encode("utf8")
  *     return _Program(program_bytes, args=args)
  */
 
@@ -2810,15 +2837,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_program_bytes);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":138
+/* "jq.pyx":141
  * 
  * 
  * cdef jq_state* _compile(object program_bytes, object args) except NULL:             # <<<<<<<<<<<<<<
  *     cdef jq_state *jq = jq_init()
  *     cdef _ErrorStore error_store
  */
 
@@ -2848,24 +2875,24 @@
   char const *__pyx_t_16;
   PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_compile", 0);
 
-  /* "jq.pyx":139
+  /* "jq.pyx":142
  * 
  * cdef jq_state* _compile(object program_bytes, object args) except NULL:
  *     cdef jq_state *jq = jq_init()             # <<<<<<<<<<<<<<
  *     cdef _ErrorStore error_store
  *     cdef jv jv_args
  */
   __pyx_v_jq = jq_init();
 
-  /* "jq.pyx":143
+  /* "jq.pyx":146
  *     cdef jv jv_args
  *     cdef int compiled
  *     try:             # <<<<<<<<<<<<<<
  *         if not jq:
  *             raise Exception("jq_init failed")
  */
   {
@@ -2873,246 +2900,246 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "jq.pyx":144
+      /* "jq.pyx":147
  *     cdef int compiled
  *     try:
  *         if not jq:             # <<<<<<<<<<<<<<
  *             raise Exception("jq_init failed")
  * 
  */
       __pyx_t_4 = ((!(__pyx_v_jq != 0)) != 0);
       if (unlikely(__pyx_t_4)) {
 
-        /* "jq.pyx":145
+        /* "jq.pyx":148
  *     try:
  *         if not jq:
  *             raise Exception("jq_init failed")             # <<<<<<<<<<<<<<
  * 
  *         error_store = _ErrorStore()
  */
-        __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_Raise(__pyx_t_5, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __PYX_ERR(0, 145, __pyx_L3_error)
+        __PYX_ERR(0, 148, __pyx_L3_error)
 
-        /* "jq.pyx":144
+        /* "jq.pyx":147
  *     cdef int compiled
  *     try:
  *         if not jq:             # <<<<<<<<<<<<<<
  *             raise Exception("jq_init failed")
  * 
  */
       }
 
-      /* "jq.pyx":147
+      /* "jq.pyx":150
  *             raise Exception("jq_init failed")
  * 
  *         error_store = _ErrorStore()             # <<<<<<<<<<<<<<
  * 
  *         with _compilation_lock:
  */
-      __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2jq__ErrorStore)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2jq__ErrorStore)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_v_error_store = ((struct __pyx_obj_2jq__ErrorStore *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "jq.pyx":149
+      /* "jq.pyx":152
  *         error_store = _ErrorStore()
  * 
  *         with _compilation_lock:             # <<<<<<<<<<<<<<
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)
  * 
  */
       /*with:*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_compilation_lock); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L3_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_compilation_lock); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_exit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_8 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_enter); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 149, __pyx_L10_error)
+        __pyx_t_8 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_enter); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 152, __pyx_L10_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_8, function);
           }
         }
         __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 149, __pyx_L10_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L10_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*try:*/ {
           {
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
             __Pyx_XGOTREF(__pyx_t_10);
             __Pyx_XGOTREF(__pyx_t_11);
             __Pyx_XGOTREF(__pyx_t_12);
             /*try:*/ {
 
-              /* "jq.pyx":150
+              /* "jq.pyx":153
  * 
  *         with _compilation_lock:
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)             # <<<<<<<<<<<<<<
  * 
  *             if args is None:
  */
               jq_set_error_cb(__pyx_v_jq, __pyx_f_2jq__store_error, ((void *)__pyx_v_error_store));
 
-              /* "jq.pyx":152
+              /* "jq.pyx":155
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)
  * 
  *             if args is None:             # <<<<<<<<<<<<<<
  *                 compiled = jq_compile(jq, program_bytes)
  *             else:
  */
               __pyx_t_4 = (__pyx_v_args == Py_None);
               __pyx_t_13 = (__pyx_t_4 != 0);
               if (__pyx_t_13) {
 
-                /* "jq.pyx":153
+                /* "jq.pyx":156
  * 
  *             if args is None:
  *                 compiled = jq_compile(jq, program_bytes)             # <<<<<<<<<<<<<<
  *             else:
  *                 args_bytes = json.dumps(args).encode("utf-8")
  */
-                __pyx_t_14 = __Pyx_PyObject_AsString(__pyx_v_program_bytes); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L14_error)
+                __pyx_t_14 = __Pyx_PyObject_AsString(__pyx_v_program_bytes); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L14_error)
                 __pyx_v_compiled = jq_compile(__pyx_v_jq, __pyx_t_14);
 
-                /* "jq.pyx":152
+                /* "jq.pyx":155
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)
  * 
  *             if args is None:             # <<<<<<<<<<<<<<
  *                 compiled = jq_compile(jq, program_bytes)
  *             else:
  */
                 goto __pyx_L20;
               }
 
-              /* "jq.pyx":155
+              /* "jq.pyx":158
  *                 compiled = jq_compile(jq, program_bytes)
  *             else:
  *                 args_bytes = json.dumps(args).encode("utf-8")             # <<<<<<<<<<<<<<
  *                 jv_args = jv_parse(PyBytes_AsString(args_bytes))
  *                 compiled = jq_compile_args(jq, program_bytes, jv_args)
  */
               /*else*/ {
-                __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L14_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_8);
-                __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 155, __pyx_L14_error)
+                __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 158, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_9);
                 __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
                 __pyx_t_8 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
                   __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
                   if (likely(__pyx_t_8)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
                     __Pyx_INCREF(__pyx_t_8);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_9, function);
                   }
                 }
                 __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_args) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_args);
                 __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-                if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 155, __pyx_L14_error)
+                if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_7);
                 __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-                __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 155, __pyx_L14_error)
+                __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 158, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_9);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __pyx_t_7 = NULL;
                 if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
                   __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_9);
                   if (likely(__pyx_t_7)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
                     __Pyx_INCREF(__pyx_t_7);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_9, function);
                   }
                 }
                 __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_7, __pyx_kp_s_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_kp_s_utf_8);
                 __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-                if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L14_error)
+                if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_5);
                 __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
                 __pyx_v_args_bytes = __pyx_t_5;
                 __pyx_t_5 = 0;
 
-                /* "jq.pyx":156
+                /* "jq.pyx":159
  *             else:
  *                 args_bytes = json.dumps(args).encode("utf-8")
  *                 jv_args = jv_parse(PyBytes_AsString(args_bytes))             # <<<<<<<<<<<<<<
  *                 compiled = jq_compile_args(jq, program_bytes, jv_args)
  * 
  */
-                __pyx_t_15 = PyBytes_AsString(__pyx_v_args_bytes); if (unlikely(__pyx_t_15 == ((char *)NULL))) __PYX_ERR(0, 156, __pyx_L14_error)
+                __pyx_t_15 = PyBytes_AsString(__pyx_v_args_bytes); if (unlikely(__pyx_t_15 == ((char *)NULL))) __PYX_ERR(0, 159, __pyx_L14_error)
                 __pyx_v_jv_args = jv_parse(__pyx_t_15);
 
-                /* "jq.pyx":157
+                /* "jq.pyx":160
  *                 args_bytes = json.dumps(args).encode("utf-8")
  *                 jv_args = jv_parse(PyBytes_AsString(args_bytes))
  *                 compiled = jq_compile_args(jq, program_bytes, jv_args)             # <<<<<<<<<<<<<<
  * 
  *             if error_store.has_errors():
  */
-                __pyx_t_16 = __Pyx_PyObject_AsString(__pyx_v_program_bytes); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L14_error)
+                __pyx_t_16 = __Pyx_PyObject_AsString(__pyx_v_program_bytes); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L14_error)
                 __pyx_v_compiled = jq_compile_args(__pyx_v_jq, __pyx_t_16, __pyx_v_jv_args);
               }
               __pyx_L20:;
 
-              /* "jq.pyx":159
+              /* "jq.pyx":162
  *                 compiled = jq_compile_args(jq, program_bytes, jv_args)
  * 
  *             if error_store.has_errors():             # <<<<<<<<<<<<<<
  *                 raise ValueError(error_store.error_string())
  * 
  */
               __pyx_t_13 = (((struct __pyx_vtabstruct_2jq__ErrorStore *)__pyx_v_error_store->__pyx_vtab)->has_errors(__pyx_v_error_store) != 0);
               if (unlikely(__pyx_t_13)) {
 
-                /* "jq.pyx":160
+                /* "jq.pyx":163
  * 
  *             if error_store.has_errors():
  *                 raise ValueError(error_store.error_string())             # <<<<<<<<<<<<<<
  * 
  *         if not compiled:
  */
-                __pyx_t_5 = ((struct __pyx_vtabstruct_2jq__ErrorStore *)__pyx_v_error_store->__pyx_vtab)->error_string(__pyx_v_error_store); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L14_error)
+                __pyx_t_5 = ((struct __pyx_vtabstruct_2jq__ErrorStore *)__pyx_v_error_store->__pyx_vtab)->error_string(__pyx_v_error_store); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_5);
-                __pyx_t_9 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 160, __pyx_L14_error)
+                __pyx_t_9 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 163, __pyx_L14_error)
                 __Pyx_GOTREF(__pyx_t_9);
                 __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
                 __Pyx_Raise(__pyx_t_9, 0, 0, 0);
                 __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-                __PYX_ERR(0, 160, __pyx_L14_error)
+                __PYX_ERR(0, 163, __pyx_L14_error)
 
-                /* "jq.pyx":159
+                /* "jq.pyx":162
  *                 compiled = jq_compile_args(jq, program_bytes, jv_args)
  * 
  *             if error_store.has_errors():             # <<<<<<<<<<<<<<
  *                 raise ValueError(error_store.error_string())
  * 
  */
               }
 
-              /* "jq.pyx":149
+              /* "jq.pyx":152
  *         error_store = _ErrorStore()
  * 
  *         with _compilation_lock:             # <<<<<<<<<<<<<<
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)
  * 
  */
             }
@@ -3123,36 +3150,36 @@
             __pyx_L14_error:;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
             /*except:*/ {
               __Pyx_AddTraceback("jq._compile", __pyx_clineno, __pyx_lineno, __pyx_filename);
-              if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_7) < 0) __PYX_ERR(0, 149, __pyx_L16_except_error)
+              if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_7) < 0) __PYX_ERR(0, 152, __pyx_L16_except_error)
               __Pyx_GOTREF(__pyx_t_9);
               __Pyx_GOTREF(__pyx_t_5);
               __Pyx_GOTREF(__pyx_t_7);
-              __pyx_t_8 = PyTuple_Pack(3, __pyx_t_9, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 149, __pyx_L16_except_error)
+              __pyx_t_8 = PyTuple_Pack(3, __pyx_t_9, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 152, __pyx_L16_except_error)
               __Pyx_GOTREF(__pyx_t_8);
               __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-              if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 149, __pyx_L16_except_error)
+              if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 152, __pyx_L16_except_error)
               __Pyx_GOTREF(__pyx_t_17);
               __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-              if (__pyx_t_13 < 0) __PYX_ERR(0, 149, __pyx_L16_except_error)
+              if (__pyx_t_13 < 0) __PYX_ERR(0, 152, __pyx_L16_except_error)
               __pyx_t_4 = ((!(__pyx_t_13 != 0)) != 0);
               if (__pyx_t_4) {
                 __Pyx_GIVEREF(__pyx_t_9);
                 __Pyx_GIVEREF(__pyx_t_5);
                 __Pyx_XGIVEREF(__pyx_t_7);
                 __Pyx_ErrRestoreWithState(__pyx_t_9, __pyx_t_5, __pyx_t_7);
                 __pyx_t_9 = 0; __pyx_t_5 = 0; __pyx_t_7 = 0; 
-                __PYX_ERR(0, 149, __pyx_L16_except_error)
+                __PYX_ERR(0, 152, __pyx_L16_except_error)
               }
               __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
               __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
               __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
               goto __pyx_L15_exception_handled;
             }
             __pyx_L16_except_error:;
@@ -3170,62 +3197,62 @@
           }
         }
         /*finally:*/ {
           /*normal exit:*/{
             if (__pyx_t_6) {
               __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 149, __pyx_L3_error)
+              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 152, __pyx_L3_error)
               __Pyx_GOTREF(__pyx_t_12);
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             }
             goto __pyx_L13;
           }
           __pyx_L13:;
         }
         goto __pyx_L25;
         __pyx_L10_error:;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         goto __pyx_L3_error;
         __pyx_L25:;
       }
 
-      /* "jq.pyx":162
+      /* "jq.pyx":165
  *                 raise ValueError(error_store.error_string())
  * 
  *         if not compiled:             # <<<<<<<<<<<<<<
  *             raise ValueError("program was not valid")
  *     except:
  */
       __pyx_t_4 = ((!(__pyx_v_compiled != 0)) != 0);
       if (unlikely(__pyx_t_4)) {
 
-        /* "jq.pyx":163
+        /* "jq.pyx":166
  * 
  *         if not compiled:
  *             raise ValueError("program was not valid")             # <<<<<<<<<<<<<<
  *     except:
  *         jq_teardown(&jq)
  */
-        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L3_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 166, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __PYX_ERR(0, 163, __pyx_L3_error)
+        __PYX_ERR(0, 166, __pyx_L3_error)
 
-        /* "jq.pyx":162
+        /* "jq.pyx":165
  *                 raise ValueError(error_store.error_string())
  * 
  *         if not compiled:             # <<<<<<<<<<<<<<
  *             raise ValueError("program was not valid")
  *     except:
  */
       }
 
-      /* "jq.pyx":143
+      /* "jq.pyx":146
  *     cdef jv jv_args
  *     cdef int compiled
  *     try:             # <<<<<<<<<<<<<<
  *         if not jq:
  *             raise Exception("jq_init failed")
  */
     }
@@ -3235,79 +3262,79 @@
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "jq.pyx":164
+    /* "jq.pyx":167
  *         if not compiled:
  *             raise ValueError("program was not valid")
  *     except:             # <<<<<<<<<<<<<<
  *         jq_teardown(&jq)
  *         raise
  */
     /*except:*/ {
       __Pyx_AddTraceback("jq._compile", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_5, &__pyx_t_9) < 0) __PYX_ERR(0, 164, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_5, &__pyx_t_9) < 0) __PYX_ERR(0, 167, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_9);
 
-      /* "jq.pyx":165
+      /* "jq.pyx":168
  *             raise ValueError("program was not valid")
  *     except:
  *         jq_teardown(&jq)             # <<<<<<<<<<<<<<
  *         raise
  *     # TODO: unset error callback?
  */
       jq_teardown((&__pyx_v_jq));
 
-      /* "jq.pyx":166
+      /* "jq.pyx":169
  *     except:
  *         jq_teardown(&jq)
  *         raise             # <<<<<<<<<<<<<<
  *     # TODO: unset error callback?
  * 
  */
       __Pyx_GIVEREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_9);
       __Pyx_ErrRestoreWithState(__pyx_t_7, __pyx_t_5, __pyx_t_9);
       __pyx_t_7 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0; 
-      __PYX_ERR(0, 166, __pyx_L5_except_error)
+      __PYX_ERR(0, 169, __pyx_L5_except_error)
     }
     __pyx_L5_except_error:;
 
-    /* "jq.pyx":143
+    /* "jq.pyx":146
  *     cdef jv jv_args
  *     cdef int compiled
  *     try:             # <<<<<<<<<<<<<<
  *         if not jq:
  *             raise Exception("jq_init failed")
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "jq.pyx":169
+  /* "jq.pyx":172
  *     # TODO: unset error callback?
  * 
  *     return jq             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_jq;
   goto __pyx_L0;
 
-  /* "jq.pyx":138
+  /* "jq.pyx":141
  * 
  * 
  * cdef jq_state* _compile(object program_bytes, object args) except NULL:             # <<<<<<<<<<<<<<
  *     cdef jq_state *jq = jq_init()
  *     cdef _ErrorStore error_store
  */
 
@@ -3322,15 +3349,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_error_store);
   __Pyx_XDECREF(__pyx_v_args_bytes);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":172
+/* "jq.pyx":175
  * 
  * 
  * cdef void _store_error(void* store_ptr, jv error):             # <<<<<<<<<<<<<<
  *     # TODO: handle errors not of JV_KIND_STRING
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr
  */
 
@@ -3340,67 +3367,67 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_store_error", 0);
 
-  /* "jq.pyx":174
+  /* "jq.pyx":177
  * cdef void _store_error(void* store_ptr, jv error):
  *     # TODO: handle errors not of JV_KIND_STRING
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr             # <<<<<<<<<<<<<<
  *     if jv_get_kind(error) == JV_KIND_STRING:
  *         store.store_error(jv_string_to_py_string(error))
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_store_ptr);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_store = ((struct __pyx_obj_2jq__ErrorStore *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "jq.pyx":175
+  /* "jq.pyx":178
  *     # TODO: handle errors not of JV_KIND_STRING
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr
  *     if jv_get_kind(error) == JV_KIND_STRING:             # <<<<<<<<<<<<<<
  *         store.store_error(jv_string_to_py_string(error))
  * 
  */
   __pyx_t_2 = ((jv_get_kind(__pyx_v_error) == JV_KIND_STRING) != 0);
   if (__pyx_t_2) {
 
-    /* "jq.pyx":176
+    /* "jq.pyx":179
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr
  *     if jv_get_kind(error) == JV_KIND_STRING:
  *         store.store_error(jv_string_to_py_string(error))             # <<<<<<<<<<<<<<
  * 
  *     jv_free(error)
  */
-    __pyx_t_1 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     ((struct __pyx_vtabstruct_2jq__ErrorStore *)__pyx_v_store->__pyx_vtab)->store_error(__pyx_v_store, ((PyObject*)__pyx_t_1));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "jq.pyx":175
+    /* "jq.pyx":178
  *     # TODO: handle errors not of JV_KIND_STRING
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr
  *     if jv_get_kind(error) == JV_KIND_STRING:             # <<<<<<<<<<<<<<
  *         store.store_error(jv_string_to_py_string(error))
  * 
  */
   }
 
-  /* "jq.pyx":178
+  /* "jq.pyx":181
  *         store.store_error(jv_string_to_py_string(error))
  * 
  *     jv_free(error)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   jv_free(__pyx_v_error);
 
-  /* "jq.pyx":172
+  /* "jq.pyx":175
  * 
  * 
  * cdef void _store_error(void* store_ptr, jv error):             # <<<<<<<<<<<<<<
  *     # TODO: handle errors not of JV_KIND_STRING
  *     cdef _ErrorStore store = <_ErrorStore>store_ptr
  */
 
@@ -3410,15 +3437,15 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_WriteUnraisable("jq._store_error", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_store);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "jq.pyx":184
+/* "jq.pyx":187
  *     cdef object _errors
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.clear()
  * 
  */
 
@@ -3439,38 +3466,38 @@
 }
 
 static int __pyx_pf_2jq_11_ErrorStore___cinit__(struct __pyx_obj_2jq__ErrorStore *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "jq.pyx":185
+  /* "jq.pyx":188
  * 
  *     def __cinit__(self):
  *         self.clear()             # <<<<<<<<<<<<<<
  * 
  *     cdef int has_errors(self):
  */
   ((struct __pyx_vtabstruct_2jq__ErrorStore *)__pyx_v_self->__pyx_vtab)->clear(__pyx_v_self);
 
-  /* "jq.pyx":184
+  /* "jq.pyx":187
  *     cdef object _errors
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.clear()
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":187
+/* "jq.pyx":190
  *         self.clear()
  * 
  *     cdef int has_errors(self):             # <<<<<<<<<<<<<<
  *         return len(self._errors)
  * 
  */
 
@@ -3480,29 +3507,29 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("has_errors", 0);
 
-  /* "jq.pyx":188
+  /* "jq.pyx":191
  * 
  *     cdef int has_errors(self):
  *         return len(self._errors)             # <<<<<<<<<<<<<<
  * 
  *     cdef object error_string(self):
  */
   __pyx_t_1 = __pyx_v_self->_errors;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "jq.pyx":187
+  /* "jq.pyx":190
  *         self.clear()
  * 
  *     cdef int has_errors(self):             # <<<<<<<<<<<<<<
  *         return len(self._errors)
  * 
  */
 
@@ -3512,15 +3539,15 @@
   __Pyx_WriteUnraisable("jq._ErrorStore.has_errors", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":190
+/* "jq.pyx":193
  *         return len(self._errors)
  * 
  *     cdef object error_string(self):             # <<<<<<<<<<<<<<
  *         return "\n".join(self._errors)
  * 
  */
 
@@ -3530,32 +3557,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("error_string", 0);
 
-  /* "jq.pyx":191
+  /* "jq.pyx":194
  * 
  *     cdef object error_string(self):
  *         return "\n".join(self._errors)             # <<<<<<<<<<<<<<
  * 
  *     cdef void store_error(self, unicode error):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->_errors;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":190
+  /* "jq.pyx":193
  *         return len(self._errors)
  * 
  *     cdef object error_string(self):             # <<<<<<<<<<<<<<
  *         return "\n".join(self._errors)
  * 
  */
 
@@ -3567,15 +3594,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":193
+/* "jq.pyx":196
  *         return "\n".join(self._errors)
  * 
  *     cdef void store_error(self, unicode error):             # <<<<<<<<<<<<<<
  *         self._errors.append(error)
  * 
  */
 
@@ -3583,24 +3610,24 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("store_error", 0);
 
-  /* "jq.pyx":194
+  /* "jq.pyx":197
  * 
  *     cdef void store_error(self, unicode error):
  *         self._errors.append(error)             # <<<<<<<<<<<<<<
  * 
  *     cdef void clear(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_Append(__pyx_v_self->_errors, __pyx_v_error); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Append(__pyx_v_self->_errors, __pyx_v_error); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
 
-  /* "jq.pyx":193
+  /* "jq.pyx":196
  *         return "\n".join(self._errors)
  * 
  *     cdef void store_error(self, unicode error):             # <<<<<<<<<<<<<<
  *         self._errors.append(error)
  * 
  */
 
@@ -3608,15 +3635,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("jq._ErrorStore.store_error", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "jq.pyx":196
+/* "jq.pyx":199
  *         self._errors.append(error)
  * 
  *     cdef void clear(self):             # <<<<<<<<<<<<<<
  *         self._errors = []
  * 
  */
 
@@ -3624,30 +3651,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
 
-  /* "jq.pyx":197
+  /* "jq.pyx":200
  * 
  *     cdef void clear(self):
  *         self._errors = []             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_errors);
   __Pyx_DECREF(__pyx_v_self->_errors);
   __pyx_v_self->_errors = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "jq.pyx":196
+  /* "jq.pyx":199
  *         self._errors.append(error)
  * 
  *     cdef void clear(self):             # <<<<<<<<<<<<<<
  *         self._errors = []
  * 
  */
 
@@ -3769,15 +3796,15 @@
   __Pyx_AddTraceback("jq._ErrorStore.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":212
+/* "jq.pyx":215
  *     cdef object _lock
  * 
  *     def __cinit__(self, program_bytes, args):             # <<<<<<<<<<<<<<
  *         self._program_bytes = program_bytes
  *         self._args = args
  */
 
@@ -3811,32 +3838,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_program_bytes)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 212, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 215, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 212, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 215, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_program_bytes = values[0];
     __pyx_v_args = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 212, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 215, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._JqStatePool.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_12_JqStatePool___cinit__(((struct __pyx_obj_2jq__JqStatePool *)__pyx_v_self), __pyx_v_program_bytes, __pyx_v_args);
 
@@ -3853,90 +3880,90 @@
   jq_state *__pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "jq.pyx":213
+  /* "jq.pyx":216
  * 
  *     def __cinit__(self, program_bytes, args):
  *         self._program_bytes = program_bytes             # <<<<<<<<<<<<<<
  *         self._args = args
  *         self._jq_state = _compile(self._program_bytes, args=self._args)
  */
   __Pyx_INCREF(__pyx_v_program_bytes);
   __Pyx_GIVEREF(__pyx_v_program_bytes);
   __Pyx_GOTREF(__pyx_v_self->_program_bytes);
   __Pyx_DECREF(__pyx_v_self->_program_bytes);
   __pyx_v_self->_program_bytes = __pyx_v_program_bytes;
 
-  /* "jq.pyx":214
+  /* "jq.pyx":217
  *     def __cinit__(self, program_bytes, args):
  *         self._program_bytes = program_bytes
  *         self._args = args             # <<<<<<<<<<<<<<
  *         self._jq_state = _compile(self._program_bytes, args=self._args)
  *         self._lock = threading.Lock()
  */
   __Pyx_INCREF(__pyx_v_args);
   __Pyx_GIVEREF(__pyx_v_args);
   __Pyx_GOTREF(__pyx_v_self->_args);
   __Pyx_DECREF(__pyx_v_self->_args);
   __pyx_v_self->_args = __pyx_v_args;
 
-  /* "jq.pyx":215
+  /* "jq.pyx":218
  *         self._program_bytes = program_bytes
  *         self._args = args
  *         self._jq_state = _compile(self._program_bytes, args=self._args)             # <<<<<<<<<<<<<<
  *         self._lock = threading.Lock()
  * 
  */
   __pyx_t_1 = __pyx_v_self->_program_bytes;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __pyx_v_self->_args;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_2jq__compile(__pyx_t_1, __pyx_t_2); if (unlikely(__pyx_t_3 == ((jq_state *)NULL))) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_2jq__compile(__pyx_t_1, __pyx_t_2); if (unlikely(__pyx_t_3 == ((jq_state *)NULL))) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->_jq_state = __pyx_t_3;
 
-  /* "jq.pyx":216
+  /* "jq.pyx":219
  *         self._args = args
  *         self._jq_state = _compile(self._program_bytes, args=self._args)
  *         self._lock = threading.Lock()             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_threading); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_threading); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Lock); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Lock); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_lock);
   __Pyx_DECREF(__pyx_v_self->_lock);
   __pyx_v_self->_lock = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "jq.pyx":212
+  /* "jq.pyx":215
  *     cdef object _lock
  * 
  *     def __cinit__(self, program_bytes, args):             # <<<<<<<<<<<<<<
  *         self._program_bytes = program_bytes
  *         self._args = args
  */
 
@@ -3950,15 +3977,15 @@
   __Pyx_AddTraceback("jq._JqStatePool.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":218
+/* "jq.pyx":221
  *         self._lock = threading.Lock()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         jq_teardown(&self._jq_state)
  * 
  */
 
@@ -3973,36 +4000,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_2jq_12_JqStatePool_2__dealloc__(struct __pyx_obj_2jq__JqStatePool *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "jq.pyx":219
+  /* "jq.pyx":222
  * 
  *     def __dealloc__(self):
  *         jq_teardown(&self._jq_state)             # <<<<<<<<<<<<<<
  * 
  *     cdef jq_state* acquire(self):
  */
   jq_teardown((&__pyx_v_self->_jq_state));
 
-  /* "jq.pyx":218
+  /* "jq.pyx":221
  *         self._lock = threading.Lock()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         jq_teardown(&self._jq_state)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "jq.pyx":221
+/* "jq.pyx":224
  *         jq_teardown(&self._jq_state)
  * 
  *     cdef jq_state* acquire(self):             # <<<<<<<<<<<<<<
  *         with self._lock:
  *             if self._jq_state == NULL:
  */
 
@@ -4023,155 +4050,155 @@
   PyObject *__pyx_t_11 = NULL;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("acquire", 0);
 
-  /* "jq.pyx":222
+  /* "jq.pyx":225
  * 
  *     cdef jq_state* acquire(self):
  *         with self._lock:             # <<<<<<<<<<<<<<
  *             if self._jq_state == NULL:
  *                 return _compile(self._program_bytes, args=self._args)
  */
   /*with:*/ {
-    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         /*try:*/ {
 
-          /* "jq.pyx":223
+          /* "jq.pyx":226
  *     cdef jq_state* acquire(self):
  *         with self._lock:
  *             if self._jq_state == NULL:             # <<<<<<<<<<<<<<
  *                 return _compile(self._program_bytes, args=self._args)
  *             else:
  */
           __pyx_t_8 = ((__pyx_v_self->_jq_state == NULL) != 0);
           if (__pyx_t_8) {
 
-            /* "jq.pyx":224
+            /* "jq.pyx":227
  *         with self._lock:
  *             if self._jq_state == NULL:
  *                 return _compile(self._program_bytes, args=self._args)             # <<<<<<<<<<<<<<
  *             else:
  *                 state = self._jq_state
  */
             __pyx_t_2 = __pyx_v_self->_program_bytes;
             __Pyx_INCREF(__pyx_t_2);
             __pyx_t_3 = __pyx_v_self->_args;
             __Pyx_INCREF(__pyx_t_3);
-            __pyx_t_9 = __pyx_f_2jq__compile(__pyx_t_2, __pyx_t_3); if (unlikely(__pyx_t_9 == ((jq_state *)NULL))) __PYX_ERR(0, 224, __pyx_L7_error)
+            __pyx_t_9 = __pyx_f_2jq__compile(__pyx_t_2, __pyx_t_3); if (unlikely(__pyx_t_9 == ((jq_state *)NULL))) __PYX_ERR(0, 227, __pyx_L7_error)
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __pyx_r = __pyx_t_9;
             goto __pyx_L11_try_return;
 
-            /* "jq.pyx":223
+            /* "jq.pyx":226
  *     cdef jq_state* acquire(self):
  *         with self._lock:
  *             if self._jq_state == NULL:             # <<<<<<<<<<<<<<
  *                 return _compile(self._program_bytes, args=self._args)
  *             else:
  */
           }
 
-          /* "jq.pyx":226
+          /* "jq.pyx":229
  *                 return _compile(self._program_bytes, args=self._args)
  *             else:
  *                 state = self._jq_state             # <<<<<<<<<<<<<<
  *                 self._jq_state = NULL
  *                 return state
  */
           /*else*/ {
             __pyx_t_9 = __pyx_v_self->_jq_state;
             __pyx_v_state = __pyx_t_9;
 
-            /* "jq.pyx":227
+            /* "jq.pyx":230
  *             else:
  *                 state = self._jq_state
  *                 self._jq_state = NULL             # <<<<<<<<<<<<<<
  *                 return state
  * 
  */
             __pyx_v_self->_jq_state = NULL;
 
-            /* "jq.pyx":228
+            /* "jq.pyx":231
  *                 state = self._jq_state
  *                 self._jq_state = NULL
  *                 return state             # <<<<<<<<<<<<<<
  * 
  *     cdef void release(self, jq_state* state):
  */
             __pyx_r = __pyx_v_state;
             goto __pyx_L11_try_return;
           }
 
-          /* "jq.pyx":222
+          /* "jq.pyx":225
  * 
  *     cdef jq_state* acquire(self):
  *         with self._lock:             # <<<<<<<<<<<<<<
  *             if self._jq_state == NULL:
  *                 return _compile(self._program_bytes, args=self._args)
  */
         }
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("jq._JqStatePool.acquire", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 222, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 225, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_10 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 222, __pyx_L9_except_error)
+          __pyx_t_10 = PyTuple_Pack(3, __pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 225, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 222, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_8 < 0) __PYX_ERR(0, 222, __pyx_L9_except_error)
+          if (__pyx_t_8 < 0) __PYX_ERR(0, 225, __pyx_L9_except_error)
           __pyx_t_12 = ((!(__pyx_t_8 != 0)) != 0);
           if (__pyx_t_12) {
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_4);
             __Pyx_ErrRestoreWithState(__pyx_t_3, __pyx_t_2, __pyx_t_4);
             __pyx_t_3 = 0; __pyx_t_2 = 0; __pyx_t_4 = 0; 
-            __PYX_ERR(0, 222, __pyx_L9_except_error)
+            __PYX_ERR(0, 225, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -4194,26 +4221,26 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_1) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_9 = __pyx_r;
         if (__pyx_t_1) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __pyx_r = __pyx_t_9;
         goto __pyx_L0;
       }
       __pyx_L6:;
@@ -4221,15 +4248,15 @@
     goto __pyx_L17;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L1_error;
     __pyx_L17:;
   }
 
-  /* "jq.pyx":221
+  /* "jq.pyx":224
  *         jq_teardown(&self._jq_state)
  * 
  *     cdef jq_state* acquire(self):             # <<<<<<<<<<<<<<
  *         with self._lock:
  *             if self._jq_state == NULL:
  */
 
@@ -4244,15 +4271,15 @@
   __Pyx_WriteUnraisable("jq._JqStatePool.acquire", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":230
+/* "jq.pyx":233
  *                 return state
  * 
  *     cdef void release(self, jq_state* state):             # <<<<<<<<<<<<<<
  *         with self._lock:
  *             if self._jq_state == NULL:
  */
 
@@ -4267,119 +4294,119 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("release", 0);
 
-  /* "jq.pyx":231
+  /* "jq.pyx":234
  * 
  *     cdef void release(self, jq_state* state):
  *         with self._lock:             # <<<<<<<<<<<<<<
  *             if self._jq_state == NULL:
  *                 self._jq_state = state
  */
   /*with:*/ {
-    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_exit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_v_self->_lock, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
         (void)__pyx_t_5; (void)__pyx_t_6; (void)__pyx_t_7; /* mark used */
         /*try:*/ {
 
-          /* "jq.pyx":232
+          /* "jq.pyx":235
  *     cdef void release(self, jq_state* state):
  *         with self._lock:
  *             if self._jq_state == NULL:             # <<<<<<<<<<<<<<
  *                 self._jq_state = state
  *             else:
  */
           __pyx_t_8 = ((__pyx_v_self->_jq_state == NULL) != 0);
           if (__pyx_t_8) {
 
-            /* "jq.pyx":233
+            /* "jq.pyx":236
  *         with self._lock:
  *             if self._jq_state == NULL:
  *                 self._jq_state = state             # <<<<<<<<<<<<<<
  *             else:
  *                 jq_teardown(&state)
  */
             __pyx_v_self->_jq_state = __pyx_v_state;
 
-            /* "jq.pyx":232
+            /* "jq.pyx":235
  *     cdef void release(self, jq_state* state):
  *         with self._lock:
  *             if self._jq_state == NULL:             # <<<<<<<<<<<<<<
  *                 self._jq_state = state
  *             else:
  */
             goto __pyx_L13;
           }
 
-          /* "jq.pyx":235
+          /* "jq.pyx":238
  *                 self._jq_state = state
  *             else:
  *                 jq_teardown(&state)             # <<<<<<<<<<<<<<
  * 
  * 
  */
           /*else*/ {
             jq_teardown((&__pyx_v_state));
           }
           __pyx_L13:;
 
-          /* "jq.pyx":231
+          /* "jq.pyx":234
  * 
  *     cdef void release(self, jq_state* state):
  *         with self._lock:             # <<<<<<<<<<<<<<
  *             if self._jq_state == NULL:
  *                 self._jq_state = state
  */
         }
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_1) {
           __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 231, __pyx_L1_error)
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 234, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L14;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L1_error;
     __pyx_L14:;
   }
 
-  /* "jq.pyx":230
+  /* "jq.pyx":233
  *                 return state
  * 
  *     cdef void release(self, jq_state* state):             # <<<<<<<<<<<<<<
  *         with self._lock:
  *             if self._jq_state == NULL:
  */
 
@@ -4503,15 +4530,15 @@
   __Pyx_AddTraceback("jq._JqStatePool.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":242
+/* "jq.pyx":245
  *     cdef _JqStatePool _jq_state_pool
  * 
  *     def __cinit__(self, program_bytes, args):             # <<<<<<<<<<<<<<
  *         self._program_bytes = program_bytes
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
  */
 
@@ -4545,32 +4572,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_program_bytes)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 242, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 245, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 242, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 245, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_program_bytes = values[0];
     __pyx_v_args = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 242, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 245, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._Program.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_8_Program___cinit__(((struct __pyx_obj_2jq__Program *)__pyx_v_self), __pyx_v_program_bytes, __pyx_v_args);
 
@@ -4586,53 +4613,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "jq.pyx":243
+  /* "jq.pyx":246
  * 
  *     def __cinit__(self, program_bytes, args):
  *         self._program_bytes = program_bytes             # <<<<<<<<<<<<<<
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
  * 
  */
   __Pyx_INCREF(__pyx_v_program_bytes);
   __Pyx_GIVEREF(__pyx_v_program_bytes);
   __Pyx_GOTREF(__pyx_v_self->_program_bytes);
   __Pyx_DECREF(__pyx_v_self->_program_bytes);
   __pyx_v_self->_program_bytes = __pyx_v_program_bytes;
 
-  /* "jq.pyx":244
+  /* "jq.pyx":247
  *     def __cinit__(self, program_bytes, args):
  *         self._program_bytes = program_bytes
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)             # <<<<<<<<<<<<<<
  * 
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_program_bytes);
   __Pyx_GIVEREF(__pyx_v_program_bytes);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_program_bytes);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_args, __pyx_v_args) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__JqStatePool), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_args, __pyx_v_args) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__JqStatePool), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_jq_state_pool);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   __pyx_v_self->_jq_state_pool = ((struct __pyx_obj_2jq__JqStatePool *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "jq.pyx":242
+  /* "jq.pyx":245
  *     cdef _JqStatePool _jq_state_pool
  * 
  *     def __cinit__(self, program_bytes, args):             # <<<<<<<<<<<<<<
  *         self._program_bytes = program_bytes
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
  */
 
@@ -4646,15 +4673,15 @@
   __Pyx_AddTraceback("jq._Program.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":246
+/* "jq.pyx":249
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
  * 
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):
  *             raise ValueError("Either the value or text argument should be set")
  */
 
@@ -4696,15 +4723,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "input") < 0)) __PYX_ERR(0, 246, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "input") < 0)) __PYX_ERR(0, 249, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -4713,188 +4740,723 @@
       }
     }
     __pyx_v_value = values[0];
     __pyx_v_text = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("input", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 246, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("input", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 249, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._Program.input", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_8_Program_2input(((struct __pyx_obj_2jq__Program *)__pyx_v_self), __pyx_v_value, __pyx_v_text);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_2jq_8_Program_2input(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text) {
-  PyObject *__pyx_v_string_input = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("input", 0);
 
-  /* "jq.pyx":247
+  /* "jq.pyx":250
  * 
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):             # <<<<<<<<<<<<<<
  *             raise ValueError("Either the value or text argument should be set")
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)
+ * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_v_value == __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_text == __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = ((__pyx_t_2 == __pyx_t_3) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "jq.pyx":248
+    /* "jq.pyx":251
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):
  *             raise ValueError("Either the value or text argument should be set")             # <<<<<<<<<<<<<<
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)
  * 
+ *         if text is not _NO_VALUE:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 248, __pyx_L1_error)
+    __PYX_ERR(0, 251, __pyx_L1_error)
 
-    /* "jq.pyx":247
+    /* "jq.pyx":250
  * 
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):             # <<<<<<<<<<<<<<
  *             raise ValueError("Either the value or text argument should be set")
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)
+ * 
  */
   }
 
+  /* "jq.pyx":253
+ *             raise ValueError("Either the value or text argument should be set")
+ * 
+ *         if text is not _NO_VALUE:             # <<<<<<<<<<<<<<
+ *             return self.input_text(text)
+ *         else:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = (__pyx_v_text != __pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_4 != 0);
+  if (__pyx_t_3) {
+
+    /* "jq.pyx":254
+ * 
+ *         if text is not _NO_VALUE:
+ *             return self.input_text(text)             # <<<<<<<<<<<<<<
+ *         else:
+ *             return self.input_value(value)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_text) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_text);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+
+    /* "jq.pyx":253
+ *             raise ValueError("Either the value or text argument should be set")
+ * 
+ *         if text is not _NO_VALUE:             # <<<<<<<<<<<<<<
+ *             return self.input_text(text)
+ *         else:
+ */
+  }
+
+  /* "jq.pyx":256
+ *             return self.input_text(text)
+ *         else:
+ *             return self.input_value(value)             # <<<<<<<<<<<<<<
+ * 
+ *     def input_value(self, value):
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input_value); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+  }
+
   /* "jq.pyx":249
+ *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
+ * 
+ *     def input(self, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):
  *             raise ValueError("Either the value or text argument should be set")
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)             # <<<<<<<<<<<<<<
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("jq._Program.input", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "jq.pyx":258
+ *             return self.input_value(value)
+ * 
+ *     def input_value(self, value):             # <<<<<<<<<<<<<<
+ *         return self.input_text(json.dumps(value))
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_2jq_8_Program_5input_value(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_5input_value(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("input_value (wrapper)", 0);
+  __pyx_r = __pyx_pf_2jq_8_Program_4input_value(((struct __pyx_obj_2jq__Program *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_2jq_8_Program_4input_value(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("input_value", 0);
+
+  /* "jq.pyx":259
+ * 
+ *     def input_value(self, value):
+ *         return self.input_text(json.dumps(value))             # <<<<<<<<<<<<<<
  * 
- *         return _ProgramWithInput(self._jq_state_pool, string_input.encode("utf8"))
+ *     def input_values(self, values):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_json); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dumps); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = (__pyx_v_text != __pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+    }
+  }
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_value);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if ((__pyx_t_4 != 0)) {
-    __Pyx_INCREF(__pyx_v_text);
-    __pyx_t_1 = __pyx_v_text;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "jq.pyx":258
+ *             return self.input_value(value)
+ * 
+ *     def input_value(self, value):             # <<<<<<<<<<<<<<
+ *         return self.input_text(json.dumps(value))
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("jq._Program.input_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "jq.pyx":261
+ *         return self.input_text(json.dumps(value))
+ * 
+ *     def input_values(self, values):             # <<<<<<<<<<<<<<
+ *         fileobj = io.StringIO()
+ *         for value in values:
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_2jq_8_Program_7input_values(PyObject *__pyx_v_self, PyObject *__pyx_v_values); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_7input_values(PyObject *__pyx_v_self, PyObject *__pyx_v_values) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("input_values (wrapper)", 0);
+  __pyx_r = __pyx_pf_2jq_8_Program_6input_values(((struct __pyx_obj_2jq__Program *)__pyx_v_self), ((PyObject *)__pyx_v_values));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_2jq_8_Program_6input_values(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_values) {
+  PyObject *__pyx_v_fileobj = NULL;
+  PyObject *__pyx_v_value = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  PyObject *(*__pyx_t_5)(PyObject *);
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("input_values", 0);
+
+  /* "jq.pyx":262
+ * 
+ *     def input_values(self, values):
+ *         fileobj = io.StringIO()             # <<<<<<<<<<<<<<
+ *         for value in values:
+ *             json.dump(value, fileobj)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_io); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_StringIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_fileobj = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "jq.pyx":263
+ *     def input_values(self, values):
+ *         fileobj = io.StringIO()
+ *         for value in values:             # <<<<<<<<<<<<<<
+ *             json.dump(value, fileobj)
+ *             fileobj.write("\n")
+ */
+  if (likely(PyList_CheckExact(__pyx_v_values)) || PyTuple_CheckExact(__pyx_v_values)) {
+    __pyx_t_1 = __pyx_v_values; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+    __pyx_t_5 = NULL;
   } else {
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_5)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      } else {
+        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
+    } else {
+      __pyx_t_3 = __pyx_t_5(__pyx_t_1);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 263, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "jq.pyx":264
+ *         fileobj = io.StringIO()
+ *         for value in values:
+ *             json.dump(value, fileobj)             # <<<<<<<<<<<<<<
+ *             fileobj.write("\n")
+ *         return self.input_text(fileobj.getvalue())
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dump); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 249, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = NULL;
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_7 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_6)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_v_fileobj};
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_GOTREF(__pyx_t_3);
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_value, __pyx_v_fileobj};
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_GOTREF(__pyx_t_3);
+    } else
+    #endif
+    {
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      if (__pyx_t_2) {
+        __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_2); __pyx_t_2 = NULL;
+      }
+      __Pyx_INCREF(__pyx_v_value);
+      __Pyx_GIVEREF(__pyx_v_value);
+      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_value);
+      __Pyx_INCREF(__pyx_v_fileobj);
+      __Pyx_GIVEREF(__pyx_v_fileobj);
+      PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_fileobj);
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "jq.pyx":265
+ *         for value in values:
+ *             json.dump(value, fileobj)
+ *             fileobj.write("\n")             # <<<<<<<<<<<<<<
+ *         return self.input_text(fileobj.getvalue())
+ * 
+ */
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_fileobj, __pyx_n_s_write); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
-    __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_value);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_1 = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_8, __pyx_kp_s__5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_s__5);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "jq.pyx":263
+ *     def input_values(self, values):
+ *         fileobj = io.StringIO()
+ *         for value in values:             # <<<<<<<<<<<<<<
+ *             json.dump(value, fileobj)
+ *             fileobj.write("\n")
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "jq.pyx":266
+ *             json.dump(value, fileobj)
+ *             fileobj.write("\n")
+ *         return self.input_text(fileobj.getvalue())             # <<<<<<<<<<<<<<
+ * 
+ *     def input_text(self, text, *, slurp=False):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_fileobj, __pyx_n_s_getvalue); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_8, function);
+    }
+  }
+  __pyx_t_6 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
   }
-  __pyx_v_string_input = __pyx_t_1;
+  __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
+  goto __pyx_L0;
 
-  /* "jq.pyx":251
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)
+  /* "jq.pyx":261
+ *         return self.input_text(json.dumps(value))
+ * 
+ *     def input_values(self, values):             # <<<<<<<<<<<<<<
+ *         fileobj = io.StringIO()
+ *         for value in values:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("jq._Program.input_values", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_fileobj);
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "jq.pyx":268
+ *         return self.input_text(fileobj.getvalue())
+ * 
+ *     def input_text(self, text, *, slurp=False):             # <<<<<<<<<<<<<<
+ *         return _ProgramWithInput(self._jq_state_pool, text.encode("utf8"), slurp=slurp)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_2jq_8_Program_9input_text(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_9input_text(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_text = 0;
+  PyObject *__pyx_v_slurp = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("input_text (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text,&__pyx_n_s_slurp,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)Py_False);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (kw_args == 1) {
+        const Py_ssize_t index = 1;
+        PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
+        if (value) { values[index] = value; kw_args--; }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "input_text") < 0)) __PYX_ERR(0, 268, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+    }
+    __pyx_v_text = values[0];
+    __pyx_v_slurp = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("input_text", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 268, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("jq._Program.input_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_2jq_8_Program_8input_text(((struct __pyx_obj_2jq__Program *)__pyx_v_self), __pyx_v_text, __pyx_v_slurp);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_2jq_8_Program_8input_text(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_slurp) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("input_text", 0);
+
+  /* "jq.pyx":269
  * 
- *         return _ProgramWithInput(self._jq_state_pool, string_input.encode("utf8"))             # <<<<<<<<<<<<<<
+ *     def input_text(self, text, *, slurp=False):
+ *         return _ProgramWithInput(self._jq_state_pool, text.encode("utf8"), slurp=slurp)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_string_input, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 251, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_7);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
-  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_utf8);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 251, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self->_jq_state_pool));
-  PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_self->_jq_state_pool));
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_self->_jq_state_pool));
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__ProgramWithInput), __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_slurp, __pyx_v_slurp) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__ProgramWithInput), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":246
- *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
+  /* "jq.pyx":268
+ *         return self.input_text(fileobj.getvalue())
+ * 
+ *     def input_text(self, text, *, slurp=False):             # <<<<<<<<<<<<<<
+ *         return _ProgramWithInput(self._jq_state_pool, text.encode("utf8"), slurp=slurp)
  * 
- *     def input(self, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
- *         if (value is _NO_VALUE) == (text is _NO_VALUE):
- *             raise ValueError("Either the value or text argument should be set")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("jq._Program.input", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("jq._Program.input_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_string_input);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":254
+/* "jq.pyx":272
  * 
  *     @property
  *     def program_string(self):             # <<<<<<<<<<<<<<
  *         return self._program_bytes.decode("utf8")
  * 
  */
 
@@ -4918,44 +5480,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "jq.pyx":255
+  /* "jq.pyx":273
  *     @property
  *     def program_string(self):
  *         return self._program_bytes.decode("utf8")             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_program_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_program_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":254
+  /* "jq.pyx":272
  * 
  *     @property
  *     def program_string(self):             # <<<<<<<<<<<<<<
  *         return self._program_bytes.decode("utf8")
  * 
  */
 
@@ -4968,80 +5530,80 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":257
+/* "jq.pyx":275
  *         return self._program_bytes.decode("utf8")
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "jq.compile({!r})".format(self.program_string)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2jq_8_Program_5__repr__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_2jq_8_Program_5__repr__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_2jq_8_Program_11__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_11__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_2jq_8_Program_4__repr__(((struct __pyx_obj_2jq__Program *)__pyx_v_self));
+  __pyx_r = __pyx_pf_2jq_8_Program_10__repr__(((struct __pyx_obj_2jq__Program *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2jq_8_Program_4__repr__(struct __pyx_obj_2jq__Program *__pyx_v_self) {
+static PyObject *__pyx_pf_2jq_8_Program_10__repr__(struct __pyx_obj_2jq__Program *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "jq.pyx":258
+  /* "jq.pyx":276
  * 
  *     def __repr__(self):
  *         return "jq.compile({!r})".format(self.program_string)             # <<<<<<<<<<<<<<
  * 
  *     # Support the 0.1.x API for backwards compatibility
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_jq_compile_r, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_jq_compile_r, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_program_string); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_program_string); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":257
+  /* "jq.pyx":275
  *         return self._program_bytes.decode("utf8")
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "jq.compile({!r})".format(self.program_string)
  * 
  */
 
@@ -5055,25 +5617,25 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":261
+/* "jq.pyx":279
  * 
  *     # Support the 0.1.x API for backwards compatibility
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):             # <<<<<<<<<<<<<<
  *         program_with_input = self.input(value, text=text)
  *         if text_output:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2jq_8_Program_7transform(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_2jq_8_Program_7transform(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_2jq_8_Program_13transform(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_13transform(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_value = 0;
   PyObject *__pyx_v_text = 0;
   PyObject *__pyx_v_text_output = 0;
   PyObject *__pyx_v_multiple_output = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5125,15 +5687,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_multiple_output);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "transform") < 0)) __PYX_ERR(0, 261, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "transform") < 0)) __PYX_ERR(0, 279, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -5148,194 +5710,194 @@
     __pyx_v_value = values[0];
     __pyx_v_text = values[1];
     __pyx_v_text_output = values[2];
     __pyx_v_multiple_output = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("transform", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 261, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("transform", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 279, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._Program.transform", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2jq_8_Program_6transform(((struct __pyx_obj_2jq__Program *)__pyx_v_self), __pyx_v_value, __pyx_v_text, __pyx_v_text_output, __pyx_v_multiple_output);
+  __pyx_r = __pyx_pf_2jq_8_Program_12transform(((struct __pyx_obj_2jq__Program *)__pyx_v_self), __pyx_v_value, __pyx_v_text, __pyx_v_text_output, __pyx_v_multiple_output);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2jq_8_Program_6transform(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text, PyObject *__pyx_v_text_output, PyObject *__pyx_v_multiple_output) {
+static PyObject *__pyx_pf_2jq_8_Program_12transform(struct __pyx_obj_2jq__Program *__pyx_v_self, PyObject *__pyx_v_value, PyObject *__pyx_v_text, PyObject *__pyx_v_text_output, PyObject *__pyx_v_multiple_output) {
   PyObject *__pyx_v_program_with_input = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("transform", 0);
 
-  /* "jq.pyx":262
+  /* "jq.pyx":280
  *     # Support the 0.1.x API for backwards compatibility
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):
  *         program_with_input = self.input(value, text=text)             # <<<<<<<<<<<<<<
  *         if text_output:
  *             return program_with_input.text()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_input); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_value);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 262, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_program_with_input = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "jq.pyx":263
+  /* "jq.pyx":281
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):
  *         program_with_input = self.input(value, text=text)
  *         if text_output:             # <<<<<<<<<<<<<<
  *             return program_with_input.text()
  *         elif multiple_output:
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_text_output); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_text_output); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 281, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "jq.pyx":264
+    /* "jq.pyx":282
  *         program_with_input = self.input(value, text=text)
  *         if text_output:
  *             return program_with_input.text()             # <<<<<<<<<<<<<<
  *         elif multiple_output:
  *             return program_with_input.all()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 282, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "jq.pyx":263
+    /* "jq.pyx":281
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):
  *         program_with_input = self.input(value, text=text)
  *         if text_output:             # <<<<<<<<<<<<<<
  *             return program_with_input.text()
  *         elif multiple_output:
  */
   }
 
-  /* "jq.pyx":265
+  /* "jq.pyx":283
  *         if text_output:
  *             return program_with_input.text()
  *         elif multiple_output:             # <<<<<<<<<<<<<<
  *             return program_with_input.all()
  *         else:
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_multiple_output); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_multiple_output); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "jq.pyx":266
+    /* "jq.pyx":284
  *             return program_with_input.text()
  *         elif multiple_output:
  *             return program_with_input.all()             # <<<<<<<<<<<<<<
  *         else:
  *             return program_with_input.first()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_all); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_all); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "jq.pyx":265
+    /* "jq.pyx":283
  *         if text_output:
  *             return program_with_input.text()
  *         elif multiple_output:             # <<<<<<<<<<<<<<
  *             return program_with_input.all()
  *         else:
  */
   }
 
-  /* "jq.pyx":268
+  /* "jq.pyx":286
  *             return program_with_input.all()
  *         else:
  *             return program_with_input.first()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_first); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_program_with_input, __pyx_n_s_first); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 268, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
   }
 
-  /* "jq.pyx":261
+  /* "jq.pyx":279
  * 
  *     # Support the 0.1.x API for backwards compatibility
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):             # <<<<<<<<<<<<<<
  *         program_with_input = self.input(value, text=text)
  *         if text_output:
  */
 
@@ -5357,27 +5919,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2jq_8_Program_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_2jq_8_Program_9__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_2jq_8_Program_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_2jq_8_Program_8__reduce_cython__(((struct __pyx_obj_2jq__Program *)__pyx_v_self));
+  __pyx_r = __pyx_pf_2jq_8_Program_14__reduce_cython__(((struct __pyx_obj_2jq__Program *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2jq_8_Program_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self) {
+static PyObject *__pyx_pf_2jq_8_Program_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -5414,27 +5976,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2jq_8_Program_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_2jq_8_Program_11__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_2jq_8_Program_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_2jq_8_Program_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_2jq_8_Program_10__setstate_cython__(((struct __pyx_obj_2jq__Program *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_2jq_8_Program_16__setstate_cython__(((struct __pyx_obj_2jq__Program *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2jq_8_Program_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_2jq_8_Program_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2jq__Program *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -5463,37 +6025,38 @@
   __Pyx_AddTraceback("jq._Program.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":275
- *     cdef object _bytes_input
+/* "jq.pyx":294
+ *     cdef bint _slurp
  * 
- *     def __cinit__(self, jq_state_pool, bytes_input):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, jq_state_pool, bytes_input, *, bint slurp):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool = jq_state_pool
  *         self._bytes_input = bytes_input
  */
 
 /* Python wrapper */
 static int __pyx_pw_2jq_17_ProgramWithInput_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_2jq_17_ProgramWithInput_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_jq_state_pool = 0;
   PyObject *__pyx_v_bytes_input = 0;
+  int __pyx_v_slurp;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_jq_state_pool,&__pyx_n_s_bytes_input,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_jq_state_pool,&__pyx_n_s_bytes_input,&__pyx_n_s_slurp,0};
+    PyObject* values[3] = {0,0,0};
+    if (likely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -5505,86 +6068,101 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_jq_state_pool)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytes_input)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 275, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 294, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slurp)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseKeywordRequired("__cinit__", __pyx_n_s_slurp); __PYX_ERR(0, 294, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 275, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 294, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      __Pyx_RaiseKeywordRequired("__cinit__", __pyx_n_s_slurp); __PYX_ERR(0, 294, __pyx_L3_error)
     }
     __pyx_v_jq_state_pool = values[0];
     __pyx_v_bytes_input = values[1];
+    __pyx_v_slurp = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_slurp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 275, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 294, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._ProgramWithInput.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2jq_17_ProgramWithInput___cinit__(((struct __pyx_obj_2jq__ProgramWithInput *)__pyx_v_self), __pyx_v_jq_state_pool, __pyx_v_bytes_input);
+  __pyx_r = __pyx_pf_2jq_17_ProgramWithInput___cinit__(((struct __pyx_obj_2jq__ProgramWithInput *)__pyx_v_self), __pyx_v_jq_state_pool, __pyx_v_bytes_input, __pyx_v_slurp);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_2jq_17_ProgramWithInput___cinit__(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self, PyObject *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input) {
+static int __pyx_pf_2jq_17_ProgramWithInput___cinit__(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self, PyObject *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input, int __pyx_v_slurp) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "jq.pyx":276
+  /* "jq.pyx":295
  * 
- *     def __cinit__(self, jq_state_pool, bytes_input):
+ *     def __cinit__(self, jq_state_pool, bytes_input, *, bint slurp):
  *         self._jq_state_pool = jq_state_pool             # <<<<<<<<<<<<<<
  *         self._bytes_input = bytes_input
- * 
+ *         self._slurp = slurp
  */
-  if (!(likely(((__pyx_v_jq_state_pool) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_jq_state_pool, __pyx_ptype_2jq__JqStatePool))))) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (!(likely(((__pyx_v_jq_state_pool) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_jq_state_pool, __pyx_ptype_2jq__JqStatePool))))) __PYX_ERR(0, 295, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_jq_state_pool;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_jq_state_pool);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   __pyx_v_self->_jq_state_pool = ((struct __pyx_obj_2jq__JqStatePool *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "jq.pyx":277
- *     def __cinit__(self, jq_state_pool, bytes_input):
+  /* "jq.pyx":296
+ *     def __cinit__(self, jq_state_pool, bytes_input, *, bint slurp):
  *         self._jq_state_pool = jq_state_pool
  *         self._bytes_input = bytes_input             # <<<<<<<<<<<<<<
+ *         self._slurp = slurp
  * 
- *     def __iter__(self):
  */
   __Pyx_INCREF(__pyx_v_bytes_input);
   __Pyx_GIVEREF(__pyx_v_bytes_input);
   __Pyx_GOTREF(__pyx_v_self->_bytes_input);
   __Pyx_DECREF(__pyx_v_self->_bytes_input);
   __pyx_v_self->_bytes_input = __pyx_v_bytes_input;
 
-  /* "jq.pyx":275
- *     cdef object _bytes_input
+  /* "jq.pyx":297
+ *         self._jq_state_pool = jq_state_pool
+ *         self._bytes_input = bytes_input
+ *         self._slurp = slurp             # <<<<<<<<<<<<<<
  * 
- *     def __cinit__(self, jq_state_pool, bytes_input):             # <<<<<<<<<<<<<<
+ *     def __iter__(self):
+ */
+  __pyx_v_self->_slurp = __pyx_v_slurp;
+
+  /* "jq.pyx":294
+ *     cdef bint _slurp
+ * 
+ *     def __cinit__(self, jq_state_pool, bytes_input, *, bint slurp):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool = jq_state_pool
  *         self._bytes_input = bytes_input
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -5593,16 +6171,16 @@
   __Pyx_AddTraceback("jq._ProgramWithInput.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":279
- *         self._bytes_input = bytes_input
+/* "jq.pyx":299
+ *         self._slurp = slurp
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self._make_iterator()
  * 
  */
 
 /* Python wrapper */
@@ -5623,30 +6201,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "jq.pyx":280
+  /* "jq.pyx":300
  * 
  *     def __iter__(self):
  *         return self._make_iterator()             # <<<<<<<<<<<<<<
  * 
  *     cdef _ResultIterator _make_iterator(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_2jq__ProgramWithInput *)__pyx_v_self->__pyx_vtab)->_make_iterator(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_2jq__ProgramWithInput *)__pyx_v_self->__pyx_vtab)->_make_iterator(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":279
- *         self._bytes_input = bytes_input
+  /* "jq.pyx":299
+ *         self._slurp = slurp
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self._make_iterator()
  * 
  */
 
   /* function exit code */
@@ -5656,77 +6234,86 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":282
+/* "jq.pyx":302
  *         return self._make_iterator()
  * 
  *     cdef _ResultIterator _make_iterator(self):             # <<<<<<<<<<<<<<
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  */
 
 static struct __pyx_obj_2jq__ResultIterator *__pyx_f_2jq_17_ProgramWithInput__make_iterator(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self) {
   struct __pyx_obj_2jq__ResultIterator *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_make_iterator", 0);
 
-  /* "jq.pyx":283
+  /* "jq.pyx":303
  * 
  *     cdef _ResultIterator _make_iterator(self):
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)             # <<<<<<<<<<<<<<
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)             # <<<<<<<<<<<<<<
  * 
  *     def text(self):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_v_self->_jq_state_pool));
   __Pyx_INCREF(__pyx_v_self->_bytes_input);
   __Pyx_GIVEREF(__pyx_v_self->_bytes_input);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_self->_bytes_input);
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__ResultIterator), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_self->_slurp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_slurp, __pyx_t_3) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2jq__ResultIterator), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_r = ((struct __pyx_obj_2jq__ResultIterator *)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = ((struct __pyx_obj_2jq__ResultIterator *)__pyx_t_3);
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":282
+  /* "jq.pyx":302
  *         return self._make_iterator()
  * 
  *     cdef _ResultIterator _make_iterator(self):             # <<<<<<<<<<<<<<
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("jq._ProgramWithInput._make_iterator", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":285
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+/* "jq.pyx":305
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  *     def text(self):             # <<<<<<<<<<<<<<
  *         # Performance testing suggests that using _jv_to_python (within the
  *         # result iterator) followed by json.dumps is faster than using
  */
 
 /* Python wrapper */
@@ -5739,15 +6326,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2jq_17_ProgramWithInput_4text_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "jq.pyx":290
+/* "jq.pyx":310
  *         # jv_dump_string to generate the string directly from the jv values.
  *         # See: https://github.com/mwilliamson/jq.py/pull/50
  *         return "\n".join(json.dumps(v) for v in self)             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
 
@@ -5759,23 +6346,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2jq___pyx_scope_struct_1_genexpr *)__pyx_tp_new_2jq___pyx_scope_struct_1_genexpr(__pyx_ptype_2jq___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2jq___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 290, __pyx_L1_error)
+    __PYX_ERR(0, 310, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_2jq___pyx_scope_struct__text *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2jq_17_ProgramWithInput_4text_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_text_locals_genexpr, __pyx_n_s_jq); if (unlikely(!gen)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2jq_17_ProgramWithInput_4text_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_text_locals_genexpr, __pyx_n_s_jq); if (unlikely(!gen)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5806,77 +6393,77 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 290, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 290, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 310, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 310, __pyx_L1_error) }
   if (likely(PyList_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self))) {
     __pyx_t_1 = ((PyObject *)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self); __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 310, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 310, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 290, __pyx_L1_error)
+          else __PYX_ERR(0, 310, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_v);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_v, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_cur_scope->__pyx_v_v) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_cur_scope->__pyx_v_v);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
@@ -5889,15 +6476,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 290, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 310, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -5914,16 +6501,16 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":285
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+/* "jq.pyx":305
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  *     def text(self):             # <<<<<<<<<<<<<<
  *         # Performance testing suggests that using _jv_to_python (within the
  *         # result iterator) followed by json.dumps is faster than using
  */
 
 static PyObject *__pyx_pf_2jq_17_ProgramWithInput_4text(struct __pyx_obj_2jq__ProgramWithInput *__pyx_v_self) {
@@ -5937,41 +6524,41 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("text", 0);
   __pyx_cur_scope = (struct __pyx_obj_2jq___pyx_scope_struct__text *)__pyx_tp_new_2jq___pyx_scope_struct__text(__pyx_ptype_2jq___pyx_scope_struct__text, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2jq___pyx_scope_struct__text *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 285, __pyx_L1_error)
+    __PYX_ERR(0, 305, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
 
-  /* "jq.pyx":290
+  /* "jq.pyx":310
  *         # jv_dump_string to generate the string directly from the jv values.
  *         # See: https://github.com/mwilliamson/jq.py/pull/50
  *         return "\n".join(json.dumps(v) for v in self)             # <<<<<<<<<<<<<<
  * 
  *     def all(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_pf_2jq_17_ProgramWithInput_4text_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2jq_17_ProgramWithInput_4text_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":285
- *         return _ResultIterator(self._jq_state_pool, self._bytes_input)
+  /* "jq.pyx":305
+ *         return _ResultIterator(self._jq_state_pool, self._bytes_input, slurp=self._slurp)
  * 
  *     def text(self):             # <<<<<<<<<<<<<<
  *         # Performance testing suggests that using _jv_to_python (within the
  *         # result iterator) followed by json.dumps is faster than using
  */
 
   /* function exit code */
@@ -5984,15 +6571,15 @@
   __Pyx_XDECREF(__pyx_gb_2jq_17_ProgramWithInput_4text_2generator);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":292
+/* "jq.pyx":312
  *         return "\n".join(json.dumps(v) for v in self)
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         return list(self)
  * 
  */
 
@@ -6014,29 +6601,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all", 0);
 
-  /* "jq.pyx":293
+  /* "jq.pyx":313
  * 
  *     def all(self):
  *         return list(self)             # <<<<<<<<<<<<<<
  * 
  *     def first(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PySequence_List(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":292
+  /* "jq.pyx":312
  *         return "\n".join(json.dumps(v) for v in self)
  * 
  *     def all(self):             # <<<<<<<<<<<<<<
  *         return list(self)
  * 
  */
 
@@ -6047,15 +6634,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":295
+/* "jq.pyx":315
  *         return list(self)
  * 
  *     def first(self):             # <<<<<<<<<<<<<<
  *         return next(_iter(self))
  * 
  */
 
@@ -6079,47 +6666,47 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("first", 0);
 
-  /* "jq.pyx":296
+  /* "jq.pyx":316
  * 
  *     def first(self):
  *         return next(_iter(self))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_self)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_self));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 296, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyIter_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyIter_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":295
+  /* "jq.pyx":315
  *         return list(self)
  * 
  *     def first(self):             # <<<<<<<<<<<<<<
  *         return next(_iter(self))
  * 
  */
 
@@ -6245,15 +6832,15 @@
   __Pyx_AddTraceback("jq._ProgramWithInput.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":306
+/* "jq.pyx":327
  *     cdef bint _ready
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool.release(self._jq)
  *         jv_parser_free(self._parser)
  */
 
@@ -6268,67 +6855,68 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_2jq_15_ResultIterator___dealloc__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "jq.pyx":307
+  /* "jq.pyx":328
  * 
  *     def __dealloc__(self):
  *         self._jq_state_pool.release(self._jq)             # <<<<<<<<<<<<<<
  *         jv_parser_free(self._parser)
  * 
  */
   ((struct __pyx_vtabstruct_2jq__JqStatePool *)__pyx_v_self->_jq_state_pool->__pyx_vtab)->release(__pyx_v_self->_jq_state_pool, __pyx_v_self->_jq);
 
-  /* "jq.pyx":308
+  /* "jq.pyx":329
  *     def __dealloc__(self):
  *         self._jq_state_pool.release(self._jq)
  *         jv_parser_free(self._parser)             # <<<<<<<<<<<<<<
  * 
- *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input):
+ *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input, *, bint slurp):
  */
   jv_parser_free(__pyx_v_self->_parser);
 
-  /* "jq.pyx":306
+  /* "jq.pyx":327
  *     cdef bint _ready
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool.release(self._jq)
  *         jv_parser_free(self._parser)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "jq.pyx":310
+/* "jq.pyx":331
  *         jv_parser_free(self._parser)
  * 
- *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input, *, bint slurp):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool = jq_state_pool
  *         self._jq = jq_state_pool.acquire()
  */
 
 /* Python wrapper */
 static int __pyx_pw_2jq_15_ResultIterator_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_2jq_15_ResultIterator_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_2jq__JqStatePool *__pyx_v_jq_state_pool = 0;
   PyObject *__pyx_v_bytes_input = 0;
+  int __pyx_v_slurp;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_jq_state_pool,&__pyx_n_s_bytes_input,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_jq_state_pool,&__pyx_n_s_bytes_input,&__pyx_n_s_slurp,0};
+    PyObject* values[3] = {0,0,0};
+    if (likely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -6340,152 +6928,167 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_jq_state_pool)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytes_input)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 310, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, 1); __PYX_ERR(0, 331, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slurp)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseKeywordRequired("__cinit__", __pyx_n_s_slurp); __PYX_ERR(0, 331, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 310, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 331, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      __Pyx_RaiseKeywordRequired("__cinit__", __pyx_n_s_slurp); __PYX_ERR(0, 331, __pyx_L3_error)
     }
     __pyx_v_jq_state_pool = ((struct __pyx_obj_2jq__JqStatePool *)values[0]);
     __pyx_v_bytes_input = ((PyObject*)values[1]);
+    __pyx_v_slurp = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_slurp == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 331, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 310, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 331, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq._ResultIterator.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_jq_state_pool), __pyx_ptype_2jq__JqStatePool, 1, "jq_state_pool", 0))) __PYX_ERR(0, 310, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_bytes_input), (&PyBytes_Type), 1, "bytes_input", 1))) __PYX_ERR(0, 310, __pyx_L1_error)
-  __pyx_r = __pyx_pf_2jq_15_ResultIterator_2__cinit__(((struct __pyx_obj_2jq__ResultIterator *)__pyx_v_self), __pyx_v_jq_state_pool, __pyx_v_bytes_input);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_jq_state_pool), __pyx_ptype_2jq__JqStatePool, 1, "jq_state_pool", 0))) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_bytes_input), (&PyBytes_Type), 1, "bytes_input", 1))) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_r = __pyx_pf_2jq_15_ResultIterator_2__cinit__(((struct __pyx_obj_2jq__ResultIterator *)__pyx_v_self), __pyx_v_jq_state_pool, __pyx_v_bytes_input, __pyx_v_slurp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_2jq_15_ResultIterator_2__cinit__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self, struct __pyx_obj_2jq__JqStatePool *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input) {
+static int __pyx_pf_2jq_15_ResultIterator_2__cinit__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self, struct __pyx_obj_2jq__JqStatePool *__pyx_v_jq_state_pool, PyObject *__pyx_v_bytes_input, int __pyx_v_slurp) {
   struct jv_parser *__pyx_v_parser;
   char *__pyx_v_cbytes_input;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "jq.pyx":311
+  /* "jq.pyx":332
  * 
- *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input):
+ *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input, *, bint slurp):
  *         self._jq_state_pool = jq_state_pool             # <<<<<<<<<<<<<<
  *         self._jq = jq_state_pool.acquire()
  *         self._bytes_input = bytes_input
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_jq_state_pool));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_jq_state_pool));
   __Pyx_GOTREF(__pyx_v_self->_jq_state_pool);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_jq_state_pool));
   __pyx_v_self->_jq_state_pool = __pyx_v_jq_state_pool;
 
-  /* "jq.pyx":312
- *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input):
+  /* "jq.pyx":333
+ *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input, *, bint slurp):
  *         self._jq_state_pool = jq_state_pool
  *         self._jq = jq_state_pool.acquire()             # <<<<<<<<<<<<<<
  *         self._bytes_input = bytes_input
- *         self._ready = False
+ *         self._slurp = slurp
  */
   __pyx_v_self->_jq = ((struct __pyx_vtabstruct_2jq__JqStatePool *)__pyx_v_jq_state_pool->__pyx_vtab)->acquire(__pyx_v_jq_state_pool);
 
-  /* "jq.pyx":313
+  /* "jq.pyx":334
  *         self._jq_state_pool = jq_state_pool
  *         self._jq = jq_state_pool.acquire()
  *         self._bytes_input = bytes_input             # <<<<<<<<<<<<<<
+ *         self._slurp = slurp
  *         self._ready = False
- *         cdef jv_parser* parser = jv_parser_new(0)
  */
   __Pyx_INCREF(__pyx_v_bytes_input);
   __Pyx_GIVEREF(__pyx_v_bytes_input);
   __Pyx_GOTREF(__pyx_v_self->_bytes_input);
   __Pyx_DECREF(__pyx_v_self->_bytes_input);
   __pyx_v_self->_bytes_input = __pyx_v_bytes_input;
 
-  /* "jq.pyx":314
+  /* "jq.pyx":335
  *         self._jq = jq_state_pool.acquire()
  *         self._bytes_input = bytes_input
+ *         self._slurp = slurp             # <<<<<<<<<<<<<<
+ *         self._ready = False
+ *         cdef jv_parser* parser = jv_parser_new(0)
+ */
+  __pyx_v_self->_slurp = __pyx_v_slurp;
+
+  /* "jq.pyx":336
+ *         self._bytes_input = bytes_input
+ *         self._slurp = slurp
  *         self._ready = False             # <<<<<<<<<<<<<<
  *         cdef jv_parser* parser = jv_parser_new(0)
  *         cdef char* cbytes_input = PyBytes_AsString(bytes_input)
  */
   __pyx_v_self->_ready = 0;
 
-  /* "jq.pyx":315
- *         self._bytes_input = bytes_input
+  /* "jq.pyx":337
+ *         self._slurp = slurp
  *         self._ready = False
  *         cdef jv_parser* parser = jv_parser_new(0)             # <<<<<<<<<<<<<<
  *         cdef char* cbytes_input = PyBytes_AsString(bytes_input)
  *         jv_parser_set_buf(parser, cbytes_input, len(bytes_input), 0)
  */
   __pyx_v_parser = jv_parser_new(0);
 
-  /* "jq.pyx":316
+  /* "jq.pyx":338
  *         self._ready = False
  *         cdef jv_parser* parser = jv_parser_new(0)
  *         cdef char* cbytes_input = PyBytes_AsString(bytes_input)             # <<<<<<<<<<<<<<
  *         jv_parser_set_buf(parser, cbytes_input, len(bytes_input), 0)
  *         self._parser = parser
  */
-  __pyx_t_1 = PyBytes_AsString(__pyx_v_bytes_input); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_AsString(__pyx_v_bytes_input); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(0, 338, __pyx_L1_error)
   __pyx_v_cbytes_input = __pyx_t_1;
 
-  /* "jq.pyx":317
+  /* "jq.pyx":339
  *         cdef jv_parser* parser = jv_parser_new(0)
  *         cdef char* cbytes_input = PyBytes_AsString(bytes_input)
  *         jv_parser_set_buf(parser, cbytes_input, len(bytes_input), 0)             # <<<<<<<<<<<<<<
  *         self._parser = parser
  * 
  */
   if (unlikely(__pyx_v_bytes_input == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 317, __pyx_L1_error)
+    __PYX_ERR(0, 339, __pyx_L1_error)
   }
-  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_bytes_input); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_bytes_input); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 339, __pyx_L1_error)
   jv_parser_set_buf(__pyx_v_parser, __pyx_v_cbytes_input, __pyx_t_2, 0);
 
-  /* "jq.pyx":318
+  /* "jq.pyx":340
  *         cdef char* cbytes_input = PyBytes_AsString(bytes_input)
  *         jv_parser_set_buf(parser, cbytes_input, len(bytes_input), 0)
  *         self._parser = parser             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_v_self->_parser = __pyx_v_parser;
 
-  /* "jq.pyx":310
+  /* "jq.pyx":331
  *         jv_parser_free(self._parser)
  * 
- *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input):             # <<<<<<<<<<<<<<
+ *     def __cinit__(self, _JqStatePool jq_state_pool, bytes bytes_input, *, bint slurp):             # <<<<<<<<<<<<<<
  *         self._jq_state_pool = jq_state_pool
  *         self._jq = jq_state_pool.acquire()
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -6493,15 +7096,15 @@
   __Pyx_AddTraceback("jq._ResultIterator.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":320
+/* "jq.pyx":342
  *         self._parser = parser
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -6519,47 +7122,47 @@
 }
 
 static PyObject *__pyx_pf_2jq_15_ResultIterator_4__iter__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "jq.pyx":321
+  /* "jq.pyx":343
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "jq.pyx":320
+  /* "jq.pyx":342
  *         self._parser = parser
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":323
+/* "jq.pyx":345
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
- *         cdef int dumpopts = 0
  *         while True:
+ *             if not self._ready:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2jq_15_ResultIterator_7__next__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_2jq_15_ResultIterator_7__next__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6568,213 +7171,203 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_2jq_15_ResultIterator_6__next__(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self) {
-  CYTHON_UNUSED int __pyx_v_dumpopts;
   jv __pyx_v_result;
   jv __pyx_v_error_message;
   PyObject *__pyx_v_message = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "jq.pyx":324
+  /* "jq.pyx":346
  * 
  *     def __next__(self):
- *         cdef int dumpopts = 0             # <<<<<<<<<<<<<<
- *         while True:
- *             if not self._ready:
- */
-  __pyx_v_dumpopts = 0;
-
-  /* "jq.pyx":325
- *     def __next__(self):
- *         cdef int dumpopts = 0
  *         while True:             # <<<<<<<<<<<<<<
  *             if not self._ready:
  *                 self._ready_next_input()
  */
   while (1) {
 
-    /* "jq.pyx":326
- *         cdef int dumpopts = 0
+    /* "jq.pyx":347
+ *     def __next__(self):
  *         while True:
  *             if not self._ready:             # <<<<<<<<<<<<<<
  *                 self._ready_next_input()
  *                 self._ready = True
  */
     __pyx_t_1 = ((!(__pyx_v_self->_ready != 0)) != 0);
     if (__pyx_t_1) {
 
-      /* "jq.pyx":327
+      /* "jq.pyx":348
  *         while True:
  *             if not self._ready:
  *                 self._ready_next_input()             # <<<<<<<<<<<<<<
  *                 self._ready = True
  * 
  */
-      __pyx_t_1 = ((struct __pyx_vtabstruct_2jq__ResultIterator *)__pyx_v_self->__pyx_vtab)->_ready_next_input(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)1))) __PYX_ERR(0, 327, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_2jq__ResultIterator *)__pyx_v_self->__pyx_vtab)->_ready_next_input(__pyx_v_self); if (unlikely(__pyx_t_1 == ((int)1))) __PYX_ERR(0, 348, __pyx_L1_error)
 
-      /* "jq.pyx":328
+      /* "jq.pyx":349
  *             if not self._ready:
  *                 self._ready_next_input()
  *                 self._ready = True             # <<<<<<<<<<<<<<
  * 
  *             result = jq_next(self._jq)
  */
       __pyx_v_self->_ready = 1;
 
-      /* "jq.pyx":326
- *         cdef int dumpopts = 0
+      /* "jq.pyx":347
+ *     def __next__(self):
  *         while True:
  *             if not self._ready:             # <<<<<<<<<<<<<<
  *                 self._ready_next_input()
  *                 self._ready = True
  */
     }
 
-    /* "jq.pyx":330
+    /* "jq.pyx":351
  *                 self._ready = True
  * 
  *             result = jq_next(self._jq)             # <<<<<<<<<<<<<<
  *             if jv_is_valid(result):
  *                 return _jv_to_python(result)
  */
     __pyx_v_result = jq_next(__pyx_v_self->_jq);
 
-    /* "jq.pyx":331
+    /* "jq.pyx":352
  * 
  *             result = jq_next(self._jq)
  *             if jv_is_valid(result):             # <<<<<<<<<<<<<<
  *                 return _jv_to_python(result)
  *             elif jv_invalid_has_msg(jv_copy(result)):
  */
     __pyx_t_1 = (jv_is_valid(__pyx_v_result) != 0);
     if (__pyx_t_1) {
 
-      /* "jq.pyx":332
+      /* "jq.pyx":353
  *             result = jq_next(self._jq)
  *             if jv_is_valid(result):
  *                 return _jv_to_python(result)             # <<<<<<<<<<<<<<
  *             elif jv_invalid_has_msg(jv_copy(result)):
  *                 error_message = jv_invalid_get_msg(result)
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_2 = __pyx_f_2jq__jv_to_python(__pyx_v_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_2jq__jv_to_python(__pyx_v_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_r = __pyx_t_2;
       __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "jq.pyx":331
+      /* "jq.pyx":352
  * 
  *             result = jq_next(self._jq)
  *             if jv_is_valid(result):             # <<<<<<<<<<<<<<
  *                 return _jv_to_python(result)
  *             elif jv_invalid_has_msg(jv_copy(result)):
  */
     }
 
-    /* "jq.pyx":333
+    /* "jq.pyx":354
  *             if jv_is_valid(result):
  *                 return _jv_to_python(result)
  *             elif jv_invalid_has_msg(jv_copy(result)):             # <<<<<<<<<<<<<<
  *                 error_message = jv_invalid_get_msg(result)
  *                 message = jv_string_to_py_string(error_message)
  */
     __pyx_t_1 = (jv_invalid_has_msg(jv_copy(__pyx_v_result)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "jq.pyx":334
+      /* "jq.pyx":355
  *                 return _jv_to_python(result)
  *             elif jv_invalid_has_msg(jv_copy(result)):
  *                 error_message = jv_invalid_get_msg(result)             # <<<<<<<<<<<<<<
  *                 message = jv_string_to_py_string(error_message)
  *                 jv_free(error_message)
  */
       __pyx_v_error_message = jv_invalid_get_msg(__pyx_v_result);
 
-      /* "jq.pyx":335
+      /* "jq.pyx":356
  *             elif jv_invalid_has_msg(jv_copy(result)):
  *                 error_message = jv_invalid_get_msg(result)
  *                 message = jv_string_to_py_string(error_message)             # <<<<<<<<<<<<<<
  *                 jv_free(error_message)
  *                 raise ValueError(message)
  */
-      __pyx_t_2 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_v_message = ((PyObject*)__pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "jq.pyx":336
+      /* "jq.pyx":357
  *                 error_message = jv_invalid_get_msg(result)
  *                 message = jv_string_to_py_string(error_message)
  *                 jv_free(error_message)             # <<<<<<<<<<<<<<
  *                 raise ValueError(message)
  *             else:
  */
       jv_free(__pyx_v_error_message);
 
-      /* "jq.pyx":337
+      /* "jq.pyx":358
  *                 message = jv_string_to_py_string(error_message)
  *                 jv_free(error_message)
  *                 raise ValueError(message)             # <<<<<<<<<<<<<<
  *             else:
  *                 jv_free(result)
  */
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 337, __pyx_L1_error)
+      __PYX_ERR(0, 358, __pyx_L1_error)
 
-      /* "jq.pyx":333
+      /* "jq.pyx":354
  *             if jv_is_valid(result):
  *                 return _jv_to_python(result)
  *             elif jv_invalid_has_msg(jv_copy(result)):             # <<<<<<<<<<<<<<
  *                 error_message = jv_invalid_get_msg(result)
  *                 message = jv_string_to_py_string(error_message)
  */
     }
 
-    /* "jq.pyx":339
+    /* "jq.pyx":360
  *                 raise ValueError(message)
  *             else:
  *                 jv_free(result)             # <<<<<<<<<<<<<<
  *                 self._ready = False
  * 
  */
     /*else*/ {
       jv_free(__pyx_v_result);
 
-      /* "jq.pyx":340
+      /* "jq.pyx":361
  *             else:
  *                 jv_free(result)
  *                 self._ready = False             # <<<<<<<<<<<<<<
  * 
  *     cdef bint _ready_next_input(self) except 1:
  */
       __pyx_v_self->_ready = 0;
     }
   }
 
-  /* "jq.pyx":323
+  /* "jq.pyx":345
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
- *         cdef int dumpopts = 0
  *         while True:
+ *             if not self._ready:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -6783,196 +7376,417 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":342
+/* "jq.pyx":363
  *                 self._ready = False
  * 
  *     cdef bint _ready_next_input(self) except 1:             # <<<<<<<<<<<<<<
  *         cdef int jq_flags = 0
- *         cdef jv value = jv_parser_next(self._parser)
+ *         cdef jv value
  */
 
 static int __pyx_f_2jq_15_ResultIterator__ready_next_input(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self) {
   int __pyx_v_jq_flags;
   jv __pyx_v_value;
-  jv __pyx_v_error_message;
-  PyObject *__pyx_v_message = NULL;
+  jv __pyx_v_next_value;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  jv __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_ready_next_input", 0);
 
-  /* "jq.pyx":343
+  /* "jq.pyx":364
  * 
  *     cdef bint _ready_next_input(self) except 1:
  *         cdef int jq_flags = 0             # <<<<<<<<<<<<<<
- *         cdef jv value = jv_parser_next(self._parser)
- *         if jv_is_valid(value):
+ *         cdef jv value
+ * 
  */
   __pyx_v_jq_flags = 0;
 
-  /* "jq.pyx":344
- *     cdef bint _ready_next_input(self) except 1:
+  /* "jq.pyx":367
+ *         cdef jv value
+ * 
+ *         if self._slurp:             # <<<<<<<<<<<<<<
+ *             value = jv_array()
+ * 
+ */
+  __pyx_t_1 = (__pyx_v_self->_slurp != 0);
+  if (__pyx_t_1) {
+
+    /* "jq.pyx":368
+ * 
+ *         if self._slurp:
+ *             value = jv_array()             # <<<<<<<<<<<<<<
+ * 
+ *             while True:
+ */
+    __pyx_v_value = jv_array();
+
+    /* "jq.pyx":370
+ *             value = jv_array()
+ * 
+ *             while True:             # <<<<<<<<<<<<<<
+ *                 try:
+ *                     next_value = self._parse_next_input()
+ */
+    while (1) {
+
+      /* "jq.pyx":371
+ * 
+ *             while True:
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     next_value = self._parse_next_input()
+ *                     value = jv_array_append(value, next_value)
+ */
+      {
+        __Pyx_PyThreadState_declare
+        __Pyx_PyThreadState_assign
+        __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
+        __Pyx_XGOTREF(__pyx_t_2);
+        __Pyx_XGOTREF(__pyx_t_3);
+        __Pyx_XGOTREF(__pyx_t_4);
+        /*try:*/ {
+
+          /* "jq.pyx":372
+ *             while True:
+ *                 try:
+ *                     next_value = self._parse_next_input()             # <<<<<<<<<<<<<<
+ *                     value = jv_array_append(value, next_value)
+ *                 except StopIteration:
+ */
+          __pyx_t_5 = __pyx_f_2jq_15_ResultIterator__parse_next_input(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 372, __pyx_L6_error)
+          __pyx_v_next_value = __pyx_t_5;
+
+          /* "jq.pyx":373
+ *                 try:
+ *                     next_value = self._parse_next_input()
+ *                     value = jv_array_append(value, next_value)             # <<<<<<<<<<<<<<
+ *                 except StopIteration:
+ *                     self._slurp = False
+ */
+          __pyx_v_value = jv_array_append(__pyx_v_value, __pyx_v_next_value);
+
+          /* "jq.pyx":371
+ * 
+ *             while True:
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     next_value = self._parse_next_input()
+ *                     value = jv_array_append(value, next_value)
+ */
+        }
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        goto __pyx_L13_try_end;
+        __pyx_L6_error:;
+
+        /* "jq.pyx":374
+ *                     next_value = self._parse_next_input()
+ *                     value = jv_array_append(value, next_value)
+ *                 except StopIteration:             # <<<<<<<<<<<<<<
+ *                     self._slurp = False
+ *                     break
+ */
+        __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
+        if (__pyx_t_6) {
+          __Pyx_AddTraceback("jq._ResultIterator._ready_next_input", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9) < 0) __PYX_ERR(0, 374, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_GOTREF(__pyx_t_9);
+
+          /* "jq.pyx":375
+ *                     value = jv_array_append(value, next_value)
+ *                 except StopIteration:
+ *                     self._slurp = False             # <<<<<<<<<<<<<<
+ *                     break
+ *         else:
+ */
+          __pyx_v_self->_slurp = 0;
+
+          /* "jq.pyx":376
+ *                 except StopIteration:
+ *                     self._slurp = False
+ *                     break             # <<<<<<<<<<<<<<
+ *         else:
+ *             value = self._parse_next_input()
+ */
+          goto __pyx_L14_except_break;
+          __pyx_L14_except_break:;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+          goto __pyx_L11_try_break;
+        }
+        goto __pyx_L8_except_error;
+        __pyx_L8_except_error:;
+
+        /* "jq.pyx":371
+ * 
+ *             while True:
+ *                 try:             # <<<<<<<<<<<<<<
+ *                     next_value = self._parse_next_input()
+ *                     value = jv_array_append(value, next_value)
+ */
+        __Pyx_XGIVEREF(__pyx_t_2);
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
+        goto __pyx_L1_error;
+        __pyx_L11_try_break:;
+        __Pyx_XGIVEREF(__pyx_t_2);
+        __Pyx_XGIVEREF(__pyx_t_3);
+        __Pyx_XGIVEREF(__pyx_t_4);
+        __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
+        goto __pyx_L5_break;
+        __pyx_L13_try_end:;
+      }
+    }
+    __pyx_L5_break:;
+
+    /* "jq.pyx":367
+ *         cdef jv value
+ * 
+ *         if self._slurp:             # <<<<<<<<<<<<<<
+ *             value = jv_array()
+ * 
+ */
+    goto __pyx_L3;
+  }
+
+  /* "jq.pyx":378
+ *                     break
+ *         else:
+ *             value = self._parse_next_input()             # <<<<<<<<<<<<<<
+ * 
+ *         jq_start(self._jq, value, jq_flags)
+ */
+  /*else*/ {
+    __pyx_t_5 = __pyx_f_2jq_15_ResultIterator__parse_next_input(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 378, __pyx_L1_error)
+    __pyx_v_value = __pyx_t_5;
+  }
+  __pyx_L3:;
+
+  /* "jq.pyx":380
+ *             value = self._parse_next_input()
+ * 
+ *         jq_start(self._jq, value, jq_flags)             # <<<<<<<<<<<<<<
+ *         return 0
+ * 
+ */
+  jq_start(__pyx_v_self->_jq, __pyx_v_value, __pyx_v_jq_flags);
+
+  /* "jq.pyx":381
+ * 
+ *         jq_start(self._jq, value, jq_flags)
+ *         return 0             # <<<<<<<<<<<<<<
+ * 
+ *     cdef inline jv _parse_next_input(self) except *:
+ */
+  __pyx_r = 0;
+  goto __pyx_L0;
+
+  /* "jq.pyx":363
+ *                 self._ready = False
+ * 
+ *     cdef bint _ready_next_input(self) except 1:             # <<<<<<<<<<<<<<
  *         cdef int jq_flags = 0
+ *         cdef jv value
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("jq._ResultIterator._ready_next_input", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "jq.pyx":383
+ *         return 0
+ * 
+ *     cdef inline jv _parse_next_input(self) except *:             # <<<<<<<<<<<<<<
+ *         cdef jv value = jv_parser_next(self._parser)
+ *         if jv_is_valid(value):
+ */
+
+static CYTHON_INLINE jv __pyx_f_2jq_15_ResultIterator__parse_next_input(struct __pyx_obj_2jq__ResultIterator *__pyx_v_self) {
+  jv __pyx_v_value;
+  jv __pyx_v_error_message;
+  PyObject *__pyx_v_message = NULL;
+  jv __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_parse_next_input", 0);
+
+  /* "jq.pyx":384
+ * 
+ *     cdef inline jv _parse_next_input(self) except *:
  *         cdef jv value = jv_parser_next(self._parser)             # <<<<<<<<<<<<<<
  *         if jv_is_valid(value):
- *             jq_start(self._jq, value, jq_flags)
+ *             return value
  */
   __pyx_v_value = jv_parser_next(__pyx_v_self->_parser);
 
-  /* "jq.pyx":345
- *         cdef int jq_flags = 0
+  /* "jq.pyx":385
+ *     cdef inline jv _parse_next_input(self) except *:
  *         cdef jv value = jv_parser_next(self._parser)
  *         if jv_is_valid(value):             # <<<<<<<<<<<<<<
- *             jq_start(self._jq, value, jq_flags)
- *             return 0
+ *             return value
+ *         elif jv_invalid_has_msg(jv_copy(value)):
  */
   __pyx_t_1 = (jv_is_valid(__pyx_v_value) != 0);
   if (__pyx_t_1) {
 
-    /* "jq.pyx":346
+    /* "jq.pyx":386
  *         cdef jv value = jv_parser_next(self._parser)
  *         if jv_is_valid(value):
- *             jq_start(self._jq, value, jq_flags)             # <<<<<<<<<<<<<<
- *             return 0
- *         elif jv_invalid_has_msg(jv_copy(value)):
- */
-    jq_start(__pyx_v_self->_jq, __pyx_v_value, __pyx_v_jq_flags);
-
-    /* "jq.pyx":347
- *         if jv_is_valid(value):
- *             jq_start(self._jq, value, jq_flags)
- *             return 0             # <<<<<<<<<<<<<<
+ *             return value             # <<<<<<<<<<<<<<
  *         elif jv_invalid_has_msg(jv_copy(value)):
  *             error_message = jv_invalid_get_msg(value)
  */
-    __pyx_r = 0;
+    __pyx_r = __pyx_v_value;
     goto __pyx_L0;
 
-    /* "jq.pyx":345
- *         cdef int jq_flags = 0
+    /* "jq.pyx":385
+ *     cdef inline jv _parse_next_input(self) except *:
  *         cdef jv value = jv_parser_next(self._parser)
  *         if jv_is_valid(value):             # <<<<<<<<<<<<<<
- *             jq_start(self._jq, value, jq_flags)
- *             return 0
+ *             return value
+ *         elif jv_invalid_has_msg(jv_copy(value)):
  */
   }
 
-  /* "jq.pyx":348
- *             jq_start(self._jq, value, jq_flags)
- *             return 0
+  /* "jq.pyx":387
+ *         if jv_is_valid(value):
+ *             return value
  *         elif jv_invalid_has_msg(jv_copy(value)):             # <<<<<<<<<<<<<<
  *             error_message = jv_invalid_get_msg(value)
  *             message = jv_string_to_py_string(error_message)
  */
   __pyx_t_1 = (jv_invalid_has_msg(jv_copy(__pyx_v_value)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "jq.pyx":349
- *             return 0
+    /* "jq.pyx":388
+ *             return value
  *         elif jv_invalid_has_msg(jv_copy(value)):
  *             error_message = jv_invalid_get_msg(value)             # <<<<<<<<<<<<<<
  *             message = jv_string_to_py_string(error_message)
  *             jv_free(error_message)
  */
     __pyx_v_error_message = jv_invalid_get_msg(__pyx_v_value);
 
-    /* "jq.pyx":350
+    /* "jq.pyx":389
  *         elif jv_invalid_has_msg(jv_copy(value)):
  *             error_message = jv_invalid_get_msg(value)
  *             message = jv_string_to_py_string(error_message)             # <<<<<<<<<<<<<<
  *             jv_free(error_message)
  *             raise ValueError(u"parse error: " + message)
  */
-    __pyx_t_2 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_2jq_jv_string_to_py_string(__pyx_v_error_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_message = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "jq.pyx":351
+    /* "jq.pyx":390
  *             error_message = jv_invalid_get_msg(value)
  *             message = jv_string_to_py_string(error_message)
  *             jv_free(error_message)             # <<<<<<<<<<<<<<
  *             raise ValueError(u"parse error: " + message)
  *         else:
  */
     jv_free(__pyx_v_error_message);
 
-    /* "jq.pyx":352
+    /* "jq.pyx":391
  *             message = jv_string_to_py_string(error_message)
  *             jv_free(error_message)
  *             raise ValueError(u"parse error: " + message)             # <<<<<<<<<<<<<<
  *         else:
  *             jv_free(value)
  */
-    __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_parse_error, __pyx_v_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_parse_error, __pyx_v_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 352, __pyx_L1_error)
+    __PYX_ERR(0, 391, __pyx_L1_error)
 
-    /* "jq.pyx":348
- *             jq_start(self._jq, value, jq_flags)
- *             return 0
+    /* "jq.pyx":387
+ *         if jv_is_valid(value):
+ *             return value
  *         elif jv_invalid_has_msg(jv_copy(value)):             # <<<<<<<<<<<<<<
  *             error_message = jv_invalid_get_msg(value)
  *             message = jv_string_to_py_string(error_message)
  */
   }
 
-  /* "jq.pyx":354
+  /* "jq.pyx":393
  *             raise ValueError(u"parse error: " + message)
  *         else:
  *             jv_free(value)             # <<<<<<<<<<<<<<
  *             raise StopIteration()
  * 
  */
   /*else*/ {
     jv_free(__pyx_v_value);
 
-    /* "jq.pyx":355
+    /* "jq.pyx":394
  *         else:
  *             jv_free(value)
  *             raise StopIteration()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_builtin_StopIteration); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_builtin_StopIteration); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 355, __pyx_L1_error)
+    __PYX_ERR(0, 394, __pyx_L1_error)
   }
 
-  /* "jq.pyx":342
- *                 self._ready = False
+  /* "jq.pyx":383
+ *         return 0
  * 
- *     cdef bint _ready_next_input(self) except 1:             # <<<<<<<<<<<<<<
- *         cdef int jq_flags = 0
+ *     cdef inline jv _parse_next_input(self) except *:             # <<<<<<<<<<<<<<
  *         cdef jv value = jv_parser_next(self._parser)
+ *         if jv_is_valid(value):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("jq._ResultIterator._ready_next_input", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 1;
+  __Pyx_AddTraceback("jq._ResultIterator._parse_next_input", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
@@ -7084,15 +7898,15 @@
   __Pyx_AddTraceback("jq._ResultIterator.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":358
+/* "jq.pyx":397
  * 
  * 
  * def all(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).all()
  * 
  */
 
@@ -7142,15 +7956,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "all") < 0)) __PYX_ERR(0, 358, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "all") < 0)) __PYX_ERR(0, 397, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7161,15 +7975,15 @@
     }
     __pyx_v_program = values[0];
     __pyx_v_value = values[1];
     __pyx_v_text = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("all", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 358, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("all", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 397, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq.all", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_2all(__pyx_self, __pyx_v_program, __pyx_v_value, __pyx_v_text);
 
@@ -7187,78 +8001,78 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all", 0);
 
-  /* "jq.pyx":359
+  /* "jq.pyx":398
  * 
  * def all(program, value=_NO_VALUE, text=_NO_VALUE):
  *     return compile(program).input(value, text=text).all()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_program) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_program);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_value);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 359, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_all); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_all); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":358
+  /* "jq.pyx":397
  * 
  * 
  * def all(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).all()
  * 
  */
 
@@ -7273,15 +8087,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":362
+/* "jq.pyx":401
  * 
  * 
  * def first(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).first()
  * 
  */
 
@@ -7331,15 +8145,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "first") < 0)) __PYX_ERR(0, 362, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "first") < 0)) __PYX_ERR(0, 401, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7350,15 +8164,15 @@
     }
     __pyx_v_program = values[0];
     __pyx_v_value = values[1];
     __pyx_v_text = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("first", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 362, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("first", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 401, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq.first", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_4first(__pyx_self, __pyx_v_program, __pyx_v_value, __pyx_v_text);
 
@@ -7376,78 +8190,78 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("first", 0);
 
-  /* "jq.pyx":363
+  /* "jq.pyx":402
  * 
  * def first(program, value=_NO_VALUE, text=_NO_VALUE):
  *     return compile(program).input(value, text=text).first()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_program) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_program);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_value);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_first); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_first); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":362
+  /* "jq.pyx":401
  * 
  * 
  * def first(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).first()
  * 
  */
 
@@ -7462,15 +8276,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":369
+/* "jq.pyx":408
  * 
  * 
  * def iter(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return _iter(compile(program).input(value, text=text))
  * 
  */
 
@@ -7520,15 +8334,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "iter") < 0)) __PYX_ERR(0, 369, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "iter") < 0)) __PYX_ERR(0, 408, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7539,15 +8353,15 @@
     }
     __pyx_v_program = values[0];
     __pyx_v_value = values[1];
     __pyx_v_text = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("iter", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 369, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("iter", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 408, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq.iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_6iter(__pyx_self, __pyx_v_program, __pyx_v_value, __pyx_v_text);
 
@@ -7566,53 +8380,53 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("iter", 0);
 
-  /* "jq.pyx":370
+  /* "jq.pyx":409
  * 
  * def iter(program, value=_NO_VALUE, text=_NO_VALUE):
  *     return _iter(compile(program).input(value, text=text))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_compile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_compile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_program) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_program);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_input); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_input); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_value);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
@@ -7622,22 +8436,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":369
+  /* "jq.pyx":408
  * 
  * 
  * def iter(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return _iter(compile(program).input(value, text=text))
  * 
  */
 
@@ -7653,15 +8467,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":373
+/* "jq.pyx":412
  * 
  * 
  * def text(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).text()
  * 
  */
 
@@ -7711,15 +8525,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_text);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "text") < 0)) __PYX_ERR(0, 373, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "text") < 0)) __PYX_ERR(0, 412, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7730,15 +8544,15 @@
     }
     __pyx_v_program = values[0];
     __pyx_v_value = values[1];
     __pyx_v_text = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("text", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 373, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("text", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 412, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("jq.text", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2jq_8text(__pyx_self, __pyx_v_program, __pyx_v_value, __pyx_v_text);
 
@@ -7756,78 +8570,78 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("text", 0);
 
-  /* "jq.pyx":374
+  /* "jq.pyx":413
  * 
  * def text(program, value=_NO_VALUE, text=_NO_VALUE):
  *     return compile(program).input(value, text=text).text()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_program) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_program);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_value);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_text, __pyx_v_text) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_text); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_text); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":373
+  /* "jq.pyx":412
  * 
  * 
  * def text(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).text()
  * 
  */
 
@@ -7842,15 +8656,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":378
+/* "jq.pyx":417
  * 
  * # Support the 0.1.x API for backwards compatibility
  * def jq(object program):             # <<<<<<<<<<<<<<
  *     return compile(program)
  * 
  */
 
@@ -7875,44 +8689,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jq", 0);
 
-  /* "jq.pyx":379
+  /* "jq.pyx":418
  * # Support the 0.1.x API for backwards compatibility
  * def jq(object program):
  *     return compile(program)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_program) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_program);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":378
+  /* "jq.pyx":417
  * 
  * # Support the 0.1.x API for backwards compatibility
  * def jq(object program):             # <<<<<<<<<<<<<<
  *     return compile(program)
  * 
  */
 
@@ -7925,15 +8739,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "jq.pyx":382
+/* "jq.pyx":421
  * 
  * 
  * cdef unicode jv_string_to_py_string(jv value):             # <<<<<<<<<<<<<<
  *     cdef int length = jv_string_length_bytes(jv_copy(value))
  *     cdef char* string_value = jv_string_value(value)
  */
 
@@ -7944,44 +8758,44 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jv_string_to_py_string", 0);
 
-  /* "jq.pyx":383
+  /* "jq.pyx":422
  * 
  * cdef unicode jv_string_to_py_string(jv value):
  *     cdef int length = jv_string_length_bytes(jv_copy(value))             # <<<<<<<<<<<<<<
  *     cdef char* string_value = jv_string_value(value)
  *     return string_value[:length].decode("utf-8")
  */
   __pyx_v_length = jv_string_length_bytes(jv_copy(__pyx_v_value));
 
-  /* "jq.pyx":384
+  /* "jq.pyx":423
  * cdef unicode jv_string_to_py_string(jv value):
  *     cdef int length = jv_string_length_bytes(jv_copy(value))
  *     cdef char* string_value = jv_string_value(value)             # <<<<<<<<<<<<<<
  *     return string_value[:length].decode("utf-8")
  */
   __pyx_v_string_value = jv_string_value(__pyx_v_value);
 
-  /* "jq.pyx":385
+  /* "jq.pyx":424
  *     cdef int length = jv_string_length_bytes(jv_copy(value))
  *     cdef char* string_value = jv_string_value(value)
  *     return string_value[:length].decode("utf-8")             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_string_value, 0, __pyx_v_length, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_string_value, 0, __pyx_v_length, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "jq.pyx":382
+  /* "jq.pyx":421
  * 
  * 
  * cdef unicode jv_string_to_py_string(jv value):             # <<<<<<<<<<<<<<
  *     cdef int length = jv_string_length_bytes(jv_copy(value))
  *     cdef char* string_value = jv_string_value(value)
  */
 
@@ -8334,17 +9148,20 @@
 
 static PyObject *__pyx_getprop_2jq_8_Program_program_string(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2jq_8_Program_14program_string_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_2jq__Program[] = {
   {"input", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2jq_8_Program_3input, METH_VARARGS|METH_KEYWORDS, 0},
-  {"transform", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2jq_8_Program_7transform, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_2jq_8_Program_9__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_2jq_8_Program_11__setstate_cython__, METH_O, 0},
+  {"input_value", (PyCFunction)__pyx_pw_2jq_8_Program_5input_value, METH_O, 0},
+  {"input_values", (PyCFunction)__pyx_pw_2jq_8_Program_7input_values, METH_O, 0},
+  {"input_text", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2jq_8_Program_9input_text, METH_VARARGS|METH_KEYWORDS, 0},
+  {"transform", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2jq_8_Program_13transform, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_2jq_8_Program_15__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_2jq_8_Program_17__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_2jq__Program[] = {
   {(char *)"program_string", __pyx_getprop_2jq_8_Program_program_string, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -8365,15 +9182,15 @@
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
   #endif
-  __pyx_pw_2jq_8_Program_5__repr__, /*tp_repr*/
+  __pyx_pw_2jq_8_Program_11__repr__, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
@@ -8990,37 +9807,43 @@
   {&__pyx_n_s_JqStatePool, __pyx_k_JqStatePool, sizeof(__pyx_k_JqStatePool), 0, 0, 1, 1},
   {&__pyx_n_s_Lock, __pyx_k_Lock, sizeof(__pyx_k_Lock), 0, 0, 1, 1},
   {&__pyx_n_s_NO_VALUE, __pyx_k_NO_VALUE, sizeof(__pyx_k_NO_VALUE), 0, 0, 1, 1},
   {&__pyx_n_s_Program, __pyx_k_Program, sizeof(__pyx_k_Program), 0, 0, 1, 1},
   {&__pyx_n_s_ProgramWithInput, __pyx_k_ProgramWithInput, sizeof(__pyx_k_ProgramWithInput), 0, 0, 1, 1},
   {&__pyx_n_s_ResultIterator, __pyx_k_ResultIterator, sizeof(__pyx_k_ResultIterator), 0, 0, 1, 1},
   {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
+  {&__pyx_n_s_StringIO, __pyx_k_StringIO, sizeof(__pyx_k_StringIO), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 0},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_bytes_input, __pyx_k_bytes_input, sizeof(__pyx_k_bytes_input), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_compilation_lock, __pyx_k_compilation_lock, sizeof(__pyx_k_compilation_lock), 0, 0, 1, 1},
   {&__pyx_n_s_compile, __pyx_k_compile, sizeof(__pyx_k_compile), 0, 0, 1, 1},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+  {&__pyx_n_s_dump, __pyx_k_dump, sizeof(__pyx_k_dump), 0, 0, 1, 1},
   {&__pyx_n_s_dumps, __pyx_k_dumps, sizeof(__pyx_k_dumps), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
   {&__pyx_n_s_first, __pyx_k_first, sizeof(__pyx_k_first), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_n_s_getvalue, __pyx_k_getvalue, sizeof(__pyx_k_getvalue), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
+  {&__pyx_n_s_input_text, __pyx_k_input_text, sizeof(__pyx_k_input_text), 0, 0, 1, 1},
+  {&__pyx_n_s_input_value, __pyx_k_input_value, sizeof(__pyx_k_input_value), 0, 0, 1, 1},
+  {&__pyx_n_s_io, __pyx_k_io, sizeof(__pyx_k_io), 0, 0, 1, 1},
   {&__pyx_n_s_iter, __pyx_k_iter, sizeof(__pyx_k_iter), 0, 0, 1, 1},
   {&__pyx_n_s_iter_2, __pyx_k_iter_2, sizeof(__pyx_k_iter_2), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_jq, __pyx_k_jq, sizeof(__pyx_k_jq), 0, 0, 1, 1},
   {&__pyx_kp_s_jq_compile_r, __pyx_k_jq_compile_r, sizeof(__pyx_k_jq_compile_r), 0, 0, 1, 0},
   {&__pyx_kp_s_jq_init_failed, __pyx_k_jq_init_failed, sizeof(__pyx_k_jq_init_failed), 0, 0, 1, 0},
   {&__pyx_kp_s_jq_pyx, __pyx_k_jq_pyx, sizeof(__pyx_k_jq_pyx), 0, 0, 1, 0},
@@ -9044,81 +9867,83 @@
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_slurp, __pyx_k_slurp, sizeof(__pyx_k_slurp), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
   {&__pyx_n_s_text_locals_genexpr, __pyx_k_text_locals_genexpr, sizeof(__pyx_k_text_locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_text_output, __pyx_k_text_output, sizeof(__pyx_k_text_output), 0, 0, 1, 1},
   {&__pyx_n_s_threading, __pyx_k_threading, sizeof(__pyx_k_threading), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_utf8, __pyx_k_utf8, sizeof(__pyx_k_utf8), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+  {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 79, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 105, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 374, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "jq.pyx":79
+  /* "jq.pyx":82
  * 
  *     if kind == JV_KIND_INVALID:
  *         raise ValueError("Invalid value")             # <<<<<<<<<<<<<<
  *     elif kind == JV_KIND_NULL:
  *         python_value = None
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Invalid_value); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Invalid_value); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "jq.pyx":145
+  /* "jq.pyx":148
  *     try:
  *         if not jq:
  *             raise Exception("jq_init failed")             # <<<<<<<<<<<<<<
  * 
  *         error_store = _ErrorStore()
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_jq_init_failed); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_jq_init_failed); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "jq.pyx":149
+  /* "jq.pyx":152
  *         error_store = _ErrorStore()
  * 
  *         with _compilation_lock:             # <<<<<<<<<<<<<<
  *             jq_set_error_cb(jq, _store_error, <void*>error_store)
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "jq.pyx":163
+  /* "jq.pyx":166
  * 
  *         if not compiled:
  *             raise ValueError("program was not valid")             # <<<<<<<<<<<<<<
  *     except:
  *         jq_teardown(&jq)
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_program_was_not_valid); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_program_was_not_valid); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -9152,22 +9977,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "jq.pyx":248
+  /* "jq.pyx":251
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):
  *             raise ValueError("Either the value or text argument should be set")             # <<<<<<<<<<<<<<
- *         string_input = text if text is not _NO_VALUE else json.dumps(value)
  * 
+ *         if text is not _NO_VALUE:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Either_the_value_or_text_argumen); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Either_the_value_or_text_argumen); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -9220,96 +10045,96 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "jq.pyx":130
+  /* "jq.pyx":133
  * 
  * 
  * def compile(object program, args=None):             # <<<<<<<<<<<<<<
  *     cdef object program_bytes = program.encode("utf8")
  *     return _Program(program_bytes, args=args)
  */
-  __pyx_tuple__29 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_args, __pyx_n_s_program_bytes); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_args, __pyx_n_s_program_bytes); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_compile, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_compile, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 133, __pyx_L1_error)
 
-  /* "jq.pyx":200
+  /* "jq.pyx":203
  * 
  * 
  * class _EmptyValue(object):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_builtin_object); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
 
-  /* "jq.pyx":358
+  /* "jq.pyx":397
  * 
  * 
  * def all(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).all()
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_all, 358, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_all, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 397, __pyx_L1_error)
 
-  /* "jq.pyx":362
+  /* "jq.pyx":401
  * 
  * 
  * def first(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).first()
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_first, 362, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_first, 401, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 401, __pyx_L1_error)
 
-  /* "jq.pyx":369
+  /* "jq.pyx":408
  * 
  * 
  * def iter(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return _iter(compile(program).input(value, text=text))
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_iter_2, 369, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_iter_2, 408, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 408, __pyx_L1_error)
 
-  /* "jq.pyx":373
+  /* "jq.pyx":412
  * 
  * 
  * def text(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).text()
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_program, __pyx_n_s_value, __pyx_n_s_text); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_text, 373, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_text, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 412, __pyx_L1_error)
 
-  /* "jq.pyx":378
+  /* "jq.pyx":417
  * 
  * # Support the 0.1.x API for backwards compatibility
  * def jq(object program):             # <<<<<<<<<<<<<<
  *     return compile(program)
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_n_s_program); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_n_s_program); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_jq, 378, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_jq_pyx, __pyx_n_s_jq, 417, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -9360,84 +10185,85 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_2jq__ErrorStore = &__pyx_vtable_2jq__ErrorStore;
   __pyx_vtable_2jq__ErrorStore.has_errors = (int (*)(struct __pyx_obj_2jq__ErrorStore *))__pyx_f_2jq_11_ErrorStore_has_errors;
   __pyx_vtable_2jq__ErrorStore.error_string = (PyObject *(*)(struct __pyx_obj_2jq__ErrorStore *))__pyx_f_2jq_11_ErrorStore_error_string;
   __pyx_vtable_2jq__ErrorStore.store_error = (void (*)(struct __pyx_obj_2jq__ErrorStore *, PyObject *))__pyx_f_2jq_11_ErrorStore_store_error;
   __pyx_vtable_2jq__ErrorStore.clear = (void (*)(struct __pyx_obj_2jq__ErrorStore *))__pyx_f_2jq_11_ErrorStore_clear;
-  if (PyType_Ready(&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq__ErrorStore.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq__ErrorStore.tp_dictoffset && __pyx_type_2jq__ErrorStore.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq__ErrorStore.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2jq__ErrorStore.tp_dict, __pyx_vtabptr_2jq__ErrorStore) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ErrorStore, (PyObject *)&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2jq__ErrorStore.tp_dict, __pyx_vtabptr_2jq__ErrorStore) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ErrorStore, (PyObject *)&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ErrorStore) < 0) __PYX_ERR(0, 184, __pyx_L1_error)
   __pyx_ptype_2jq__ErrorStore = &__pyx_type_2jq__ErrorStore;
   __pyx_vtabptr_2jq__JqStatePool = &__pyx_vtable_2jq__JqStatePool;
   __pyx_vtable_2jq__JqStatePool.acquire = (jq_state *(*)(struct __pyx_obj_2jq__JqStatePool *))__pyx_f_2jq_12_JqStatePool_acquire;
   __pyx_vtable_2jq__JqStatePool.release = (void (*)(struct __pyx_obj_2jq__JqStatePool *, jq_state *))__pyx_f_2jq_12_JqStatePool_release;
-  if (PyType_Ready(&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq__JqStatePool.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq__JqStatePool.tp_dictoffset && __pyx_type_2jq__JqStatePool.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq__JqStatePool.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2jq__JqStatePool.tp_dict, __pyx_vtabptr_2jq__JqStatePool) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_JqStatePool, (PyObject *)&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2jq__JqStatePool.tp_dict, __pyx_vtabptr_2jq__JqStatePool) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_JqStatePool, (PyObject *)&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__JqStatePool) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
   __pyx_ptype_2jq__JqStatePool = &__pyx_type_2jq__JqStatePool;
-  if (PyType_Ready(&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq__Program.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq__Program.tp_dictoffset && __pyx_type_2jq__Program.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq__Program.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Program, (PyObject *)&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Program, (PyObject *)&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__Program) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __pyx_ptype_2jq__Program = &__pyx_type_2jq__Program;
   __pyx_vtabptr_2jq__ProgramWithInput = &__pyx_vtable_2jq__ProgramWithInput;
   __pyx_vtable_2jq__ProgramWithInput._make_iterator = (struct __pyx_obj_2jq__ResultIterator *(*)(struct __pyx_obj_2jq__ProgramWithInput *))__pyx_f_2jq_17_ProgramWithInput__make_iterator;
-  if (PyType_Ready(&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq__ProgramWithInput.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq__ProgramWithInput.tp_dictoffset && __pyx_type_2jq__ProgramWithInput.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq__ProgramWithInput.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2jq__ProgramWithInput.tp_dict, __pyx_vtabptr_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ProgramWithInput, (PyObject *)&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2jq__ProgramWithInput.tp_dict, __pyx_vtabptr_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ProgramWithInput, (PyObject *)&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ProgramWithInput) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
   __pyx_ptype_2jq__ProgramWithInput = &__pyx_type_2jq__ProgramWithInput;
   __pyx_vtabptr_2jq__ResultIterator = &__pyx_vtable_2jq__ResultIterator;
   __pyx_vtable_2jq__ResultIterator._ready_next_input = (int (*)(struct __pyx_obj_2jq__ResultIterator *))__pyx_f_2jq_15_ResultIterator__ready_next_input;
-  if (PyType_Ready(&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_vtable_2jq__ResultIterator._parse_next_input = (jv (*)(struct __pyx_obj_2jq__ResultIterator *))__pyx_f_2jq_15_ResultIterator__parse_next_input;
+  if (PyType_Ready(&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq__ResultIterator.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq__ResultIterator.tp_dictoffset && __pyx_type_2jq__ResultIterator.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq__ResultIterator.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2jq__ResultIterator.tp_dict, __pyx_vtabptr_2jq__ResultIterator) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ResultIterator, (PyObject *)&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2jq__ResultIterator.tp_dict, __pyx_vtabptr_2jq__ResultIterator) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ResultIterator, (PyObject *)&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2jq__ResultIterator) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_ptype_2jq__ResultIterator = &__pyx_type_2jq__ResultIterator;
-  if (PyType_Ready(&__pyx_type_2jq___pyx_scope_struct__text) < 0) __PYX_ERR(0, 285, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq___pyx_scope_struct__text) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq___pyx_scope_struct__text.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq___pyx_scope_struct__text.tp_dictoffset && __pyx_type_2jq___pyx_scope_struct__text.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq___pyx_scope_struct__text.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2jq___pyx_scope_struct__text = &__pyx_type_2jq___pyx_scope_struct__text;
-  if (PyType_Ready(&__pyx_type_2jq___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 290, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2jq___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2jq___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2jq___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_2jq___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2jq___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2jq___pyx_scope_struct_1_genexpr = &__pyx_type_2jq___pyx_scope_struct_1_genexpr;
@@ -9690,249 +10516,261 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "jq.pyx":1
+ * import io             # <<<<<<<<<<<<<<
+ * import json
+ * import threading
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_io, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_io, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "jq.pyx":2
+ * import io
  * import json             # <<<<<<<<<<<<<<
  * import threading
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_json, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_json, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_json, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_json, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jq.pyx":2
+  /* "jq.pyx":3
+ * import io
  * import json
  * import threading             # <<<<<<<<<<<<<<
  * 
  * from cpython.bytes cimport PyBytes_AsString
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_threading, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_threading, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_threading, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jq.pyx":130
+  /* "jq.pyx":133
  * 
  * 
  * def compile(object program, args=None):             # <<<<<<<<<<<<<<
  *     cdef object program_bytes = program.encode("utf8")
  *     return _Program(program_bytes, args=args)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_2jq_1compile, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_2jq_1compile, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compile, __pyx_t_1) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compile, __pyx_t_1) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jq.pyx":135
+  /* "jq.pyx":138
  * 
  * 
  * _compilation_lock = threading.Lock()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_threading); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_threading); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compilation_lock, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compilation_lock, __pyx_t_1) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jq.pyx":200
+  /* "jq.pyx":203
  * 
  * 
  * class _EmptyValue(object):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__31); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_tuple__31); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__31, __pyx_n_s_EmptyValue, __pyx_n_s_EmptyValue, (PyObject *) NULL, __pyx_n_s_jq, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_tuple__31, __pyx_n_s_EmptyValue, __pyx_n_s_EmptyValue, (PyObject *) NULL, __pyx_n_s_jq, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_EmptyValue, __pyx_tuple__31, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_EmptyValue, __pyx_tuple__31, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EmptyValue, __pyx_t_3) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EmptyValue, __pyx_t_3) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "jq.pyx":203
+  /* "jq.pyx":206
  *     pass
  * 
  * _NO_VALUE = _EmptyValue()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_EmptyValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_EmptyValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_VALUE, __pyx_t_2) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_VALUE, __pyx_t_2) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":246
+  /* "jq.pyx":249
  *         self._jq_state_pool = _JqStatePool(program_bytes, args=args)
  * 
  *     def input(self, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *         if (value is _NO_VALUE) == (text is _NO_VALUE):
  *             raise ValueError("Either the value or text argument should be set")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__10 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__11 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "jq.pyx":261
+  /* "jq.pyx":279
  * 
  *     # Support the 0.1.x API for backwards compatibility
  *     def transform(self, value=_NO_VALUE, text=_NO_VALUE, text_output=False, multiple_output=False):             # <<<<<<<<<<<<<<
  *         program_with_input = self.input(value, text=text)
  *         if text_output:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__13 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__14 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "jq.pyx":358
+  /* "jq.pyx":397
  * 
  * 
  * def all(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).all()
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__21 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__22 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_3all, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_3all, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_2) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_2) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":362
+  /* "jq.pyx":401
  * 
  * 
  * def first(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).first()
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__23 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__24 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_5first, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_5first, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_first, __pyx_t_2) < 0) __PYX_ERR(0, 362, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_first, __pyx_t_2) < 0) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":366
+  /* "jq.pyx":405
  * 
  * 
  * _iter = iter             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_iter_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter, __pyx_t_2) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter, __pyx_t_2) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":369
+  /* "jq.pyx":408
  * 
  * 
  * def iter(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return _iter(compile(program).input(value, text=text))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__25 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__26 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_7iter, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_7iter, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_2, __pyx_t_2) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_iter_2, __pyx_t_2) < 0) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":373
+  /* "jq.pyx":412
  * 
  * 
  * def text(program, value=_NO_VALUE, text=_NO_VALUE):             # <<<<<<<<<<<<<<
  *     return compile(program).input(value, text=text).text()
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__27 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_VALUE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__28 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_9text, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_9text, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_text, __pyx_t_2) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_text, __pyx_t_2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "jq.pyx":378
+  /* "jq.pyx":417
  * 
  * # Support the 0.1.x API for backwards compatibility
  * def jq(object program):             # <<<<<<<<<<<<<<
  *     return compile(program)
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_11jq, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2jq_11jq, NULL, __pyx_n_s_jq); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jq, __pyx_t_2) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jq, __pyx_t_2) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "jq.pyx":1
- * import json             # <<<<<<<<<<<<<<
+ * import io             # <<<<<<<<<<<<<<
+ * import json
  * import threading
- * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -11053,14 +11891,25 @@
 /* StringJoin */
 #if !CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
     return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
 }
 #endif
 
+/* RaiseKeywordRequired */
+static void __Pyx_RaiseKeywordRequired(const char* func_name, PyObject* kw_name) {
+    PyErr_Format(PyExc_TypeError,
+        #if PY_MAJOR_VERSION >= 3
+        "%s() needs keyword-only argument %U", func_name, kw_name);
+        #else
+        "%s() needs keyword-only argument %s", func_name,
+        PyString_AS_STRING(kw_name));
+        #endif
+}
+
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
@@ -11147,14 +11996,39 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
@@ -11248,39 +12122,14 @@
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
 /* PyObjectGetAttrStrNoError */
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
```

### Comparing `jq-1.4.1/setup.py` & `jq-1.5.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         os.path.join(jq_lib_dir, ".libs/libjq.a"),
         os.path.join(oniguruma_lib_install_dir, "lib/libonig.a"),
     ],
 )
 
 setup(
     name='jq',
-    version='1.4.1',
+    version='1.5.0a1',
     description='jq is a lightweight and flexible JSON processor.',
     long_description=_read("README.rst"),
     author='Michael Williamson',
     url='http://github.com/mwilliamson/jq.py',
     python_requires='>=3.5',
     license='BSD 2-Clause',
     ext_modules = [jq_extension],
```

