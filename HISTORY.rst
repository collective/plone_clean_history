Version history
===============

0.3
---

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
