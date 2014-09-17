Example Usage
~~~~~~~~~~~~~
Example ``planned-disbursement`` for an ``iati-activity``.

| This element is a parent for other child elements.
| 
| This example declares ``BudgetType`` code *1* (*Original*), using the ``type`` attribute.

.. code-block:: xml

	<budget type="1">
	...
	</budget>
	
| Note: If omitted, then ``BudgetType`` code *1* (*Original*) is assumed.
| 
| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 1, 5
	
| Note: multiple planned disbursements are expressed by repeating the ``planned-disbursement`` element.	

Changelog
~~~~~~~~~
2.01
^^^^
The attribute ``last-updated`` was removed.
The attribute ``type`` was added.


1.05
^^^^
A description was added to this element
