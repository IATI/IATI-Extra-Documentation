Example Usage
~~~~~~~~~~~~~
Example ``document-link`` with ``FileFormat`` *application/vnd.oasis.opendocument.text*.
The ``DocumentCategory`` is declared as *B01*.
In this example, the ``document-link`` is provided in two ``language``
For each ``language`` a relevant ``title``, ``Language`` code and ``url`` is provided:

Note: ``DocumentCategory`` codes with the *B* ``DocumentCategory-category`` prefix are recommended within the **IATI organisation standard**  ``document-link`` element.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 1, 5, 6, 10
	
Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

