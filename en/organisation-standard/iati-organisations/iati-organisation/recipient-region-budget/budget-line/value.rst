Example Usage
~~~~~~~~~~~~~
Example usage of ``value`` in context of ``budget-line`` element.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a ``Curency`` code *USD*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-organisation`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-region-budget starts-->
	:end-before: <!--recipient-region-budget ends-->
	:emphasize-lines: 7
			
Changelog
~~~~~~~~~
2.02
^^^^
The optional ``recipient-region-budget`` element was `added <http://support.iatistandard.org/entries/79323113-Org-Standard-recipient-region-budget>`__.
