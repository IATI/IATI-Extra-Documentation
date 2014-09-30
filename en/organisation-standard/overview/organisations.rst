Type of Organisations
=====================

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI organisation standard** three types of *organisations* can be declared:

* ``reporting-org`` - the organisation publishing the data within the *organisation file*. 
* ``iati-organisation`` - the organisation that the data is about
* ``recipient-org`` - the organisation in receipt of budgets specified in ``recipient-org-budget``


Considerations
--------------
When using the **IATI organisation standard** to declare *organisations*, the following should be considered:

* In many cases, an *organisation file* will contain information from the perspective of a single ``iati-organisation``.  Most commonly, this will be the same as the ``reporting-org``
* Multiple ``iati-organisation`` can be described in a single *organisation file*.
* ``reporting-org`` and ``iati-organisation`` should include reference to their associated unique ``iati-identifier``
* For ``reporting-org``, inclusion of the ``OrganisationType`` code is recommended.
* An ``iati-organisation`` should include a ``name`` element - free text title of the organisation
* Single or multiple ``recipient-org`` entries can be recorded.
* For each ``recipient-org`` multiple forward looking ``recipient-org-budget`` can be recorded.


Further Guidance 
----------------
Please also consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.   


