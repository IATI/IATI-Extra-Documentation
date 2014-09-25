Example Usage
~~~~~~~~~~~~~
Example usage of ``commitment-date`` within ``loan-terms`` in context of ``crs-add`` element.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->
	:emphasize-lines: 6

Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
