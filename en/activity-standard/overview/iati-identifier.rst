IATI Identifier
===============

Definition
----------
Within the **IATI activity standard**, the ``iati-identifier`` is the unique reference for an an ``iati-activity``.

The ``iati-identifier`` is a concatenation of the ``reporting-org`` reference and the reference allocated to ``iati-activity`` by the ``reporting-org``.  Together, these make the ``iati-identifier``.


Considerations
--------------
When using the **IATI activity standard** to declare an *iati-identifier* the following should be considered:

* The ``iati-identifier`` must be unique for every ``iati-activity`` within the complete dataset published.
* The ``iati-identifier`` should have no leading or trailing whitespace.
* It is recommended that no forward slashes (/) or spaces should be contained within the ``iati-identifier``.
* It is recommended to avoid spaces and non-ascii characters.
* For example:
	* *AA-AAA-123456789-ABC123* is preferable to *AA-AAA-123456789-ABC 123*.

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* The ``iati-identifier`` must begin with either the current IATI organisation identifier for the reporting organisation or a previous identifier reported in the element ``other-identifier``.

Further Guidance 
----------------
Please also consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.
