=====
CPoly
=====

`CPoly` is a SageMath package for complementary polyhedra, available here `https://github.com/emanuel-roth/CPoly <https://github.com/emanuel-roth/CPoly>`_. It computes their stability conditions, numerical invariants, degrees, canonical facets and Jordan-Hölder facets, following Kai Behrend's paper on `Semi-stability for reductive group schemes <https://link.springer.com/article/10.1007/BF01446630>`_. The Jordan-Hölder theory aspects and extensions are following Section 2 of `this paper <https://arxiv.org/abs/2609.17231>`_.

We were inspired by `QuiverCombinatoricsTools <https://quivercombinatoricstools.github.io/>`_.

To install it, run

.. code-block::

   sage --pip install git+https://github.com/emanuel-roth/CPoly.git

and then, to get started, import everything needed from Sage followed by `CPoly`

.. code-block:: python

   from sage.all import *
   from cpoly import *

The first line loads the SageMath environment (root systems, weight lattices, rationals ``QQ``, etc.), which is needed when working outside the interactive ``sage`` prompt, e.g. in a Python script or a Jupyter notebook with a Python kernel. Inside a ``sage`` session it is already loaded, but it does no harm to run it.

.. note::

   The order matters: ``cpoly`` provides its own ``RootSystem`` class extending Sage's. Importing ``from sage.all import *`` *after* ``from cpoly import *`` would overwrite it with Sage's ``RootSystem``, and the `CPoly` methods would not be available.

**Author**

* `Emanuel Roth <https://emanuel-roth.github.io/>`_ (University of Edinburgh), mostly vibecoded with `ChatGPT <https://chatgpt.com/>`_ and `claude <https://claude.com/>`_.

**How to cite CPoly**

If you have used this code in any way, please consider citing it in the following way.

.. code-block:: bibtex

   @software{cpoly,
      author = {Roth, Emanuel},
      title = {CPoly},
      url = {https://emanuel-roth.github.io/Cpoly/},
   }

Documentation
=============

.. autofunction:: cpoly.cpoly.greater_than

.. autoclass:: cpoly.cpoly.RootSystem
   :members:
   :no-inherited-members:
   :member-order: bysource
