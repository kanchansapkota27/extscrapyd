======
extscrapyd
======

Added new endpoints only all the other documentation is same as of scrapyd

New endpoints
--------------

listoverview.json
-----------------

Complete overview of scrapy deployed projects.

* Supported Request Methods: ``GET``

Example request::

    curl http://localhost:6800/listoverview.json

If basic authentication is enabled::

    curl -u yourusername:yourpassword http://localhost:6800/listoverview.json

Example response::

    {"node_name": "Demo Node", "status": "ok", "pending": 0, "running": 0, "finished": 0, "total_unique_spiders": 1, "projects": {"newsfeed": [{"versions_count": 2, "versions": ["0_1_0", "0_1_1"], "unq_spiders_count": 1, "unq_spiders": ["defensefeed"]}], "default": [{"versions_count": 0, "versions": [], "unq_spiders_count": 0, "unq_spiders": []}]}}


listall.json
-----------------

Complete details of scrapy deployed projects.

* Supported Request Methods: ``GET``

Example request::

    curl http://localhost:6800/listall.json

If basic authentication is enabled::

    curl -u yourusername:yourpassword http://localhost:6800/listall.json

Example response::

    {"node_name": "Demo Node", "status": "ok", "pending": 0, "running": 0, "finished": 0, "projects": {"newsfeed": [{"id": "0_1_0", "spiders": ["defensefeed"]}, {"id": "0_1_1", "spiders": ["defensefeed"]}], "default": []}}


* Note: No tests has been included in the change.


=======
Scrapyd
=======


The documentation (including installation and usage) can be found at:
http://scrapyd.readthedocs.org/

