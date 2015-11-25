Example Usage
~~~~~~~~~~~~~
Example ``country-budget-items`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@vocabulary`` attribute declares a valid code (*2*) from the *BudgetIdentifierVocabulary* codelist.

.. code-block:: xml

    <country-budget-items vocabulary="2">
	...
    </country-budget-items>
    
Full example with all child elements:

.. code-block:: xml
	:emphasize-lines: 1, 7
	
	<country-budget-items vocabulary="2">
		<budget-item code="1.1.1">
			<description>
				<narrative>Description text</narrative>
			</description> 
		</budget-item>
	</country-budget-items>


Changelog
~~~~~~~~~

1.03
^^^^
This is a new element, introduced in version 1.03 of the standard.

