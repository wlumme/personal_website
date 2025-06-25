---
layout: post
title:  Why Use __init__.py?
date:   2025-07-01
category: python
---

_Explicit is better than implicit._ 

― [The Zen of Python](https://peps.python.org/pep-0020/)

If you've ever looked at a Python codebase containing multiple packages, you may have
noticed some empty files named `__init__.py`.

A quick Google search (or question for your preferred LLM) will reveal that TODO

Hang on, my imports work just fine without these empty files cluttering my codebase!

While Python allows packages to exist without an `__init__.py` as of version TODO, there
actually 2 different kinds of packages: TODO and Implicit Namespace Packages.

## What's An Implicit Namespace Package?



## Issues With Implicit Namespace Packages

### Not Included In Test Coverage

### Not Found By `pkgutils.itermodules`

### VSCode Does Not Update Modules When Renaming

### Hacky `sys.path` Issues

## How Can I Remember To 