Transaction
===========

Definition
----------
The **IATI activity standard** enables ``transaction`` information to be published.

| The ``transaction`` data is a core component to IATI, detailing the flow of monies between organisations.

Considerations
--------------
When using the **IATI activity standard** to declare *transaction*, the following should be considered:

* It is expected that every ``iati-activity`` should contain at least one ``transaction``.  However, this may not always be possible for early-stage activities, for example.

* Every ``transaction`` must contain a ``transaction-date`` , ``value``,  ``value-date`` and ``transaction-type``.

* For every ``transaction`` a type contained on the ``TransactionType`` codelist is expected, 

* There are several possible types of transactions, with the most common being:

	* Commitment - the total agreed budget for the activity.
	* Disbursement - the amount transferred to another organisation in the aid delivery chain (e.g. a partner organisation being funded).
	* Expenditure - the outlay on goods and services.
	* Incoming funds - the funds received from an external funding source (e.g. a donor).

* The ``value`` of a transaction can be positive or negative, and contain decimals.  It should not contain comma seperators (eg: 3,000)

	* example: ``3000`` or ``3000.00`` is acceptable.  ``3,000`` is not
	
* Both the ``transaction-date`` and ``value-date`` must be in ISO 8601 format (YYYY-MM-DD), eg: 2014-03-21.

* Neither of ``transaction-date`` and ``value-date`` can be in the "future".  A ``transaction`` always describes something that has taken place.

* A ``transaction`` can be declared in any currency on the ``Currency`` codelist.

* A ``transaction`` can also include ``finance-type`` , ``flow-type`` , ``aid-type`` and/or ``tied-status`` information.  

* Both ``currency`` and ``finance-type`` , ``flow-type`` , ``aid-type``, ``tied-status`` can be set as defaults in the ``iati-activity`` element.  There is no requirement to restate these within a ``transaction`` if they are the same.

* A ``transaction`` can also contain information on the source and destination organisation.  When describing these the ``provider-org`` and ``receiver-org`` should be used.  Ideally, the unique organisation identifier would be included.

* Where possible, it is recommended that a ``transaction`` includes the ``provider-activity-id`` and/or ``receiver-activity-id`` to refernce the ``iati-activity`` from which funds flow from/to.


Further guidance
----------------

Reference pages:

* :doc:`transaction </activities-standard/iati-activities/iati-activity/transaction/>`
* :doc:`transaction-type </activities-standard/iati-activities/iati-activity/transaction/transaction-type/>`

* :doc:`value </activities-standard/iati-activities/iati-activity/transaction/value/>`
* :doc:`transaction-date </activities-standard/iati-activities/iati-activity/transaction/transaction-date/>`
* :doc:`provider-org </activities-standard/iati-activities/iati-activity/transaction/provider-org/>`
* :doc:`receiver-org </activities-standard/iati-activities/iati-activity/transaction/receiver-org/>`
* :doc:`description </activities-standard/iati-activities/iati-activity/transaction/description/>`

* :doc:`finance-type </activities-standard/iati-activities/iati-activity/transaction/finance-type/>`
* :doc:`disbursement-channel </activities-standard/iati-activities/iati-activity/transaction/disbursement-channel/>`
* :doc:`flow-type </activities-standard/iati-activities/iati-activity/transaction/flow-type/>`
* :doc:`aid-type </activities-standard/iati-activities/iati-activity/transaction/aid-type/>`
* :doc:`tied-status </activities-standard/iati-activities/iati-activity/transaction/tied-status/>`
