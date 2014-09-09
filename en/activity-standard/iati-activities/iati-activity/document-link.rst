Example Usage
~~~~~~~~~~~~~
| Example ``document-link`` with ``FileFormat`` *application/vnd.oasis.opendocument.text*.
|
| The ``DocumentCategory`` is declared as *A01*.
| 
| Note: ``DocumentCategory`` codes with the *A* ``DocumentCategory`` prefix are recommended within the **IATI activity standard** ``document-link`` element.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 1, 5	


Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

