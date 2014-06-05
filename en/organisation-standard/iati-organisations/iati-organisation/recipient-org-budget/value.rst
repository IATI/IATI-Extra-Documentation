Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` in context of ``recipient-org-budget`` element.

A ``value-date`` for currency conversions must be provided in ISO 8601 format (YYYY-MM-DD).

The ISO 4217 code for the ``currency`` in which the ``recipient-org-budget`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-organisation`` element.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 5, 11, 17
			
Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
