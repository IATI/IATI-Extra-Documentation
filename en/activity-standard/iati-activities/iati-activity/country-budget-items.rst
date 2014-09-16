Example Usage
~~~~~~~~~~~~~
Example ``country-budget-items`` for an ``iati-activity``.

| This element is a parent for other child elements.

| This example declares ``BudgetIdentifierVocabulary`` code *2* (*Country Chart of Accounts*) with the ``vocabulary`` attribute.

.. code-block:: xml

    <country-budget-items vocabulary="2">
	...
    </country-budget-items>
    
Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 1, 7


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
