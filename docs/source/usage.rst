Usage
=====

.. _installation:

Installation
------------

To use EwrTech, first install it using pip:

.. code-block:: console

   (.venv) $ pip install ewrtech

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``ewrtech.get_random_ingredients()`` function:

.. autofunction:: ewrtech.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`ewrtech.get_random_ingredients`
will raise an exception.

.. autoexception:: ewrtech.InvalidKindError

For example:

>>> import lumache
>>> ewrtech.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

