IATI Activity
=============

Definition
----------
Within the **IATI activity standard**. the ``iati-activity`` is the building block to describe aid.

An ``iati-activity`` represents a distinct grouping of information that reports various facts of an aid activity.

A human-readable title and description for an ``iati-activity`` can be provided using:

* ``title`` - a short, human-readable title.
* ``description`` - a  longer, human-readable description.


Considerations
--------------
When using the **IATI activity standard** to declare an *iati-identifier*, the following should be considered:

* Every ``iati-activity`` must have a globally unique ``iati-identifier``
* Publishers can decide on how best to structure and segment their organisation data around ``iati-activity``
* A publisher can set a default language and ``default-currency``, that is then used throughout the ``iati-activity``.  This can be overridden in subsequent elements however.
* The ``last-updated-datetime`` date must change whenever the value of any field within the associated ``iati-activity`` is updated.
* It is recommended that the ``title`` should be concise and jargon-free
* A ``description`` can have different focal points, by using the appropriate ``DescriptionType`` codelist
* The free-text instances of ``title`` and ``description`` should avoid use of text in CAPITALS, where possible. 
* Both the ``title`` and ``descriptions`` can be repeated for different languages.  
* When an ``iati-activity`` is being implemented in a ``recipient-country`` where the official language is different to that of the ``reporting-org`` it is recommended that activity ``title`` and ``description`` are provided in all official ``reporting-org`` and ``recipient-country`` languages

