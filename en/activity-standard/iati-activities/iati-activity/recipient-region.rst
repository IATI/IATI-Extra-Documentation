Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` of an ``iati=activity``. 
| 
| This examples declares the ``Region`` code *456*, using the ``code`` attribute.
| This examples declares the optional ``RegionVocabulary`` *1* (*OECD DAC*), using the ``vocabulary`` attribute.

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />

| The ``recipient-region`` element can be repeated in any ``iati-activity``.
| When multiple ``recipient-region`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``.
        
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-region starts-->
	:end-before: <!--recipient-region ends-->

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
