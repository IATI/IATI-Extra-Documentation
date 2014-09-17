Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-country-budget`` for an ``iati-organisation``.
| 
| This element is a parent for other child elements.

.. code-block:: xml

	<recipient-country-budget>
	...
	</recipient-country-budget>

| Full example with all child element.

.. code-block:: xml
	:emphasize-lines: 1, 12

		<recipient-country-budget>
			<recipient-country code="AF">
				<narrative>Country name</narrative>
			</recipient-country>
			<period-start iso-date="2014-01-01" />
			<period-end iso-date="2014-12-31" />
			<value currency="USD" value-date="2014-01-01">25000000</value>
			<budget-line ref="1234">
				<value value-date="2014-01-01">2000000</value>
				<narrative>Budget Line 1</narrative>
			</budget-line>
		</recipient-country-budget>
	
| The ``recipient-country-budget`` element can be repeated in any ``iati-organisation``. 
		
.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 1, 16, 17, 22, 23, 28
