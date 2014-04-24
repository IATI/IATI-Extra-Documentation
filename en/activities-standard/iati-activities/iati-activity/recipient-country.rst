Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` with relevant ``Country`` code:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--recipient-country starts-->
	:end-before: <!--recipient-country ends-->

When multiple ``recipient-country`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--recipient-country starts-->
	:end-before: <!--recipient-country ends-->

Additionally, the name of the ``Country`` can also be declared:

.. code-block:: xml

    <recipient-country code="AF">Afghanistan</recipient-country>    

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
