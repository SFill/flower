Installation
============

Installing `flower` with `pip <http://www.pip-installer.org/>`_ is simple ::

    $ pip install flower

Development version can be installed with ::

    $ pip install https://github.com/mher/flower/zipball/master#egg=flower

Usage
-----

Launch the server and open http://localhost:5555 ::

    $ flower -A proj --port=5555

Or, launch from Celery ::

    $ celery -A proj flower --address=127.0.0.1 --port=5555

Broker URL and other configuration options can be passed through the standard Celery options ::

    $ celery -A proj flower --broker=amqp://guest:guest@localhost:5672// --broker_api=http://guest:guest@localhost:15672/api/

