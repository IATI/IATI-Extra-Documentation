IATI Organisation
=================

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI organisation standard**. the ``iati-organisation`` is the building block to describe organisations.

| An ``iati-organisation`` represents a distinct grouping of information that reports various facts about an organisation.

| For each ``iati-organisation`` described, the following are expected as a minium:

* ``iati-identifier`` is the unique reference for the organisation.
* ``name`` - a human-readable name of the organisation.


Considerations
--------------
When using the **IATI organisation standard** to declare an *iati-organisation*, the following should be considered:

* Every ``iati-organisation`` must use a globally unique ``iati-identifier``
* The ``iati-identifier`` should have no leading or trailing whitespace.
* It is recommended that no forward slashes (/) or spaces should be contained within the ``iati-identifier``.
* It is recommended to avoid spaces and non-ascii characters.  For example:
	* ``AA-AAA-123456789`` is preferable to ``AA-AAA 123456789``.
* A default language and ``default-currency`` can be set for any ``iati-organisation``.  This can be overridden in subsequent elements.
* The ``last-updated-datetime`` date must change whenever the value of any field within the associated ``iati-organisation`` are updated.
* The ``name`` can be repeated for different languages.  
* The free-text instance of ``name`` should avoid use of text in CAPITALS, where possible. 

Further Guidance 
----------------
Please also consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.
