Example Usage
~~~~~~~~~~~~~
This is a child element of ``country-budget-items``

Example that declares ``BudgetIdentifier`` code *1.1.1* (*Executive - executive*):

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 2, 4

When multiple ``budget-item`` elements are declared within a single ``country-budget-items`` element, then, for each ``vocabulary`` used, the ``percentage`` values should sum 100%:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 2, 6


Changelog
~~~~~~~~~

1.04
^^^^

The @percentage attribute had been erroneously set to be required in the schema on it's introduction in 1.03. This has now been set to 'optional' in the schema.

1.03
^^^^

Added the optional country-budget-item element

1.02
^^^^

This element did not exist

1.01
^^^^

This element did not exist
