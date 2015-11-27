Example Usage
~~~~~~~~~~~~~
| Example usage of the ``document-date`` element within a ``document-link`` as part of an ``iati-organisation``.

| This examples declares an ISO date (corresponding to 5th February 2014) using the ``@iso-date`` attribute.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 7

| The ``document-date`` element should only be used once for each ``document-link`` element.		

Changelog
~~~~~~~~~

2.02
^^^^
Added the optional ``document-date`` element was `added <http://support.iatistandard.org/entries/92707776-Document-Dates>`__.
