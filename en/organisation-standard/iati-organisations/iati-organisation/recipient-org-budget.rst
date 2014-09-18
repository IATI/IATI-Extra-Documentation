Example Usage
~~~~~~~~~~~~~
Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-org-budget`` for an ``iati-organisation``.
| 
| This element is a parent for other child elements.

.. code-block:: xml

	<recipient-org-budget>
	...
	</recipient-org-budget>

| Full example with all child element.

.. code-block:: xml
	:emphasize-lines: 1, 12

		<recipient-org-budget>
			<recipient-org ref="AA-ABC-1234567">
				<narrative>Country name</narrative>
			</recipient-org>
			<period-start iso-date="2014-01-01" />
			<period-end iso-date="2014-12-31" />
			<value currency="USD" value-date="2014-01-01">2500000</value>
			<budget-line ref="1234">
				<value value-date="2014-01-01">2000000</value>
				<narrative>Budget Line 1</narrative>
			</budget-line>
		</recipient-org-budget>
	
| The ``recipient-org-budget`` element can be repeated in any ``iati-organisation``. 
		
.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 1, 16, 17, 24, 25, 32
