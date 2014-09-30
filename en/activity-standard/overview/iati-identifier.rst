IATI Identifier
===============

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI activity standard**, the ``iati-identifier`` is the unique reference for an an ``iati-activity``.

The ``iati-identifier`` is a concatenation of the ``reporting-org`` reference and the reference allocated to ``iati-activity`` by the ``reporting-org``.  Together, these make the ``iati-identifier``

The ``iati-identifier`` in the **IATI activity standard** is not the same as the ``iati-identifier`` in the **IATI organisation standard**


Considerations
--------------
When using the **IATI activity standard** to declare an *iati-identifier* the following should be considered:

* The ``iati-identifier`` must be unique for every ``iati-activity`` within the complete dataset published. 
* The ``iati-identifier`` should have no leading or trailing whitespace.
* It is recommended that no forward slashes (/) or spaces should be contained within the ``iati-identifier``
* It is recommended to avoid spaces and non-ascii characters.  
* For example:
	* ``AA-AAA-123456789-ABC123`` is preferable to ``AA-AAA-123456789-ABC 123``.


Further Guidance 
----------------
Please also consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.
