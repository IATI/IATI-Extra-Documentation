Example Usage
~~~~~~~~~~~~~
Example ``country-budget-items`` for an ``iati-activity``.

| This element is a parent for other child elements.
|
| This example declares ``BudgetIdentifierVocabulary`` code *2* (*Country Chart of Accounts*), using the ``vocabulary`` attribute.

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

Changelog
~~~~~~~~~

1.03
^^^^

This is a new element, introduced in version 1.03 of the standard

1.02
^^^^

This element did not exist

1.01
^^^^

This element did not exist
