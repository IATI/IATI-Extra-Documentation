Usage in practice
~~~~~~~~~~~~~~~~~
This ``document-date`` element would normally be the production or published date of the relevant document to identify the specific document version.

Example Usage
~~~~~~~~~~~~~
| Example usage of the ``document-date`` element within a ``document-link`` as part of an ``iati-activity``.

| This examples declares an ISO date (corresponding to 5th February 2014) using the ``@iso-date`` attribute.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 8

| The ``document-date`` element should only be used once for each ``document-link`` element.		

Changelog
~~~~~~~~~

2.02
^^^^
Added the optional ``document-date`` element was `added <http://support.iatistandard.org/entries/92707776-Document-Dates >`__.
