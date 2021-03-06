Example Usage
~~~~~~~~~~~~~~~~~

This ``document-date`` element would normally be the production or published date of the relevant document to identify the specific document version.

Example Usage
~~~~~~~~~~~~~
| Example usage of the ``document-date`` element within a ``document-link`` in a ``indicator`` as part of a ``result`` element.

| This examples declares an ISO date (corresponding to 5th February 2014) using the ``@iso-date`` attribute.

.. literalinclude:: ../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-document-link example starts-->
	:end-before: <!--result-document-link example ends-->

| The ``document-date`` element should only be used once for each ``document-link`` element.

Changelog
~~~~~~~~~

The optional ``document-date`` element of a ``document-link`` in a ``indicator`` in a ``result`` element was `added <https://discuss.iatistandard.org/t/add-document-link-to-results-indicator-included-2-03/895>`__.
