******************
Local Docker Setup
******************

download docker

.. code-block:: bash

    docker run -d -it -p 8000:8000 -e "RTD_PRODUCTION_DOMAIN=0.0.0.0:8000" --name readthedocs vassilvk/readthedocs

automatically runs

.. note:: Old RTD doesn't have webhook or gitlab capabilities

