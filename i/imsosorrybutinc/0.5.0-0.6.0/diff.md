# Comparing `tmp/imsosorrybutinc-0.5.0.tar.gz` & `tmp/imsosorrybutinc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsosorrybutinc-0.5.0.tar", last modified: Sun Dec 31 02:09:07 2023, max compression
+gzip compressed data, was "imsosorrybutinc-0.6.0.tar", last modified: Sun Apr  7 15:04:36 2024, max compression
```

## Comparing `imsosorrybutinc-0.5.0.tar` & `imsosorrybutinc-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 02:09:07.004255 imsosorrybutinc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-31 02:09:07.004255 imsosorrybutinc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 02:09:07.004255 imsosorrybutinc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 02:09:07.004255 imsosorrybutinc-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 02:09:07.004255 imsosorrybutinc-0.5.0/src/imsosorrybutinc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-31 02:09:06.000000 imsosorrybutinc-0.5.0/src/imsosorrybutinc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-31 02:09:07.000000 imsosorrybutinc-0.5.0/src/imsosorrybutinc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 02:09:06.000000 imsosorrybutinc-0.5.0/src/imsosorrybutinc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-31 02:09:06.000000 imsosorrybutinc-0.5.0/src/imsosorrybutinc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    53193 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/src/uwuifier.c
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2023-12-31 02:09:00.000000 imsosorrybutinc-0.5.0/src/uwuifier.stringlib.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.359379 imsosorrybutinc-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/src/uwuifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51178 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.c
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/uwuifier.stringlib.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/tests/test_uwuify.py
```

### Comparing `imsosorrybutinc-0.5.0/LICENSE` & `imsosorrybutinc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imsosorrybutinc-0.5.0/src/uwuifier.c` & `imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.c`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     PyErr_SetString(PyExc_ ## err ## Error, msg); \
     return NULL; \
 
 #define FMT_ERROR_RET(err, msg, ...) \
     PyErr_Format(PyExc_ ## err ## Error, msg, __VA_ARGS__); \
     return NULL; \
 
+typedef struct {
+    PyObject *lower__str__;
+} uwuifier_modstate;
+
 LOCAL(unsigned long long)
 rand_ull(void)
 {
     unsigned long long r = 0;
 
     /*
     msb (max)   i*8
@@ -104,27 +108,29 @@
 
 LOCAL(double)
 rand_double(void)
 {
     return rand_to_double(rand_ull());
 }
 
+#define SIZE_ROUND_DOWN(n, a) ((size_t)(n) & ~(size_t)((a) - 1))
+
 /* Generic helper macro to convert characters of different types.
    from_type and to_type have to be valid type names, begin and end
    are pointers to the source characters which should be of type
    "from_type *".  to is a pointer of type "to_type *" and points to the
    buffer where the result characters are written to. */
-#define _PyUnicode_CONVERT_BYTES(from_type, to_type, begin, end, to) \
+#define CONVERT_BYTES(from_type, to_type, begin, end, to) \
     do {                                                \
         to_type *_to = (to_type *)(to);                 \
         const from_type *_iter = (const from_type *)(begin);\
         const from_type *_end = (const from_type *)(end);\
         Py_ssize_t n = (_end) - (_iter);                \
         const from_type *_unrolled_end =                \
-            _iter + _Py_SIZE_ROUND_DOWN(n, 4);          \
+            _iter + SIZE_ROUND_DOWN(n, 4);              \
         while (_iter < (_unrolled_end)) {               \
             _to[0] = (to_type) _iter[0];                \
             _to[1] = (to_type) _iter[1];                \
             _to[2] = (to_type) _iter[2];                \
             _to[3] = (to_type) _iter[3];                \
             _iter += 4; _to += 4;                       \
         }                                               \
@@ -168,14 +174,16 @@
 #undef STRINGLIB_CHAR
 #undef STRINGLIB_FAST_MEMCHR
 
 LOCAL(Py_UCS4)
 any_getchar(const void *s, const Py_ssize_t i,
             const int kind)
 {
+    /* We have to not use PyUnicode_READ() here,
+       since we need to allow negative (backward) indexes. */
     switch (kind) {
     case PyUnicode_1BYTE_KIND:
         return ((const Py_UCS1 *)s)[i];
     case PyUnicode_2BYTE_KIND:
         return ((const Py_UCS2 *)s)[i];
     case PyUnicode_4BYTE_KIND:
         return ((const Py_UCS4 *)s)[i];
@@ -184,81 +192,40 @@
     }
 }
 
 LOCAL(void)
 any_setchar(void *s, const Py_ssize_t i,
             const Py_UCS4 x, const int kind)
 {
-    switch (kind) {
-    case PyUnicode_1BYTE_KIND:
-        ((Py_UCS1 *)s)[i] = x;
-        break;
-    case PyUnicode_2BYTE_KIND:
-        ((Py_UCS2 *)s)[i] = x;
-        break;
-    case PyUnicode_4BYTE_KIND:
-        ((Py_UCS4 *)s)[i] = x;
-        break;
-    default:
-        ASSUME(0);
-    }
+    PyUnicode_WRITE(kind, s, i, x);
 }
 
 LOCAL(int)
 any_charisalpha(const void *s, const Py_ssize_t i,
                 const int kind)
 {
-    switch (kind) {
-    case PyUnicode_1BYTE_KIND:
-        return isalpha(((const Py_UCS1 *)s)[i]);
-    case PyUnicode_2BYTE_KIND:
-        return isalpha(((const Py_UCS2 *)s)[i]);
-    case PyUnicode_4BYTE_KIND:
-        return isalpha(((const Py_UCS4 *)s)[i]);
-    default:
-        ASSUME(0);
-    }
+    return Py_UNICODE_ISALPHA(PyUnicode_READ(kind, s, i));
 }
 
 LOCAL(int)
 any_charisword(const void *s, const Py_ssize_t i,
                const int kind)
 {
-    int ch;
-    switch (kind) {
-    case PyUnicode_1BYTE_KIND:
-        ch = ((const Py_UCS1 *)s)[i];
-        if (ch < 128) return isalnum(ch) || ch == '_';
-        break;
-    case PyUnicode_2BYTE_KIND:
-        ch = ((const Py_UCS2 *)s)[i];
-        break;
-    case PyUnicode_4BYTE_KIND:
-        ch = ((const Py_UCS4 *)s)[i];
-        break;
-    default:
-        ASSUME(0);
+    Py_UCS4 ch = any_getchar(s, i, kind);
+    if (ch < 128) {
+        return Py_UNICODE_ISALNUM(ch) || ch == '_';
     }
-    return _PyUnicode_IsAlpha(ch) || _PyUnicode_IsNumeric(ch);
+    return Py_UNICODE_ISALPHA(ch) || Py_UNICODE_ISNUMERIC(ch);
 }
 
 LOCAL(int)
 any_checkchar(const void *s, const Py_ssize_t i,
               const Py_UCS4 x, const int kind)
 {
-    switch (kind) {
-    case PyUnicode_1BYTE_KIND:
-        return ((Py_UCS1 *)s)[i] == x;
-    case PyUnicode_2BYTE_KIND:
-        return ((Py_UCS2 *)s)[i] == x;
-    case PyUnicode_4BYTE_KIND:
-        return ((Py_UCS4 *)s)[i] == x;
-    default:
-        ASSUME(0);
-    }
+    return any_getchar(s, i, kind) == x;
 }
 
 #define CASE(x, cond, handle) \
     case PyUnicode_##x##BYTE_KIND: { \
         Py_UCS##x *buf = (Py_UCS##x *)s; \
         for (Py_ssize_t i = 0; i < n; i++) { \
             if (cond) { \
@@ -418,25 +385,25 @@
     void *result;
 
     switch (kind) {
     case PyUnicode_2BYTE_KIND:
         result = PyMem_New(Py_UCS2, len);
         if (UNLIKELY(!result))
             return PyErr_NoMemory();
-        _PyUnicode_CONVERT_BYTES(
+        CONVERT_BYTES(
             Py_UCS1, Py_UCS2,
             (const Py_UCS1 *)data,
             ((const Py_UCS1 *)data) + len,
             result);
         return result;
     case PyUnicode_4BYTE_KIND:
         result = PyMem_New(Py_UCS4, len);
         if (UNLIKELY(!result))
             return PyErr_NoMemory();
-        _PyUnicode_CONVERT_BYTES(
+        CONVERT_BYTES(
             Py_UCS1, Py_UCS4,
             (const Py_UCS1 *)data,
             ((const Py_UCS1 *)data) + len,
             result);
         return result;
     default:
         ASSUME(0);
@@ -446,34 +413,34 @@
 LOCAL(void)
 copy_fromLE_toU2p(const void *from, void *to, Py_ssize_t len,
                   int kind0, int kind1)
 {
     switch (kind0) {
     case PyUnicode_1BYTE_KIND:
         if (kind1 == PyUnicode_2BYTE_KIND) {
-            _PyUnicode_CONVERT_BYTES(
+            CONVERT_BYTES(
                 Py_UCS1, Py_UCS2,
                 from,
                 ((const Py_UCS1 *)from) + len,
                 to);
         }
         else {
-            _PyUnicode_CONVERT_BYTES(
+            CONVERT_BYTES(
                 Py_UCS1, Py_UCS4,
                 from,
                 ((const Py_UCS1 *)from) + len,
                 to);
         }
         break;
     case PyUnicode_2BYTE_KIND:
         if (kind1 == PyUnicode_2BYTE_KIND) {
             memcpy(to, from, len + len);
         }
         else {
-            _PyUnicode_CONVERT_BYTES(
+            CONVERT_BYTES(
                 Py_UCS2, Py_UCS4,
                 from,
                 ((const Py_UCS2 *)from) + len,
                 to);
         }
         break;
     case PyUnicode_4BYTE_KIND:
@@ -486,138 +453,32 @@
 
 LOCAL(void)
 copy_fromU2p_to1B(const void *from, void *to, Py_ssize_t len,
                   int kind)
 {
     switch (kind) {
     case PyUnicode_2BYTE_KIND:
-        _PyUnicode_CONVERT_BYTES(
+        CONVERT_BYTES(
             Py_UCS2, Py_UCS1,
             from,
             ((const Py_UCS2 *)from) + len,
             to);
         break;
     case PyUnicode_4BYTE_KIND:
-        _PyUnicode_CONVERT_BYTES(
+        CONVERT_BYTES(
             Py_UCS4, Py_UCS1,
             from,
             ((const Py_UCS4 *)from) + len,
             to);
         break;
     default:
         ASSUME(0);
     }
 }
 
-LOCAL(Py_UCS4)
-handle_capital_sigma(int kind, const void *data, Py_ssize_t length, Py_ssize_t i)
-{
-    Py_ssize_t j;
-    int final_sigma;
-    Py_UCS4 c = 0;   /* initialize to prevent gcc warning */
-    /* U+03A3 is in the Final_Sigma context when, it is found like this:
-
-     \p{cased}\p{case-ignorable}*U+03A3!(\p{case-ignorable}*\p{cased})
-
-    where ! is a negation and \p{xxx} is a character with property xxx.
-    */
-    for (j = i - 1; j >= 0; j--) {
-        c = PyUnicode_READ(kind, data, j);
-        if (!_PyUnicode_IsCaseIgnorable(c))
-            break;
-    }
-    if ((final_sigma = j >= 0 && _PyUnicode_IsCased(c))) {
-        for (j = i + 1; j < length; j++) {
-            c = PyUnicode_READ(kind, data, j);
-            if (!_PyUnicode_IsCaseIgnorable(c))
-                break;
-        }
-        final_sigma = j == length || !_PyUnicode_IsCased(c);
-    }
-    return final_sigma ? 0x3C2 : 0x3C3;
-}
-
-LOCAL(int)
-lower_ucs4(int kind, const void *data, Py_ssize_t length, Py_ssize_t i,
-           Py_UCS4 c, Py_UCS4 *mapped)
-{
-    /* Obscure special case. */
-    if (c == 0x3A3) {
-        mapped[0] = handle_capital_sigma(kind, data, length, i);
-        return 1;
-    }
-    return _PyUnicode_ToLowerFull(c, mapped);
-}
-
-LOCAL(Py_ssize_t)
-do_lower(int kind, const void *data, Py_ssize_t length, Py_UCS4 *res,
-         Py_UCS4 *maxchar)
-{
-    Py_ssize_t i, k = 0;
-
-    for (i = 0; i < length; i++) {
-        Py_UCS4 c = PyUnicode_READ(kind, data, i), mapped[3];
-        int n_res, j;
-        if (UNLIKELY(c == 0x3A3)) {
-            mapped[0] = handle_capital_sigma(kind, data, length, i);
-            n_res = 1;
-        }
-        else {
-            n_res = _PyUnicode_ToLowerFull(c, mapped);
-        }
-        for (j = 0; j < n_res; j++) {
-            *maxchar = Py_MAX(*maxchar, mapped[j]);
-            res[k++] = mapped[j];
-        }
-    }
-    return k;
-}
-
-LOCAL(PyObject *)
-case_lower(PyObject *self)
-{
-    PyObject *res;
-    Py_ssize_t length, newlength;
-    int kind, outkind;
-    const void *data;
-    void *outdata;
-    Py_UCS4 maxchar = 0, *tmp, *tmpend;
-
-    kind = PyUnicode_KIND(self);
-    data = PyUnicode_DATA(self);
-    length = PyUnicode_GET_LENGTH(self);
-    if (UNLIKELY((size_t) length > PY_SSIZE_T_MAX / (3 * sizeof(Py_UCS4)))) {
-        SET_ERROR_RET(Overflow, "string is too long");
-    }
-    tmp = PyMem_Malloc(sizeof(Py_UCS4) * 3 * length);
-    if (UNLIKELY(tmp == NULL)) return PyErr_NoMemory();
-    newlength = do_lower(kind, data, length, tmp, &maxchar);
-    res = PyUnicode_New(newlength, maxchar);
-    if (UNLIKELY(res == NULL)) goto leave;
-    tmpend = tmp + newlength;
-    outdata = PyUnicode_DATA(res);
-    outkind = PyUnicode_KIND(res);
-    switch (outkind) {
-    case PyUnicode_1BYTE_KIND:
-        _PyUnicode_CONVERT_BYTES(Py_UCS4, Py_UCS1, tmp, tmpend, outdata);
-        break;
-    case PyUnicode_2BYTE_KIND:
-        _PyUnicode_CONVERT_BYTES(Py_UCS4, Py_UCS2, tmp, tmpend, outdata);
-        break;
-    case PyUnicode_4BYTE_KIND:
-        memcpy(outdata, tmp, sizeof(Py_UCS4) * newlength);
-        break;
-    default:
-        Py_UNREACHABLE();
-    }
-  leave:
-    PyMem_Free(tmp);
-    return res;
-}
-
 LOCAL(PyObject *)
 word_replace_impl(PyObject *text)
 {
     Py_ssize_t maxchar, i, j, ires, sn, n, n2, new_size;
     int r1 = 0, r2 = 0, resr = 0;
     int kind;
     char *res;
@@ -1658,16 +1519,31 @@
 }
 
 PyDoc_STRVAR(tildify__doc__,
 "tildify(text: str, strength: float = 0.0) -> str\n\
 \n\
     Adds some tildes to spaces.\n");
 
+/* Here we could use _PyLong_Sign() or other easy stuff from CPython to be
+   faster, but of course it's totally taboo to have private, unstable,
+   implementation-dependent functions. grr. ¬∧¬ */
+LOCAL(int)
+long_sign(PyObject *l)
+{
+    PyObject *zero = PyLong_FromLong(0L);
+    if (UNLIKELY(zero == NULL)) {
+        return -1;
+    }
+    int res = PyObject_RichCompareBool(l, zero, Py_GT);
+    Py_DECREF(zero);
+    return res;
+}
+
 static PyObject *
-uwuify(PyObject *Py_UNUSED(_),
+uwuify(PyObject *module,
        PyObject *const *args,
        Py_ssize_t nargs,
        PyObject *kwnames)
 {
     int has_t = 0, has_SS = 0, has_ES = 0, has_TS = 0, nochange = 1;
     float SS = 0.2, ES = 0.1, TS = 0.1;
     PyObject *text, *SS_o = NULL, *ES_o = NULL, *TS_o = NULL;
@@ -1733,61 +1609,73 @@
     else {
         text = args[0];
         goto skip_keyarg_checks;
     }
 
     if (has_SS) {
         if (PyLong_CheckExact(SS_o)) {
-            SS = _PyLong_Sign(SS_o) > 0 ? 1. : 0.;
+            int sign = long_sign(SS_o);
+            if (sign == -1) {
+                 return NULL;
+            }
+            SS = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(SS_o)) {
             SS = PyFloat_AS_DOUBLE(SS_o);
         }
         else {
             FMT_ERROR_RET(Type,
-                          "'tildify' expected 'float' for 'stutter_strength' "
+                          "'uwuify' expected 'float' for 'stutter_strength' "
                           "argument, got '%.200s'",
                           Py_TYPE(SS_o)->tp_name);
         }
     }
 
     if (has_ES) {
         if (PyLong_CheckExact(ES_o)) {
-            ES = _PyLong_Sign(ES_o) > 0 ? 1. : 0.;
+            int sign = long_sign(ES_o);
+            if (sign == -1) {
+                 return NULL;
+            }
+            ES = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(ES_o)) {
             ES = PyFloat_AS_DOUBLE(ES_o);
         }
         else {
             FMT_ERROR_RET(Type,
-                          "'tildify' expected 'float' for 'emoji_strength' "
+                          "'uwuify' expected 'float' for 'emoji_strength' "
                           "argument, got '%.200s'",
                           Py_TYPE(ES_o)->tp_name);
         }
     }
 
     if (has_TS) {
         if (PyLong_CheckExact(TS_o)) {
-            TS = _PyLong_Sign(TS_o) > 0 ? 1. : 0.;
+            int sign = long_sign(TS_o);
+            if (sign == -1) {
+                 return NULL;
+            }
+            TS = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(TS_o)) {
             TS = PyFloat_AS_DOUBLE(TS_o);
         }
         else {
             FMT_ERROR_RET(Type,
-                          "'tildify' expected 'float' for 'tilde_strength' "
+                          "'uwuify' expected 'float' for 'tilde_strength' "
                           "argument, got '%.200s'",
                           Py_TYPE(TS_o)->tp_name);
         }
     }
 
 skip_keyarg_checks:
     if (!PyUnicode_CheckExact(text)) {
         FMT_ERROR_RET(Type,
-                      "'tildify' expected 'str' for 'text' argument, "
+                      "'uwuify' expected 'str' for 'text' argument, "
                       "got '%.200s'",
                       Py_TYPE(text)->tp_name);
     }
 
 #define DO_FUNC(func, ...) \
     tmp = func(__VA_ARGS__); \
     if (UNLIKELY(tmp == NULL)) { \
@@ -1795,15 +1683,17 @@
         return NULL; \
     } \
     if (text != tmp) { \
         nochange = 0; \
         Py_SETREF(text, tmp); \
     }
 
-    PyObject *tmp = case_lower(text);
+    uwuifier_modstate *state = PyModule_GetState(module);
+    assert(state != NULL);
+    PyObject *tmp = PyObject_CallMethodNoArgs(text, state->lower__str__);
     if (UNLIKELY(tmp == NULL)) return NULL;
     text = tmp;
 
     DO_FUNC(word_replace_impl, text)
     DO_FUNC(nyaify_impl, text)
     DO_FUNC(char_replace_impl, text)
     DO_FUNC(stutter_impl, text, &SS)
@@ -1833,47 +1723,87 @@
 }
 
 PyDoc_STRVAR(uwuify__doc__,
 "uwuify(text: str, *, stutter_strength: float = 0.2,\n\
                       emoji_strength: float = 0.1,\n\
                       tilde_strength: float = 0.1) -> str\n\
 \n\
-    Takes a string and returns an uwuified version of it.\n");
+    Takes a string and returns a lowercased, uwuified version of it.\n\
+    The strength parameters are in the [0, 1] range. Anything higher\n\
+    or lower will be clamped to their respective limit.\n");
 
 #define METH_O_DOC(name) \
     { #name, (PyCFunction)name, METH_O, name##__doc__ },
 
 #define METH_FAST_KEYWORDS_DOC(name) \
     { #name, (PyCFunction)name, METH_FASTCALL | METH_KEYWORDS, \
       name##__doc__ },
 
+static int
+uwuifier_exec(PyObject *module)
+{
+    uwuifier_modstate *state = PyModule_GetState(module);
+    assert(state != NULL);
+    state->lower__str__ = PyUnicode_InternFromString("lower");
+    if (state->lower__str__ == NULL) {
+        return -1;
+    }
+    return 0;
+}
+
+static int
+uwuifier_clear(PyObject *module)
+{
+    uwuifier_modstate *state = PyModule_GetState(module);
+    assert(state != NULL);
+    Py_CLEAR(state);
+    return 0;
+}
+
+static void
+uwuifier_free(void *module)
+{
+    uwuifier_clear((PyObject *)module);
+}
+
 static PyMethodDef uwuifier_methods[] = {
     METH_O_DOC(word_replace)
     METH_O_DOC(nyaify)
     METH_O_DOC(char_replace)
 
     METH_FAST_KEYWORDS_DOC(stutter)
     METH_FAST_KEYWORDS_DOC(emoji)
     METH_FAST_KEYWORDS_DOC(tildify)
     METH_FAST_KEYWORDS_DOC(uwuify)
 
     {NULL}
 };
 
+static PyModuleDef_Slot uwuifier_slots[] = {
+    {Py_mod_exec, uwuifier_exec},
+
+/* 3.12 feature. */
+#if !defined(Py_LIMITED_API) && Py_VERSION_HEX >= 0x030c0000 \
+        || Py_LIMITED_API+0 >= 0x030c0000
+    {Py_mod_multiple_interpreters, Py_MOD_PER_INTERPRETER_GIL_SUPPORTED},
+#endif
+
+    {0, NULL}
+};
+
 static struct PyModuleDef uwuifiermodule = {
     PyModuleDef_HEAD_INIT,
-    "uwuifier",
-    ":3",
-    0,
-    uwuifier_methods,
-    NULL,
-    NULL,
-    NULL,
-    NULL
+    .m_name = "_uwuifier",
+    .m_doc = ":3",
+    .m_size = sizeof(uwuifier_modstate),
+    .m_methods = uwuifier_methods,
+    .m_slots = uwuifier_slots,
+    .m_clear = uwuifier_clear,
+    .m_free = uwuifier_free,
 };
 
 PyMODINIT_FUNC
-PyInit_uwuifier(void)
+PyInit__uwuifier(void)
 {
     srand((unsigned)time(NULL));
-    return PyModule_Create(&uwuifiermodule);
+    return PyModuleDef_Init(&uwuifiermodule);
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imsosorrybutinc-0.5.0/src/uwuifier.stringlib.h` & `imsosorrybutinc-0.6.0/src/uwuifier/uwuifier.stringlib.h`

 * *Files identical despite different names*

