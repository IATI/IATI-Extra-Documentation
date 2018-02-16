Example Usage
~~~~~~~~~~~~~
| Example usage of ``language`` of a ``document-link`` in a ``indicator`` in a ``result`` element.

| The ``@language`` attribute declares a valid code (*en*) from the *Language* codelist.
| Note: This specifies the language of the document being linked to.

.. literalinclude:: ../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-document-link example starts-->
	:end-before: <!--result-document-link example ends-->

| In some cases, a ``document-link`` may be in multiple languages.  This is expressed by repeating the ``language`` element.

Changelog
~~~~~~~~~

2.03
^^^^
The optional ``language`` element of a ``document-link`` in a ``indicator`` in a ``result`` element was `added <https://discuss.iatistandard.org/t/add-document-link-to-results-indicator-included-2-03/895>`__.
