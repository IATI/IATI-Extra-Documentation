Example Usage
~~~~~~~~~~~~~
Example usage of ``period-end`` of ``planned-disbursement`` for an ``iati-activity``.

| An example date is declared in the ``@iso-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 3
	
| In some instances, it may not be feasible to declare an ``period-end`` date.  In such cases, the element is not included:

.. code-block:: xml
	
	<planned-disbursement type="1">
		<period-start iso-date="2014-01-01" />
		<value currency="EUR" value-date="2014-01-01">3000</value>
	</planned-disbursement>


Changelog
~~~~~~~~~

2.02
^^^^
The definition of this element was amended for clarity.
