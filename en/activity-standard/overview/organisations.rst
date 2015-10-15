Organisations
=============

Definition
----------
Within the **IATI activity standard** *organisations* can be declared in three ways:

* ``reporting-org`` - the organisation publishing the activity file and associated data. 
* ``participating-org`` - the organisation that has a role within the activity (there can be various roles)
* ``provider-org`` / ``receiver-org`` - the organisation providing or receiving a specific ``transaction``


Considerations
--------------
When using the **IATI activity standard** to declare *organisations*, the following should be considered:

* In many cases, an activity file will contain information from the perspective of a single organisation.  Most commonly, this will be the same as the ``reporting-org``
* It is also expected that this organisation would be cited as a ``participating-org``, along with their associated role(s). 
* It is possible for multiple ``participating-org`` to be reported within a single activity.  
* Multiple ``participating-org`` with the same *OrganisationRole* code are also feasible.
* For ``reporting-org`` and ``participating-org`` inclusion of the *OrganisationType* code is recommended.
* In all cases, when describing an organisation, reference to their associated unique identifier should be included.
* Should a ``provider-org`` or ``receiver-org`` within a ``transaction`` be the same as the ``reporting-org`` it is not expected that they are declared, but recommended.

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* A ``reporting-org`` is a mandatory element
* A ``participating-org`` with *OrganisationRole* of funding (code *1*) and/or implementing (code *4*) is mandatory.
* A ``reporting-org`` identifier must start with a value published on the *OrganisationRegistrationAgency* codelist.
* Any freetext name for an organisation, must be included in the child ``narrative`` element, which can be repeated for different languages. 

Further Guidance 
----------------
Please consider and refer to the :doc:`Organisation Identifiers guidance <../../organisation-identifiers>` when constructing an appropriate identifier.
