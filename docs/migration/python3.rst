======================
 Migration to python3
======================

.. code-block:: sh

    # urlparse
    find . -type f -name '*.py' | xargs sed -i 's/import urlparse/import urllib.parse as urlparse/g'
    find . -type f -name '*.py' | xargs sed -i 's/from urlparse/from urllib.parse/g'
    
    # base64
    # TODO
    # SOMETHING.encode('base64') -> base64.b64encode(SOMETHING)
    # SOMETHING.decode('base64') -> base64.b64decode(SOMETHING)


