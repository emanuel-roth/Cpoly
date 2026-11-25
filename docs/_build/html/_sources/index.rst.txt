=====
CPoly
=====

`CPoly` is a SageMath package for complementary polyhedra, available `here <https://github.com/emanuel-roth/CPolyhedraTools>`_. It computes their stability conditions, numerical invariants, degrees, canonical facets and Jordan-Hölder facets, following Kai Behrend's paper on `Semi-stability for reductive group schemes <https://link.springer.com/article/10.1007/BF01446630>`_. The Jordan-Hölder theory aspects and extensions are following Section 2 of `this paper <https://arxiv.org/abs/2609.17231>`_.

We were inspired by `QuiverCombinatoricsTools <https://quivercombinatoricstools.github.io/>`_.

To install it, run

.. code-block::

   sage --pip install git+https://github.com/emanuel-roth/CPolyhedraTools.git

and then you can simply run

.. code-block:: python

   from cpoly import *

to get started.

**Author**

* `Emanuel Roth <https://emanuel-roth.github.io/>`_ (University of Edinburgh), using `ChatGPT <https://chatgpt.com/>`_ and `claude <https://claude.com/>`_.

Documentation
=============

.. autofunction:: cpoly.cpoly.greater_than

.. autoclass:: cpoly.cpoly.RootSystem
   :members:
   :no-inherited-members:
   :member-order: bysource
