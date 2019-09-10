Budgets
=======

The new budget guidance can be found here:

- `Budgets (Overview) <https://drive.google.com/open?id=1JhMfO-f3Mldrs15OMlHTAUF9KixTUq5G>`__: explains what budgets can be published in IATI.

- `Activity Budgets <https://drive.google.com/open?id=1vB3vk7gbnADwG1S8A1bRDd8mK-nOfwCh>`__: explains how to publish and use activity budget data.

These new pages were created in 2019 and will be transferred onto the new IATI Standard website in the near future.

Previous Budget Guidance:
~~~~~~~~~~~~~~~~~~~~~~~~

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

2.01 Considerations
-------------------
In version 2.01, the following must also be considered:

* The ``planned-disbursement`` element no longer has an ``@updated`` attribute.  This has been replaced by a ``@type`` attribute
