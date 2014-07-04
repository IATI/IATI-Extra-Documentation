Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` with relevant ``Region`` code.
The optional ``RegionVocabulary`` is also be declared

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-region starts-->
	:end-before: <!--recipient-region ends-->

When multiple ``recipient-region`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--recipient-region starts-->
	:end-before: <!--recipient-region ends-->
	
Additionally, the name of the ``Region`` can also be declared:

.. code-block:: xml

    <recipient-region code="289">South of Sahara, regional<recipient-region>


Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
