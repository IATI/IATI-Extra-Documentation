Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` in context of ``planned-disbursement`` element.

A ``value-date`` for currency conversions must be provided in ISO 8601 format (YYYY-MM-DD).

The ISO 4217 code for the ``currency`` in which the ``planned-disbursement`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 4

Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
