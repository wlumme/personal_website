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

Namespace Package:

- A container for subpackages.
- Subpackages may be found in different locations.
- Allows separately installed subpackages to share a parent package.
- No `__init__.py` file.

Although it is generally recommended to use regular packages, it can be easy to forget
the `__init__.py` file.

## Issues With Implicit Namespace Packages

You can find examples for all of these examples [here]().

### Not Included In Test Coverage

Consider a project with the following structure:

```
project/
    namespace_package/
        foo.py
    regular_package/
        __init__.py
        bar.py
tests/
```



### Not Found By `pkgutils.itermodules`

### Hacky `sys.path` Issues

### VSCode Does Not Update Modules When Renaming

## How Can I Remember To 