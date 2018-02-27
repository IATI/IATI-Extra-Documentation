Example Usage
~~~~~~~~~~~~~
Example ``budget`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@type`` attribute declares a valid code (*1*) from the *BudgetType* codelist.
| The ``@status`` attribute declares a valid code (*1*) from the *BudgetStatus* codelist.

.. code-block:: xml

	<budget type="1" status="1">
	...
	</budget>
	
| Note: If the @type attribute is omitted, then *BudgetType* code *1* (Original) is assumed.
| Similarly, if the @status attribute is omitted, then *BudgetStatus* code *1* (Indicative) is assumed.

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->
	:emphasize-lines: 1, 5

| The ``budget`` element can be repeated in any ``iati-activity``.      

Changelog
~~~~~~~~~

2.02
^^^^
The ``status`` attribute was `added <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__.

The ``budget`` definition was updated as a `bug fix <https://discuss.iatistandard.org/t/proposal-update-of-budget-element-description-text-in-activity-standard/1216>`__ on the 27/02/2018.
