.. _usage_installation:

Grab Installaion
================


.. _installation_linux:

Installation on Linux
--------------------------

Run the command:

.. code:: shell

    pip install -U Grab



.. _installation_windows:

Installation on Windows
-----------------------

1) Install lxml. You can get lxml here: http://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml

2) Install pycurl. You can get pycurl here: http://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml

3) Install Grab

Download the Grab package from https://pypi.python.org/pypi/grab, unpack it and run::

    python setup.py install

If you use Python 2.x, then you might get an error while using `python setup.py install`. There is a bug in python 2.7.6. Delete it, download python 2.7.5 and try to install Grab again.

You can also install Grab via pip. If you don't have pip installed, install pip first. Download the file get-pip.py from https://bootstrap.pypa.io/get-pip.py and then run this command::

    python get-pip.py

Now you can install Grab via pip with this command::

    python -m pip install grab



.. _installation_freebsd:

Installation on FreeBSD
-----------------------

Run the command:

.. code:: shell

    pip install -U Grab

You can also install Grab from FreeBSD ports (thanks to Ruslan Makhmatkhanov):

* To install the port: cd /usr/ports/devel/py-grab/ && make install clean
* To add the package: pkg_add -r py27-grab



.. _installation_macos:

Installation on MacOS
---------------------

Run the command:

.. code:: shell

    pip install -U Grab



.. _installation_deps:

Dependencies
------------

All required dependencies should be installed automatically if you 
install Grab with pip. Here is actual list of Grab dependencies::

    lxml
    pycurl
    selection
    tools
    six


.. _installation_upgrade:

Upgrade Grab from 0.5.x version to 0.6.x
------------------------------------

In Grab 0.6.x some features were moved out into separate packages. If
you install/upgrade Grab with pip command all dependencies should
be installed automatically. Anyway, if you have some ImportError issues
then try to install dependencies manually with the command:

.. code:: shell

    pip istall -U lxml pycurl selection tools six