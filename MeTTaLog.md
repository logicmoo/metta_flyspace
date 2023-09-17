
# MeTTaLog: An Implementation of MeTTa for Logic Programming

## Overview

MeTTaLog is a novel logic programming framework inspired by OpenCog Hyperon's MeTTa (Meta Type Talk) language. This project aims to provide a rich set of features, including meta-language capabilities, various types of inference, and clear semantics. MeTTaLog is designed to serve as a practical tool for both research and applications in artificial intelligence, semantic web, natural language processing, and beyond.

## Introduction

MeTTaLog is a language designed to be a successor to OpenCog Classic Atomese. It forms part of the OpenCog Hyperon initiative, with clear semantics supporting meta-language features, different types of inference, and more.

## Prerequisites

- SWI-Prolog
- Python 3.x

## Installation

### Installing Required SWI-Prolog Packs

Before you install MeTTaLog, open your SWI-Prolog terminal and install the Janus Python Bridge and logimcoo_utils packs:

```prolog

 % Utility Code used throughout this library
?- pack_install(logicmoo_utils).

 % OOP thru Prolog Dicts
?- pack_install(dictoo).

```

### Main Installation Steps

```bash
# Clone the repository
git clone https://github.com/logicmoo/metta-vspace.git

# Navigate into the directory
cd metta-vspace

# To start the first unit test, run:
./Metta examples/compat/test_scripts/00_lang_case.metta

# To run all:
./Metta examples/compat/test_scripts/*.metta

```


```bash
```

## Getting Started

To get familiar with MeTTaLog, you may:

## Documentation
1. Read the [MeTTaLog specification](https://wiki.opencog.org/wikihome/images/b/b7/MeTTa_Specification.pdf).
2. Learn the [Minimal instruction set](https://github.com/trueagi-io/hyperon-experimental/blob/main/docs/minimal-metta.md)

3. Browse through examples located in

- [00_lang_case.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/00_lang_case.html)
- [00_lang_ok_to_redefine.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/00_lang_ok_to_redefine.html)
- [01_lang_inc.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/01_lang_inc.html)
- [02-curried-plus.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/02-curried-plus.html)
- [03-soring-via-insert.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/03-soring-via-insert.html)
- [_e2_states_dia.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/_e2_states_dia.html)
- [a1_symbols.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/a1_symbols.html)
- [a2_opencoggy.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/a2_opencoggy.html)
- [a3_twoside.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/a3_twoside.html)
- [b0_chaining_prelim.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b0_chaining_prelim.html)
- [b1_equal_chain.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b1_equal_chain.html)
- [b2_backchain.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b2_backchain.html)
- [b3_direct.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b3_direct.html)
- [b4_nondeterm.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b4_nondeterm.html)
- [b5_types_prelim.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/b5_types_prelim.html)
- [c1_grounded_basic.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/c1_grounded_basic.html)
- [c2_spaces.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/c2_spaces.html)
- [c2_spaces_kb.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/c2_spaces_kb.html)
- [c3_pln_stv.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/c3_pln_stv.html)
- [d1_gadt.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/d1_gadt.html)
- [d2_higherfunc.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/d2_higherfunc.html)
- [d3_deptypes.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/d3_deptypes.html)
- [d4_type_prop.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/d4_type_prop.html)
- [d5_auto_types.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/d5_auto_types.html)
- [e1_kb_write.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/e1_kb_write.html)
- [e2_states.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/e2_states.html)
- [e3_match_states.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/e3_match_states.html)
- [f1_imports.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/f1_imports.html)
- [f1_moduleA.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/f1_moduleA.html)
- [f1_moduleB.html](https://htmlpreview.github.io/?https://raw.githubusercontent.com/logicmoo/vspace-metta/main/examples/compat/test_scripts/f1_moduleB.html)





## License

This project is licensed under the GNU Lesser General Public License v3.0 - see the [`LICENSE.md`](LICENSE.md) file for details.

## Acknowledgments

Special thanks to the OpenCog community and everyone involved in the development and conceptualization of Hyperon and MeTTa.

---

