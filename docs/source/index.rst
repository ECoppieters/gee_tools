.. geetools documentation master file, created by
   sphinx-quickstart on Wed Nov 15 08:48:59 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to GEE tools's documentation
====================================

A set of useful tools to use in Google Earth Engine Python API

.. toctree::
    :maxdepth: 2
    :caption: Contents:

    Documentation

Installation
------------

You can install it like any other python package

.. code:: bash

    pip install geetools

Basic Usage
-----------

.. code:: python

    from geetools import tools

    image = ee.Image([1,3,5,7]).rename(['b1', 'b2', 'b3', 'b4'])
    point = ee.Geometry.Point([0, 0])
    values = tools.image.getValue(image, point, scale=30, side='client')
    print(values)

More in the :doc:`Documentation`

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
