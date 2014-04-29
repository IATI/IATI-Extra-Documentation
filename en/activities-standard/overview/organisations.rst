Organisations
=============

Definition
----------
Within the **IATI activity standard** *organisations* can be declared in three ways:

* ``reporting-org`` - the organisation publishing the activity file and associated data. 
* ``participating-org`` - the organisation that has a role within the activity (there can be various roles)
* ``provider-org`` / ``receiver-org`` - the organisation in providing or receiving a specific ``transaction``


Considerations
--------------
When using the **IATI activity standard** to declare *organisations*, the following should be considered:

* In many cases, an activity file will contain information from the perspective of a single organisation.  Most commonly, this will be the same as the ``reporting-org``

* It is also expected that this organisation would be cited as a ``participating-org``, along with their associated role(s). 

* It is possible for multiple ``participating-org`` to be reported within a single activity.  

* Multiple ``participating-org`` with the same ``OrganisationRole`` code are also feasible.

* For ``reporting-org`` and ``participating-org`` inclusion of the ``OrganisationType`` code is recommended.
 
* In all cases, when describing an organisation, reference to their associated unique identifier should be included.

* Should a ``provider-org`` or ``receiver-org`` within a ``transaction`` be the same as the ``reporting-org`` it is not expected that they are declared, but recommended.


Further guidance
----------------

Reference pages:

* :doc:`reporting-org </activities-standard/iati-activities/iati-activity/reporting-org/>`
* :doc:`participating-org </activities-standard/iati-activities/iati-activity/participating-org/>`

* :doc:`transaction/provider-org </activities-standard/iati-activities/iati-activity/transaction/provider-org/>`
* :doc:`transaction/receiver-org </activities-standard/iati-activities/iati-activity/transaction/receiver-org/>`
