requests Magpie authentication library
======================================

Requests is an HTTP library, written in Python, for human beings. This library
adds optional Magpie authentication support. Basic GET usage:


.. code-block:: python

    import requests
    from requests_magpie import MagpieAuth

    auth = MagpieAuth("https://www.example.com/magpie", "username", "password")

    r = requests.get("https://www.example.com/protected", auth=auth)

The entire ``requests.api`` should be supported.

Logging
-------

This library makes extensive use of Python's logging facilities.

Log messages are logged to the ``requests_magpie`` named loggers.
