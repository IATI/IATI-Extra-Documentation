Example Usage
~~~~~~~~~~~~~
This is a child element of ``country-budget-items``

Example that declares ``BudgetIdentifier`` code *1.1.1* (Executive - executive):

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->

When multiple ``budget-item`` are declared, then the ``percentage`` values should sum 100% for the specific ``iati-activity``:

.. literalinclude:: ../../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->



Changelog
~~~~~~~~~

1.03
^^^^

Added the optional country-budget-item element

1.02
^^^^

This element did not exist

1.01
^^^^

This element did not exist
