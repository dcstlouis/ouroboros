Contributing to Ouroboros
=========================


If you experience problems with Ouroboros, `log them on GitHub`_. If you want to contribute code, please `fork the code`_ and `submit a pull request`_.

.. _log them on Github: https://github.com/pybee/ouroboros/issues
.. _fork the code: https://github.com/pybee/ouroboros
.. _submit a pull request: https://github.com/pybee/ouroboros/pulls


Setting up your development environment
---------------------------------------

The recommended way of setting up your development environment for Ouroboros
is to install a virtual environment, install the required dependencies and
start coding. Assuming that you are using ```virtualenvwrapper```_, you only have to run:

    $ git clone git@github.com:pybee/ouroboros.git
    $ cd ouroboros
    $ mkvirtualenv -p `which python3` ouroboros

If you've never used a virtual environment before and are not sure where to start,
check out `this primer`_ on virtual environments in Python.

Ouroboros uses ``unittest`` for its own test suite as well as additional helper
modules for testing. To install all the requirements for Ouroboros, you have to
run the following commands within your virtual environment:

    $ pip install -e .
    $ pip install -r requirements_dev.txt

A brief reminder that Ouroboros is intended to work only on python versions 3.3
and above.

Now you are ready to start hacking! Have fun!

.. _``virtualenvwrapper``: https://virtualenvwrapper.readthedocs.io/en/latest/
.. _this primer: https://realpython.com/python-virtual-environments-a-primer/


Running tests
-------------

Tests can be run using the following command from the project root::

    $ python setup.py test
