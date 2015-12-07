Usage in practice
~~~~~~~~~~~~~~~~~

The purpose of planned-disbursement is to describe any predefined payment schedule.

Planned disbursements should relate to an actual transfer of funds.

Planned disbursements do not replace the activity-budget.


Example Usage
~~~~~~~~~~~~~
Example ``planned-disbursement`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@type`` attribute declares a valid code (*1*) from the *BudgetType* codelist.

.. code-block:: xml

	<planned-disbursement type="1">
	...
	</planned-disbursement>
	
| Note: If omitted, then *BudgetType* code *1* (Original) is assumed.

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 1, 11
	
| Note: multiple planned disbursements are expressed by repeating the ``planned-disbursement`` element.	

Changelog
~~~~~~~~~
2.01
^^^^
The attribute ``@last-updated`` was `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#planned-disbursement-removed-renamed-attributes>`__.

The attribute ``@type`` was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#planned-disbursement-removed-renamed-attributes>`__.


1.05
^^^^
A description was added to this element
