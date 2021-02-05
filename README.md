# Multi Language in ConTeXt

[![CI](https://github.com/lrusso96/multi-language-context/workflows/CI/badge.svg)](https://github.com/lrusso96/multi-language-context/actions?query=workflow%3ACI)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

This repository is an attempt to set-up a multilanguage environment to typeset ConTeXt documents.

## Rationale

Rather than a matter of a semi-automatic process, most documents need to be carefully adjusted when translated. Then, we cannot merely store a dictionary of key-values, where we use the locale as a key for the correct translation.

## My approach

I use a simple trick to achieve multilanguage support: **Modes**. Each locale becomes a mode that can be activated at compilation time to produce the desired version.

### How to compile

Run

```bash
context --mode=[LOCALE] --result=[LOCALE]
```

For example, to produce the English version of the document, run:

```bash
context --mode=english --result=english
```
