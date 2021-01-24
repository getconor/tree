##################
Tree Documentation
##################

.. toctree::
   :maxdepth: 2
   :hidden:

   api
   changes

``tree`` is a library for working with nested data structures. In a way,
``tree`` generalizes the builtin :func:`map` function which only supports 
flat sequences, and allows to apply a function to each "leaf" preserving 
the overall structure.

Here's a quick example::

  >>> tree.map_structure(lambda v: v**2, [[1], [[[2, 3]]], [4]])
  [[1], [[[4, 9]]], [16]]

.. note::

    Most functions of the ``tree`` library were originally a part of TensorFlow 1 as 
    ``tf.contrib.framework.nest``. When ``contrib`` was deprecated in TensorFlow 2.0, 
    a few of the original functions were retained and still reside in TensorFlow 2's 
    ``tf.nest`` library, while most functions were exported to ``tree``, which was 
    then released separately. 

Installation
============

Install ``tree`` by running::

  $ pip install dm-tree

Support
=======

If you are having issues, please let us know by filing an issue on our
`issue tracker <https://github.com/deepmind/tree/issues>`_.

License
=======

Tree is licensed under the Apache 2.0 License.
