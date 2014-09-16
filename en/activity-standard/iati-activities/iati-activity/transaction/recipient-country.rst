Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` of ``transaction`` in an ``iati=activity``.

| This examples declares ``Country`` code *AF* with the ``code`` attribute.

.. code-block:: xml

        <recipient-country code="AF" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 15

 

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
