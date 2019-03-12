********************
Local Install of RTD
********************

As described
============
** insert macsetup.rst/RTD Locally


Other misc
==========
run redis server
.. code-block:: bash

    $ brew services start redis

install mactex
.. code-block:: bash

    $ brew cask install mactex

Running the server
==================

First time
----------

Every time
----------
enter the virtualenv (source venv/bin/activate)
Run server (python manage.py runserver ip.ip.ip.ip:8000)