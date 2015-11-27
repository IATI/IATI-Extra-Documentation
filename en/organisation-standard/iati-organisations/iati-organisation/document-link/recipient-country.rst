Example Usage
~~~~~~~~~~~~~
| Example usage of ``recipient-country`` of a ``document-link`` in an ``iati-organisation``.

| The ``@code`` attribute declares a valid code (*AF*) from the *Country* codelist.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 8

| The ``recipient-country`` element can be repeated in any ``document-link``.
| Example declaring multiple ``recipient-country`` elements for the same ``document-link``:

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-country-document-link starts-->
	:end-before: <!--multi-country-document-link ends-->
	:emphasize-lines: 8, 9, 10

	
Changelog
~~~~~~~~~

2.01
^^^^
| The ``recipient-country`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#document-link-new-child-element>`__ as a child element of ``document-link``.

