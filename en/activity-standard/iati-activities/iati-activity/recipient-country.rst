Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` of an ``iati=activity``.
| 
| This examples declares the ``Country`` code *AF*, using the ``code`` attribute.

.. code-block:: xml

        <recipient-country code="AF" />

| The ``recipient-country`` element can be repeated in any ``iati-activity``.
| When multiple ``recipient-country`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country starts-->
	:end-before: <!--recipient-country ends-->
 

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
