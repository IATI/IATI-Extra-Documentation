Budgets
=======

The new budget guidance can be found here:

- `Budgets (Overview) <https://drive.google.com/open?id=1JhMfO-f3Mldrs15OMlHTAUF9KixTUq5G>`__: explains what budgets can be published in IATI.

- `Organisation Budgets & Spend <https://drive.google.com/open?id=1mv2Q666tKBOAoiy5JayslmZNetxDM1uu>`__: explains how to publish and use organisation budget and spend data.

These new pages were created in 2019 and will be transferred onto the new IATI Standard website in the near future.

Previous Budget Guidance:
~~~~~~~~~~~~~~~~~~~~~~~~

Definition
----------
Within the **IATI organisation standard** three types of *budgets* can be declared.  

These all relate to the specific ``iati-organisation`` being described:

* ``total-budget`` - total annual planned budget of the ``iati-organisation``.
* ``recipient-org-budget`` - budget for disbursements to another organisation.
* ``recipient-country-budget`` -  budget for each country in which the ``iati-organisation`` operates.


Considerations
--------------
When using the **IATI organisation standard** to declare *budgets*, the following should be considered:

* It is recommended that budgets in the **IATI organisation standard** are forward-looking.
* It is recommended, where possible, that budgets are presented for the next three financial years.
* When presenting multiple budgets, then the relevant ``budget`` element should be repeated accordingly.
* It is possible to report periods other than financial years, but this is not recommended.
* Financial periods are presented using the ``period-start`` and ``period-end`` dates.
* It is expected that financial years appropriate to the relevant ``iati-organisation`` would be described.
* It is strongly recommended that the ``period-start`` and ``period-end`` of the financial years described for any ``recipient-country-budget`` match the budgetary/planning cycle of the ``recipient-country``.
* It is possible to report budget values in multiple ``@currency``.
* The ``@default-currency`` can be set in the ``iati-organisation`` element.  Should subsequent budgets be in the same ``@currency`` then there is no need to restate.
* When declaring a ``value-date`` for any budget, this date must be in the past.

2.01 Considerations
-------------------
In version 2.01, the following must also be considered:

* The ``budget-line`` element was introduced.
