Transaction
===========

Definition
----------
The **IATI activity standard** enables ``transaction`` information to be published.

The ``transaction`` data is a core component to IATI, detailing the flow of monies between organisations.


Considerations
--------------
When using the **IATI activity standard** to declare *transaction*, the following should be considered:

* Every ``iati-activity`` should contain at least one ``transaction``.  However, this may not always be possible for early-stage activities, for example.
* Every ``transaction`` must contain a ``transaction-date`` , ``value``,  ``value-date`` and ``transaction-type``.
* For every ``transaction`` a type contained on the *TransactionType* codelist is required, 
* There are several types of transactions. The most common are:
	* Incoming funds (code*1*) - the funds received from a funding source (e.g. a donor).
	* Outgoing Commitment (code*2*) - the total agreed committed budget for the activity (this may or may not match the value of the activity's budget)
	* Disbursement (code*3*) - the amount transferred to another organisation in the aid delivery chain (e.g. a partner organisation being funded).
	* Expenditure (code*4*) - the outlay on goods and services and project overheads.
* The ``value`` of a transaction can be positive or negative, and contain decimals.  It should not contain comma separators (eg: 3,000)
	* example: ``3000`` or ``3000.00`` or ``-3000`` is acceptable.  ``3,000`` is not
* Both the ``transaction-date`` and ``value-date`` must be in ISO 8601 format (YYYY-MM-DD), eg: 2014-03-21.
* Neither of ``transaction-date`` and ``value-date`` can be in the "future".  A ``transaction`` always describes something that has taken place.
* A ``transaction`` can be declared in any currency on the *Currency* codelist.
* A ``transaction`` can also include ``finance-type`` , ``flow-type`` , ``aid-type`` and/or ``tied-status`` information.  
* Both ``currency`` and ``finance-type`` , ``flow-type`` , ``aid-type``, ``tied-status`` can be set as defaults in the ``iati-activity`` element.  There is no requirement to restate these within a ``transaction`` if they are the same.
* A ``transaction`` can also contain information on the source and destination organisation.  When describing these the ``provider-org`` and ``receiver-org`` should be used.  Ideally, the unique organisation identifier would be included.
* Where possible, it is recommended that a ``transaction`` includes the ``provider-activity-id`` and/or ``receiver-activity-id`` to reference the ``iati-activity`` from which funds flow from/to.

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* Dates should be a valid *xsd:date*, and a datetimes should be a valid *xsd:dateTime*.
* A ``recipient-country``, `recipient-region`` and ``sector`` can also be published as child elements of a ``transaction``.  When this is done, it is expected that **all** ``transaction`` include such data, whilst the relevant element is subsequently **not** included at the ``iati-activity`` level. Also none of these elements when published as child elements of a ``transaction`` need or use a percentage attribute as they do at the ``iati-activity`` level.   

