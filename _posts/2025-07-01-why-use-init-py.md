---
layout: post
title:  Why Use __init__.py?
date:   2025-07-01
category: python
---

_Explicit is better than implicit._ 

― [The Zen of Python](https://peps.python.org/pep-0020/)

Since Python 3.3, it is possible to create a package without an `__init__.py` file.
However, that does not mean you should. Here are some problems I have encountered.

## Regular vs Namespace Packages

Regular Package:

- A single directory.
- Contains an `__init__.py` file.
- Generally recommended.

Namespace Package:

- A container for subpackages.
- Subpackages may be found in different locations.
- Allows separately installed subpackages to share a parent package.
- No `__init__.py` file.

## Issues With Implicit Namespace Packages

### Not Included In Test Coverage

### Not Found By `pkgutils.itermodules`

### VSCode Does Not Update Modules When Renaming

### Hacky `sys.path` Issues

## How Can I Remember To 