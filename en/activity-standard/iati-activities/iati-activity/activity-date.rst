Example Usage
~~~~~~~~~~~~~
Example ``activity-date`` for an``iati-activity``.

| In this example each of the four possible ``ActivityDateType`` codes are used with the ``type`` attribute.

| Each example has a date in the required ISO 8601 format (YYYY-MM-DD), declared in the ``iso-date`` attribute.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->	
	:end-before: <!--activity-date ends-->
	:emphasize-lines: 1, 4, 5, 6 	
	
Note: In some cases, not all ``ActivityDateType`` can be declared, depending on the ``activity-status`` of the ``iati-activity``

| Note: In all cases, a ``start-actual`` or ``end-actual`` with a date in the *future*, is not expected.


