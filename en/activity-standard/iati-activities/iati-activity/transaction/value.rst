Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` of a ``transaction`` in an ``iati-activity``.

| A date in ISO 8601 format (YYYY-MM-DD) for the ``value-date`` attribute is required.

| The ISO 4217 code for the ``currency`` in which the ``transaction`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 4
	
Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of
integers.
