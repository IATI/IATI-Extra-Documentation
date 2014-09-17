Example Usage
~~~~~~~~~~~~~
Example ``activity-date`` for an``iati-activity``.

| In this example, an ``ActivityDateType`` code *1* (*start planned*) is declared, using the ``type`` attribute.
.. code-block:: xml

	<activity-date iso-date="2012-04-28" type="1" />

| The ``activity-date`` element can be repeated in any ``iati-activity``.    
| In this example four ``activity-date`` are declared.

| An ``ActivityDateType`` code is declared for each date, using the ``type`` attribute.
| Each example date is declared in the ``iso-date`` attribute.
| Example date formats conform to the xsd:date standard - for most cases *YYYY-MM-DD* is sufficient.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->	
	:end-before: <!--activity-date ends-->
	:emphasize-lines: 1, 4, 5, 6 	
	
Note: In some cases, not all ``ActivityDateType`` can be declared, depending on the ``activity-status`` of the ``iati-activity``
| 
| Note: In all cases, dates of ``type`` *actual* are not expected to be in the *future*.


