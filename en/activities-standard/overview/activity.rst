IATI Activity
=============

Definition
----------
An ``iati-activity`` a distinct grouping of data that collects and describes various facts of an *activity*.

A human-readable title and description for an ``iati-activity`` can be provided using

* ``title``
* ``description``

Considerations
--------------
Every ``iati-activity`` must have a globally unique ``iati-identifier``

Publishers can decide on how best to structure and segment their organisation data around ``iati-activity``

A publisher can set a default language and currency, that is then used throughout the ``iati-activity``.  This can be overridden in at any point however.

It is recommended that the ``title`` should be concise and jargon-free

A ``description`` can have different focal points, by using the appropriate ``DescriptionType`` codelist

Both the ``title`` and ``descriptions`` can be repeated for different languages.  

When an ``iati-activity`` is being implemented in a ``recipient-country`` where the official language is different to that of the ``reporting-org`` it is recommended that activity ``title`` and ``description`` are provided in all official ``reporting-org`` and ``recipient-country`` languages

Further guidance
----------------

Reference pages:

* :doc:`iati-identifier </activities-standard/iati-activities/iati-activity/iati-identifier/>`
* :doc:`iati-activity </activities-standard/iati-activities/iati-activity/>`
* :doc:`title </activities-standard/iati-activities/iati-activity/title/>`
* :doc:`description </activities-standard/iati-activities/iati-activity/description/>`
