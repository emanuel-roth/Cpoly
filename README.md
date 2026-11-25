<p align="center">
  <img src="cpolylogo.svg#gh-light-mode-only" width="300" alt="logo" />
  <img src="cpolylogodark.svg#gh-dark-mode-only" width="300" alt="logo" />
</p>
 

*CPoly* is a *SageMath* package that adds functionality for complementary polyhedra, calculating their stability conditions, numerical invariants, degrees, and special facets as well as Jordan-Hölder facets. This is based on Kai Behrend's paper on [Semi-stability for reductive group schemes](https://link.springer.com/article/10.1007/BF01446630), and the author's paper on [Jordan-Hölder theory for complementary polyhedra and moduli of parahoric Higgs torsors](https://arxiv.org/abs/2609.17231).

# Author

[Emanuel Roth](https://emanuel-roth.github.io/) (University of Edinburgh), mostly vibecoded with [ChatGPT](https://chatgpt.com/) and [claude](https://claude.com/>).

# Instructions

To install it, make sure you have CPoly
```
sage --pip install git+https://github.com/emanuel-roth/CPoly.git
```
and then, to get started, import everything needed from Sage followed by *CPoly*:
```
from sage.all import *
from cpoly import *
```
The first line loads the SageMath environment, which is needed when working outside the interactive `sage` prompt (e.g. in a Python script or a notebook with a Python kernel); inside a `sage` session it is already loaded but harmless to run.

**Note:** the order matters. *CPoly* provides its own `RootSystem` class extending Sage's, so running `from sage.all import *` *after* `from cpoly import *` would overwrite it with Sage's `RootSystem`.

Alternatively, you can run it from your browser in a notebook here using binder.

# Documentation

You can read the documentation of *CPoly* as:

* a [webpage](https://emanuel-roth.github.io/cpoly/)
* a [pdf](docs/_static/cpoly.pdf)

# How to cite CPoly

If you have used this code in any way, please consider citing it in the following way.
```
@software{cpoly,
  author = {Roth, Emanuel},
  title = {CPoly},
  url = {https://emanuel-roth.github.io/Cpoly/},
}
```