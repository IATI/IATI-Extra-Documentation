Example Usage
~~~~~~~~~~~~~
Example ``budget-item`` within ``country-budget-items`` of an ``iati-activity``.

| The ``@code`` attribute declares a code (*1844*) provided from the *Reporting Organisation's* codelist.

.. code-block:: xml

	<country-budget-items vocabulary="4">
		<budget-item code="1844">
			<description>
				<narrative>Description text</narrative>
			</description>
		</budget-item>
	</country-budget-items>

| The ``budget-item`` element can be repeated in any ``country-budget-items`` of the same ``vocabulary``.
| When multiple ``budget-item`` elements are declared within a single ``country-budget-items`` element, then, for each ``vocabulary`` used, the ``percentage`` values should sum 100%:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->


Changelog
~~~~~~~~~

1.04
^^^^
The @percentage attribute had been erroneously set to be required in the schema on it's introduction in 1.03. This has now been set to 'optional' in the schema.

1.03
^^^^
Added the optional country-budget-item element
