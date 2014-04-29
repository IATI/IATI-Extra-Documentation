Geography
=========

Definition
----------
Within the **IATI activity standard** there are three ways to describe the *geography* of an ``iati-activity``:

* ``recipient-country`` - the country that will benefit from the ``iati-activity``.
* ``recipient-region`` - geopolitical region (above the country level) that will benefit from the ``iati-activity``.
* ``location`` - a geographical location of the ``iati-activity``.

In addition, the following can also be utilised:

* ``activity-scope`` - to classify the geographic coverage of the the ``iati-activity``.

Considerations
--------------
When using the **IATI activity standard** to describe *geography*, the following should be considered:

* When describing the ``recipient-country`` the relevant ``Country`` code must be used.

* When describing the ``recipient-region`` the relevant ``Region`` code must be used.

* It is possible to have multiple ``recipient-country`` in an ``iati-activity``

* It is possible to have multiple ``recipient-region`` in an ``iati-activity``

* When declaring multiple ``recipient-country`` or ``recipient-region`` then a ``pecentage`` must be declared.  These must sum to 100%.

* If a ``recipient-country`` is known, then a ``recipient-region`` is not expected.

* If a ``recipient-country`` is not known, then a ``recipient-region`` is expected.

* The free-text instances of ``name`` and ``description`` in ``location`` should avoid use of text in CAPITALS, where possible. 

* The ``activity-scope`` element should only be used once.  It must use a relevant ``ActivityScope`` code.

Further guidance
----------------

Reference pages:

* :doc:`recipient-country </activities-standard/iati-activities/iati-activity/recipient-country/>`
* :doc:`recipient-region </activities-standard/iati-activities/iati-activity/recipient-region/>`
* :doc:`activity-scope </activities-standard/iati-activities/iati-activity/activity-scope/>`
* :doc:`location </activities-standard/iati-activities/iati-activity/location/>`
