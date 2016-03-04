Type of Organisations
=====================

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

2.01 Considerations
-------------------
In version 2.01, the following must also be considered:

* A ``reporting-org`` is a mandatory element
* A ``reporting-org`` identifier must start with a value published on the *OrganisationRegistrationAgency* codelist.
* Any freetext ``name`` for an organisation, must be included in the child ``narrative`` element, which can be repeated for different languages. 


Further Guidance 
----------------
Please also consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.   


