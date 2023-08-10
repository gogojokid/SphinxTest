Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

.. cpp:type:: std::vector<int> CustomList

   A typedef-like declaration of type.

Cross-referencing Python objects
================================

The ``kind`` parameter should be either ``"meat"``, ``"fish"``, 
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

Cross reference to :cpp:type:`CustomList`.

Exception
=========

.. autoexception:: lumache.InvalidKindError

Doctests
========

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']
