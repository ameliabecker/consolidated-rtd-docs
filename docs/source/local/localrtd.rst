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




document changes
================

async
-----
celery/backends/redis.py and async.py
change async to asynchronous

projects_project__old
---------------------
while loading test data

from docker file:
create local_settings.py

.. code-block:: python

	# Setting Overrides
    # See readthedocs/settings/*.py for settings that need to be modified
    import os

    # Set this to the root domain where this RTD installation will be running
    PRODUCTION_DOMAIN = os.getenv('RTD_PRODUCTION_DOMAIN', 'localhost:8000')

    # Set the Slumber API host
    SLUMBER_API_HOST = os.getenv('RTD_SLUMBER_API_HOST', "http://" + PRODUCTION_DOMAIN)

    # Turn off email verification
    ACCOUNT_EMAIL_VERIFICATION = 'none'
    
    # Enable private Git doc repositories
    ALLOW_PRIVATE_REPOS = True



changing the "projects_project__old" issue
`stackoverflow link`_ 

.. _stackoverflow link: https://stackoverflow.com/questions/53637182/django-no-such-table-main-auth-user-old



Change "projects_project__old" issue

download sqlite3.22.0 version (install)
in /usr/local/opt/python/Frameworks/Python.framework/Versions/3.6/lib/python3.6/lib-dynload/_sqlite3.cpython-36m-darwin.so

replace with allen's file (see slack)

delete readthedocs.com/dev.db

migrate
etc...
load test_data


in venv/bin

.. code-block:: bash

    ln -s python3.6 python3.7



