we-get: command-line tool for searching torrents.
#################################################

.. image:: https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square   :target:

.. class:: head

    .. image:: https://raw.githubusercontent.com/wiki/0xl3vi/we-get/screenshots/1.png
        :alt: Main screenshot.
        :width: 100%
        :align: center



.. contents::
.. section-numbering::

Installation
============

.. code-block:: bash

    $ sudo python setup.py install

``pip`` installation will be available in the future.


Dependencies
============

* `prompt_toolkit <https://github.com/jonathanslenders/python-prompt-toolkit>`_
* `docopt <https://github.com/docopt/docopt>`_
* `colorama <https://github.com/tartley/colorama>`_

and `Python <https://www.python.org/>`_ 3.5 or above

Basic Usage
===========

.. code-block:: bash

    $ we-get --search "royal pains" --target  the_pirate_bay,1337x --filter "S01"

================    =======================================
``--search``        search term.
``--target``        specify module[s] to use, you can use multiple modules separated by comma. 
``--filter``        can be regular expression or text to match in the torrent name.
================    =======================================

Options
--------

==================    =========================================
 -s --search <term>    search query
 -l --list             list top torrents (can't be with --search)
 -t --target           target module (see -G)
 -L --links            show download links for the torrents
 -J --json             output in json format
 -G --get-list         list available modules
 -f --filter           can be regular expression or text to match in the torrent name
 -n --results          number of results to retrieve
==================    =========================================

Video options
--------------

==============   =======================
 -q --quality      try to match video quality to the torrent (720p, 1080p ...)
 -g --genre        try to find genre for the torrent video.
==============   =======================


See also ``we-get --help``.

Supported websites
------------------

* 1337x
* thepiratebay
* eztv
* yts

and the list will grow.

Contributing
------------

Any collaboration is welcome!

If you want to write a module please see ``we_get/modules/``


Licence
-------

MIT: `LICENSE <https://github.com/0xl3vi/we-get/blob/master/LICENSE>`_.
