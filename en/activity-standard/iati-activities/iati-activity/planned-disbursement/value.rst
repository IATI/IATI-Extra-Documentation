Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` in context of ``planned-disbursement`` element.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a *Currency* code *EUR*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->

Changelog
~~~~~~~~~

1.03
^^^^
Values are now allowed to be declared as decimals instead of integers.
