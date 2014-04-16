Organisations
=============

Definition
----------
Within the **IATI activity standard** organisations can be declared in three ways:

* ``reporting-org`` - the organisation publishing the activity file and associated data. 
* ``participating-org`` - the organisation that has a role within the activity (there can be various roles)
* ``provider-org`` / ``receiver-org`` - the organisation in providing or receiving a specific ``transaction``

Considerations
--------------
In many cases, an activity file will contain information from the perspective of a single organisation.  Most commonly, this will be the same as the ``reporting-org``

It is also expected that this organisation would be cited as a ``participating-org``, along with their associated role(s). 

It is possible for multiple ``participating-org`` to be reported within a single activity.  

Multiple ``participating-org`` with the same role, are also feasible.

In all cases, when describing an organisation, reference to their associated unique identifier should be included.

Should a ``provider-org`` or ``receiver-org`` within a ``transaction`` be the same as the ``reporting-org`` it is not expected that they are declared, but recommended.

Further guidance
----------------
