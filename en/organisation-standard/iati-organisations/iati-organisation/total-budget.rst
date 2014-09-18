Example Usage
~~~~~~~~~~~~~
| Example of ``total-budget`` for an ``iati-organisation``.
| 
| This element is a parent for other child elements.

.. code-block:: xml

	<total-budget>
	...
	</total-budget>

| Full example with all child element.

.. code-block:: xml
	:emphasize-lines: 1, 9

		<total-budget>
			<period-start iso-date="2014-01-01" />
			<period-end iso-date="2014-12-31" />
			<value currency="USD" value-date="2014-01-01">250000000</value>
			<budget-line ref="1234">
				<value value-date="2014-01-01">200000000</value>
				<narrative>Budget Line 1</narrative>
			</budget-line>
		</total-budget>

	
| The ``total-budget`` element can be repeated in any ``iati-organisation``. 
		
.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
	:emphasize-lines: 1, 13, 18, 19, 23
