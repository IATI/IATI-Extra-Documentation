Example Usage
~~~~~~~~~~~~~
Example ``budget-item`` within ``country-budget-items`` of an ``iati-activity``.

| This example that declares ``BudgetIdentifier`` code *1.1.1* (*Executive - executive*), using the ``code`` attribute.

.. code-block:: xml
	:emphasize-lines: 2, 5
	
	<country-budget-items vocabulary="2">
		<budget-item code="1.1.1">
			<description>
				<narrative>Description text</narrative>
		</budget-item>
	</country-budget-items>

| The ``budget-item`` element can be repeated in any ``country-budget-items`` of the same ``vocabulary``.  
| When multiple ``budget-item`` elements are declared within a single ``country-budget-items`` element, then, for each ``vocabulary`` used, the ``percentage`` values should sum 100%:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 2, 6, 7, 12


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
