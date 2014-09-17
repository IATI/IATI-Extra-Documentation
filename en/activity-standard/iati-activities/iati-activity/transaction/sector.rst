Example Usage
~~~~~~~~~~~~~
Example ``sector`` of a ``transaction`` within an ``iati-activity``.

| This example declares ``SectorVocabulary`` code *2* (*OECD DAC CRS Purpose Codes (3 digit)*) with the ``vocabulary`` attribute.

| An example value *111* from this vocabulary is declared with the ``code`` attribute.

.. code-block:: xml

	<sector vocabulary="2" code="111" />
        
| Note: multiple sectors in a ``transaction``  are expressed by repeating the ``sector`` element.
    
| The ``vocabulary`` is used to declare which ``sector`` classification list is in use. If this is omitted, then IATI assumes *1* (*OECD DAC CRS Purpose Codes (5 digit)*).

| If a vocabulary is not on the ``Vocabulary`` codelist, then the value of *99* (*Reporting Organisation*) should be declared.

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 14

Changelog
~~~~~~~~~

2.01
^^^^

The ``sector`` element was added to ``transaction`` in 2.01
