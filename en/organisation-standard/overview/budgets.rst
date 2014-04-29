Budgets
=======

Definition
----------
Within the **IATI organisation standard** three types of *budgets* can be declared.  

These all relate to the specific ``iati-organisation`` being described:

* ``total-budget`` - total annual planned budget of the ``iati-organisation``.
* ``recipient-org-budget`` - budget for disbursements to another organisation.
* ``recipient-country-budget`` -  budget for each country in which the ``iati-organisation`` operates.


Considerations
--------------
When declaring various *budgets* in the **IATI organisation standard** the following should be considered:

* It is recommended that budgets in the **IATI organisation standard** are forward-looking.

* It is recommended, where possible, that budgets are presented for the next three financial years.

* It is possible to report periods other than financial years, but this is not recommended.

* Financial years are presented using the ``period-start`` and ``period-end`` dates.

* It is expected that financial years appropriate to the relevant ``iati-organisation`` would be described.

* It is strongly recommended that the ``period-start`` and ``period-end`` of the financial years described for any ``recipient-country-budget`` match the budgetary/planning cycle of the ``recipient-country``.

* It is possible to report budget values in multiple ``currency``

* The ``default-currency`` can be set in the ``iati-organisaton`` element.  Should subsequent budgets be in the same ``currency`` then there is no need to restate.


Further guidance
----------------

* :doc:`total-budget </organisation-standard/iati-organisations/iati-organisation/total-budget/>`
* :doc:`recipient-org-budget </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/>`
* :doc:`recipient-country-budget </organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/>`
