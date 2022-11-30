Installation
============

You can install relenv like any other python package using pip.  Using a virtual environment is recommended.

.. code-block:: bash

   pip install relenv

Usage Overview
==============

After installing relenv, you will have access to its CLI.  You can see all supported commands by running the following...

.. code-block:: bash

   relenv --help

The most common sub command of Relenv is the :ref:`create` command.  Create is used
to create new relenv environments.  When using relenv for the first time you
will need to :ref:`build` or :ref:`fetch` pre-built Python build.


.. _fetch:

Fetch
-----

The fetch command can be used to download a pre-built Relenv Python.

.. code-block:: bash

   relenv fetch

Now that you have a base Relenv Python build, you can use the :ref:`create` command to make new Relenv environments. See the full :doc:`cli/fetch` documentation for more details.

.. _build:


Build
-----

The build command is what relenv uses to build a Relenv Python environment.

.. code-block:: bash

   relenv build

See the full :doc:`cli/build` documentation for more details.



.. _create:

Create
------

Use create to make a new relenv environment.

.. code-block:: bash

   relenv create myenv

The new 'myenv' environment is fully self contained. You can pip install
any python packages you would like into the new 'myenv' environment. Everything
will be installed into myenv's site-packages directory. Any scripts created by
pip will use myenv's Python interpreter. See the full :doc:`cli/create` documentation for more details.

.. code-block:: bash

   myenv/bin/pip3 install mycoolpackage


