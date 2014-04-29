IATI Identifier
===============

Definition
----------
Within the **IATI activity standard**, the ``iati-identifier`` is the unique reference for an an ``iati-activity``.

| The ``iati-identifier`` is a concatenation of the ``reporting-org`` reference and the reference allocated to ``iati-activity`` by the ``reporting-org``.  Together, these make the ``iati-identifier``

| The ``iati-identifier`` in the **IATI activity standard** is not the same as the ``iati-identifier`` in the **IATI organisation standard**


Considerations
--------------
When declaring an *iati-identifier* in the **IATI activity standard** the following should be considered:

* The ``iati-identifier`` must be unique for every ``iati-activity`` within the complete dataset published. 

* The ``iati-identifier`` should have no leading or trailing whitespace.

* It is recommended that no forward slashes (/) or spaces should be contained within the ``iati-identifier``

* It is recommended to avoid spaces and non-ascii characters.  

* For example:

** ``AA-AAA-123456789-ABC123`` is preferable to ``AA-AAA-123456789-ABC 123``.


Further guidance
----------------

Reference pages:

* Organisation Identifiers
* :doc:`iati-identifier </activities-standard/iati-activities/iati-activity/iati-identifier/>`
* :doc:`iati-activity </activities-standard/iati-activities/iati-activity/>`
* :doc:`reporting-org </activities-standard/iati-activities/iati-activity/reporting-org/>`
