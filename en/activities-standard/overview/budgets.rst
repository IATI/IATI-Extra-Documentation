Budgets
=======

Definition
----------
The monetary budget assigned to a specific ``iati-activity`` can be described in the **IATI activity standard** using the following:

* ``transaction`` type commitment - this can be used to describe the total committed budget for the duration of the activity.
* ``budget`` - the value of the ``iati-activity``'s budget for each financial year, as stated in the original project document.
* ``planned-disbursement`` - a scheduled payment, set up against the ``budget``

 'definition' of planned disbursement is "The recommendation is that, where and when possible, the amounts it is planned to disburse and spend on the activity in each of the next three financial years are reported."
 
Additionally, there are two areas within the **IATI activity standard** that allow further clarification around budgets:

* ``country-budget-item`` - alignment of ``iati-activity`` with the functional and administrative classifications used in the ``recipient-country``'s Chart of Accounts.
* ``capital-spend`` - the percentage of the total commitment that is for capital spending.

These all relate to the specific ``iati-activity`` being described.  

Considerations
--------------
IATI expects that budgets in the activity standard are forward-looking. - THIS IS NOT TRUE IN ACTIVITY STANDARD?

It is recommended, where possible, that budgets are presented for the next three financial years. THIS IS NOT TRUE IN ACTIVTY STANDARD?

It is recommended, where possible, that budgets are presented in financial years.

It is possible to report periods other than years, but this is not recommended.

Financial years can be presented using the ``period-start`` and ``period-end`` dates.

It is expected that the financial years for ``reporting-org`` would be described.

It is possible to report budget values in multiple currencies, overriding the default currency set in ``iati-activity``

It is expected that budgets would be described from the ``reporting-org`` perspective.  UNLESS A SECONDARY PUBLISHER

NOTHING HERE YET FOR BUDGETITEM OR CAPITALSPEND

Further guidance
----------------

TO BE UPDATED

* :doc:`total-budget </organisation-standard/iati-organisations/iati-organisation/total-budget/>`
* :doc:`recipient-org-budget </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/>`
* :doc:`recipient-country-budget </organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/>`

activities-standard/country-budget-items/
