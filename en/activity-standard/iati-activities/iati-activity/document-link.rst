Example Usage
~~~~~~~~~~~~~
Example ``document-link`` in an ``iati-actvity``.

| This element is a parent for other child elements.
| 
| This example declares a ``FileFormat`` of *application/vnd.oasis.opendocument.text*, using the ``format`` attribute.

.. code-block:: xml

	<document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_en.odt">
	...
    </document-link>

| Full example with all child elements: 

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 1, 8
	
| The ``document-link`` element can be repeated in any ``iati-activity``.

Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

