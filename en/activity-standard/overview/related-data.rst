Related Data
============

Definition
----------
Within the **IATI activity standard** it is possible to express relations between ``iati-activity`` records, across different publishers / ``reporting-org``.

| This can be described through two methods:

* ``related-activity`` - another ``iati-activity`` that has relationship to the one being described.
* ``transaction`` - ``provider-activity-id`` & ``receiver-activity-id`` - can be used to link funds from one ``iati-activity`` to another.


Considerations
--------------
When using the **IATI activity standard** to declare *traceability*, the following should be considered:

* A ``related-activity`` can be one published by any ``reporting-org`` - it does not have to be from the same publisher.

* When declaring a ``related-activity`` it is vital to include the reference to the unique ``iati-identifier``.  This enables structured links to be made.

* It is also recommended to include the type of relationship that is being expressed, through use of the ``RelatedActivityType`` code

* At the transaction level , it is recommended to connect ``iati-activity`` through use of the ``provider-activity-id`` & ``receiver-activity-id`` fields.  Specifically:

	* When an *Incoming Fund* is being described, use the ``provider-activity-id`` reference to declare the immediate source of the funds, using the relevant ``iati-identifier`` of the ``iati-activity``, if published by the ``provider-org``

	* When a *Disbursement* or *Commitment* is being described, use the ``receiver-activity-id`` reference to declare the immediate destination of the funds, using the relevant ``iati-identifier`` of the ``iati-activity``, if published by the ``receiver-org``

