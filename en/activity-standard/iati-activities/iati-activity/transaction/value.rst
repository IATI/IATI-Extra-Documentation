Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` of a ``transaction`` in an ``iati-activity``.
| 
| An example date is declared in the ``value-date`` attribute.
| This example date format conform to the xsd:date standard - for most cases *YYYY-MM-DD* is sufficient.
| 
| This example declares a ``Curency`` code *EUR*, using the ``currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``default-currency`` in the ``iati-activity`` element.

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
