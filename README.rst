Generic Example Buildout with RelStorage
========================================

Flavors and features:

- with RelStorage on PostgreSQL
    - for dev
    - on production

- a ZEO server for local dev
- filestorage on local dev
- RelStorage import/export/pack configurations generated through templates


Usage
-----

1. clone the buildout
2. cd into the directory
3. create symlink to desired flavor, e.g.: ``ln -s de-with-relstorage buildout.cfg``
4. run ``./bootstrap.sh``.
5. enjoy

When using RelStorage:

In ``./bin/`` there are now two scripts:

- ``zodbconvert`` can be used to convert from filestorage to RelStorage and back.
  The configurations for both are prepared in ``relstorage-import.cfg`` and ``relstorage-export.cfg``.
- ``zodbpack`` with ``relstorage-pack.cfg`` can be used two pack history-aware RelStorages and to garbage collect history-free RelStorages.


Contribute
----------

- Source Code: https://github.com/jensens/example-relstorage-buildout
- Issue Tracker: https://github.com/jensens/example-relstorage-buildout/issues


Support
-------

If you are having issues please create an issue (see above) or just let me know:
`jens@bluedynamics.com <mailto:jens@bluedynamics.com>`_


License
-------

The project is licensed under the GPLv2.
