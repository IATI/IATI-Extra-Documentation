Example Usage
~~~~~~~~~~~~~
Example ``sector`` of an ``iati-activity``.

| This example declares ``SectorVocabulary`` code *2* (*OECD DAC CRS Purpose Codes (3 digit)*), using the ``vocabulary`` attribute.
| An example value *111* from this vocabulary is declared with the ``code`` attribute.

.. code-block:: xml

	<sector vocabulary="2" code="111" />
	
| The ``sector`` element can be repeated in any ``iati-activity``.        
| When multiple ``sector`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--sector starts-->
	:end-before: <!--sector ends-->
    
| The ``vocabulary`` is used to declare which ``sector`` classification list is in use. If this is omitted, then IATI assumes *1* (*OECD DAC CRS Purpose Codes (5 digit)*).

| If a vocabulary is not on the ``Vocabulary`` codelist, then the value of *99* (*Reporting Organisation*) should be declared.


Changelog
~~~~~~~~~

1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
