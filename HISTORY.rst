Version history
===============

1.0.0
-----

* Make compatible with Python 2 and 3.

* Use portal_catalog.getAllBrains, if available.

* Use base_hasattr from CMFPlone instead of shasattr from Archetypes.

* Fixed argument parsing in Plone 4 or newer Zope2 instance recipes.

* No longer allow 0 as ``--keep-history`` value.  The original object
  is included in the count.  Strictly speaking 0 would ask to remove
  all versions plus the original objects.  This would actually fail.

* Catch and reraise KeyboardInterrupt, so you can interrupt the script.

* Added note to transaction commit.

* Added ``dry-run`` option.

* ``--keep-history`` defaults to blank, which uses the original value
  set in portal_purgehistory.  Now when the original value is -1
  (unlimited) you can set it to 0 with this option.  Previously this
  was ignored.

* Added ``--permanent`` option.

* Be more careful about keeping the history.

* Search without restrictions, like language.

* cleanup

0.2.1
-----

* delete the ``version_id`` only when don't want to keep history

0.2
---

* also delete ``version_id`` from the object
* check if object can be versioned before cleaning

0.1
---

* First version
