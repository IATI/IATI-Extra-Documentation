Example Usage
~~~~~~~~~~~~~

Example ``document-link`` in a ``indicator`` in a ``result`` element.

| This element is a parent for other child elements.

| The ``@format`` attribute declares a valid code (*application/vnd.oasis.opendocument.text*) from the *FileFormat* codelist.
| The ``@url`` attribute provides the document location.

.. code-block:: xml

    <document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/result_indicator_en.odt">
    ...
    </document-link>

| Full example with all child elements:

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-indicator starts-->
	:end-before: <!--result-indicator ends-->

| The ``document-link`` element can be repeated in any ``result`` element.

Changelog
~~~~~~~~~

2.03
^^^^
The optional ``document-link`` element was `added <https://discuss.iatistandard.org/t/add-document-link-to-results-indicator-included-2-03/895>`__.
