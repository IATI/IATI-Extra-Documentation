Budgets
=======

Definition
----------
The monetary *budgets* assigned to a specific ``iati-activity`` can be described in the **IATI activity standard** using the following:

* ``transaction-type`` type Commitment (code *2*) can be used to describe the total committed budget for the duration of the activity.
* ``budget`` - the value of the ``iati-activity`` ``budget`` for each financial year, as stated in the original project document.
* ``planned-disbursement`` - a scheduled payment, set up against the ``budget``
 
Additionally, there are two areas within the **IATI activity standard** that allow further clarification of budgets:

* ``country-budget-item`` - alignment of ``iati-activity`` with the functional and administrative classifications used in the ``recipient-country`` Chart of Accounts.
* ``capital-spend`` - the percentage of the total commitment that is for capital spending.

These all relate to the specific ``iati-activity`` being described.  


Considerations
--------------
When using the **IATI activity standard** to declare *budgets*, the following should be considered:

* It is recommended that budgets are presented in financial years.
* When presenting multiple budgets, then the ``budget`` element should be repeated accordingly.
* It is expected that the financial years for ``reporting-org`` are described.
* It is possible to report periods other than years, but this is not recommended.
* Financial periods can be presented using the ``period-start`` and ``period-end`` dates.
* For ``planned-dibursement`` it is valid to only report the ``period-start`` as a single date.
* It is possible to report budget values in multiple currencies, overriding the default currency set in ``iati-activity``
* It is expected that budgets would be described from the ``reporting-org`` perspective. 
* When declaring a ``value-date`` for any budget, this date must be in the past.

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* The ``planned-disbursement`` element no longer has an ``@updated`` attribute.  This has been replaced by a ``@type`` attribute
