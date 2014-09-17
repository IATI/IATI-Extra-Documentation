Example Usage
~~~~~~~~~~~~~
Example ``participating-org`` in an ``iati-activity``.

.. code-block:: xml

	<participating-org ref="BB-BBB-123456789" role="2" type="40">
		<narrative>Name of Agency B</narrative>
	</participating-org>
	
| The ``participating-org`` element can be repeated in any ``iati-activity``.
| In this example, three ``participating-org`` are declared.
|
| An organisation ``ref`` is provided for each. 
| An ``OrganisationRole`` code is declared for each organisation, with the ``role`` attribute.
| An ``OrganisationType`` code is declared for each organisation, with the ``type`` attribute.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--participating-org starts-->
	:end-before: <!--participating-org ends-->
	:emphasize-lines: 1, 3, 4, 6, 7, 10		
