Example Usage
~~~~~~~~~~~~~
Example ``budget`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@type`` attribute declares a valid code (*1*) from the *BudgetType* codelist.

.. code-block:: xml

	<budget type="1">
	...
	</budget>
	
| Note: If omitted, then *BudgetType* code *1* (Original) is assumed.

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->
	:emphasize-lines: 1, 5

| The ``budget`` element can be repeated in any ``iati-activity``.      
