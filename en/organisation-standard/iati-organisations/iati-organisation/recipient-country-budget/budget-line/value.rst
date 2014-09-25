Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` in context of ``budget-line`` element.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a ``Curency`` code *USD*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-organisation`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 9, 13
			
Changelog
~~~~~~~~~
2.01
^^^^

| The ``budget-line`` element was introduced in 2.01.

