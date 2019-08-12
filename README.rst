requests Magpie authentication library
======================================

.. image:: https://travis-ci.org/requests/requests-magpie.svg?branch=master
    :target: https://travis-ci.org/requests/requests-magpie

Requests is an HTTP library, written in Python, for human beings. This library
adds optional Magpie authentication support. Basic GET usage:


.. code-block:: python

    >>> import requests
    >>> from requests_magpie import MagpieAuth
    >>> magpie_url = "https://www.example.com/magpie"
    >>> r = requests.get("http://example.org", auth=MagpieAuth(magpie_url, "username", "password"))
    ...

The entire ``requests.api`` should be supported.

Logging
-------

This library makes extensive use of Python's logging facilities.

Log messages are logged to the ``requests_magpie`` named loggers.

Thanks
------

Thanks to the `requests-kerberos <https://github.com/requests/requests-kerberos>`_
library, from which the packaging template was inspired by.
