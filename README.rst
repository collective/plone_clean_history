usage: /your/instance run clean_history.py [options] [sites]

Cleanup CMFEdition history in Plone sites. Default is: all sites in the
database.

options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -p PORTAL_TYPE, --portal-type=PORTAL_TYPE
                        select to cleanup only histories for a kind of
                        portal_type. Default is "all types". Can be called
                        multiple times.
  -k HISTORY_SIZE, --keep-history=HISTORY_SIZE
                        Before purging, temporary set the value of "maximum
                        number of versions to keep in the storage" to this
                        value in the portal_purgehistory. Default is: do not
                        change the value. In any case, the original value will
                        be restored.
  -v, --verbose         Show verbose output, for every cleaned content's
                        history.

