Example Usage
~~~~~~~~~~~~~
Example ``document-link`` with ``FileFormat`` *application/vnd.oasis.opendocument.text*.
The ``DocumentCategory`` is declared as *B01*.
In this example, the ``document-link`` is provided in two ``language``
For each ``language`` a relevant ``title``, ``Language`` code and ``url`` is provided:

Note: ``DocumentCategory`` codes with the B prefix are recommended within the ``iati-organisation`` ``document-link`` element.

	.. literalinclude:: ../../organisation-standard-example-1.04-annotated.xml
		:language: xml
		:start-after: <!--document-link starts-->
		:end-before: <!--document-link ends-->

Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

