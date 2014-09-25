Example Usage
~~~~~~~~~~~~~
Example ``value`` of ``total-budget`` for an ``iati-organisation``.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a ``Curency`` code *USD*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-organisation`` element.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
	:emphasize-lines: 4, 17, 22
			
Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
