Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` of an ``iati=activity``. 

| This examples declares ``Region`` code *456* with the ``code`` attribute.

| The optional ``RegionVocabulary`` is also be declared as *1* (*OECD DAC*)

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 16

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
