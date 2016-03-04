Example Usage
~~~~~~~~~~~~~
Example usage of ``loan-status`` in context of ``crs-add`` element.

| This element is a parent for other child elements.

| This example declares the attribute ``@year`` as *2014*.

| An example date is declared in the ``@iso-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a *Currency* code *GBP*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->
	:emphasize-lines: 10, 15


Changelog
~~~~~~~~~

1.03
^^^^
| New in 1.03
| Added the optional ``crs-add`` element and its child elements
