Usage in practice
~~~~~~~~~~~~~~~~~
The ``period start`` should define when the actual transfer of funds will take place, if a specific date is known. If the specific payment date is not known, the period in which the transfer is due to take place should be described by using both ``period-start`` and ``period-end`` dates.

The timeframe between ``period-start`` and ``period-end`` should not normally exceed 3 calendar months.

Example Usage
~~~~~~~~~~~~~
Example usage of ``period-end`` of ``planned-disbursement`` for an ``iati-activity``.

| An example date is declared in the ``@iso-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->

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
