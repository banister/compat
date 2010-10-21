Compat
======

Manages Ruby 1.9 and 1.8 compatibility in a single header file

Features
--------

* Detects version based on existence of `ROBJECT_EMBED_LEN_MAX` macro
* Defines `RCLASS_M_TBL` / `RCLASS_SUPER` / `RCLASS_IV_TBL` for 1.8
* Automatically includes `st.h`
* Creates a `create_class(VALUE flags, VALUE klass)` function to
  manage creation in both versions
* Defines a `KLASS_OF(obj)` macro, (lvalue version of `CLASS_OF`)
* Defines FALSE and TRUE macros

