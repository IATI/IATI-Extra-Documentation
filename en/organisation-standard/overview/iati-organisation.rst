IATI Organisation
=================

Definition
----------
Within the **IATI organisation standard**. the ``iati-organisation`` is the building block to describe organisations.

| An ``iati-organisation`` represents a distinct grouping of information that reports various facts about an organisation.

| A human-readable title and description for an ``iati-organisation`` can be provided using:

* ``name`` - a human-readable name of the organisation.


Considerations
--------------
When using the **IATI organisation standard** to declare an *iati-organisation*, the following should be considered:

* Every ``iati-organisation`` must use a globally unique ``iati-identifier``
* A publisher can set a default language and ``default-currency``, that is then used throughout the ``iati-activity``.  This can be overridden in subsequent elements however.
* The ``last-updated-datetime`` date must change whenever the value of any field within the associated ``iati-organisation`` are updated.
* The ``name`` can be repeated for different languages.  
* The free-text instance of ``name`` should avoid use of text in CAPITALS, where possible. 

