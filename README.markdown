Compat
======

Manages Ruby 1.9 and 1.8 compatibility in a single header file

Features
--------

* Detects version based on existence of `ROBJECT_EMBED_LEN_MAX` macro
* `RCLASS_M_TBL` / `RCLASS_SUPER` / `RCLASS_IV_TBL`
* Automatically includes st.h
* Creates a `create_class(VALUE flags, VALUE klass)` function to
  manage creation in both versions
* Defines a `KLASS_OF(obj)` macro, (lvalue version of `CLASS_OF`)
* Defines FALSE and TRUE macros

