gears-handlebars
==================

Handlebars_ compiler for Gears_. This package already includes the Handlebars
source code for you, so you don't need to worry about installing it yourself.

Bundled Handlebars version: **1.0.7**

Installation
------------

Install ``gears-handlebars`` with pip::

    $ pip install gears-handlebars


Requirements
------------

``gears-handlebars`` requires node.js_ to be installed in your system.


Usage
-----

Add ``gears_handlebars.HandlebarsCompiler`` to ``environment``'s compilers
registry::

    from gears_handlebars import HandlebarsCompiler
    environment.compilers.register('.handlebars', HandlebarsCompiler.as_handler())

If you use Gears in your Django project, add this code to its settings::

    GEARS_COMPILERS = {
        '.handlebars': 'gears_handlebars.HandlebarsCompiler',
    }

.. _Handlebars: http://handlebarsjs.com/
.. _Gears: https://github.com/gears/gears
.. _node.js: http://nodejs.org/
