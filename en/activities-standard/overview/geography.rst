Geography
=========

Definition
----------
Within the **IATI activity standard** there are three ways to describe the geographies of an ``iati-activity``:

* ``recipient-country`` - the country that will benefit from this activity.
* ``recipient-region`` - geopolitical region (above the country level) that will benefit from this activity.
* ``location`` - a geographical location.

In addition, the following can also be utilised:

* ``activity-scope`` - to classify the geographic coverage of the activity.

Considerations
--------------
When describing the ``recipient-country`` the relevant ``Country`` code must be used.

When describing the ``recipient-region`` the relevant ``Region`` code must be used.

It is possible to have multiple ``recipient-country`` in an ``iati-activity``

It is possible to have multiple ``recipient-region`` in an ``iati-activity``

When declaring multiple ``recipient-country`` or ``recipient-region`` then a ``pecentage`` must be declared.  These must sum to 100%.

If a ``recipient-country`` is known, then a ``recipient-region`` is not expected.

If a ``recipient-country`` is not known, then a ``recipient-region`` is expected.

The ``activity-scope`` element should only be used once.  It must use a relevant ``ActivityScope`` code.

Further guidance
----------------
