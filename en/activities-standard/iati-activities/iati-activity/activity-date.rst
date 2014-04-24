Example Usage
~~~~~~~~~~~~~
Example of an ``iati-activity`` with one each of the four possible ``ActivityDateType`` codes:

A date in ISO 8601 format (YYYY-MM-DD) is required:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--activity-date starts-->	
	:end-before: <!--activity-date ends-->

In some cases, not all ``ActivityDateType`` can be declared, depending on the ``activity-status`` of the ``iati-activity``:    

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->
	:end-before: <!--activity-date ends-->

Note: In all cases, a ``start-actual`` or ``end-actual`` with a date in the *future*, is not expected.




