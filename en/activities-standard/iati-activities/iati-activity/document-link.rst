Example Usage
~~~~~~~~~~~~~
Example ``document-link`` with ``FileFormat`` *application/vnd.oasis.opendocument.text*.
The ``DocumentCategory`` is declared as *A01*.

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->

In this example, the ``document-link`` is provided in two ``language``
For each ``language`` a relevant ``title``, ``Language`` code and ``url`` is provided:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->

Note: ``DocumentCategory`` codes with the *A* ``DocumentCategory-category`` prefix are recommended within the **IATI activity standard** ``document-link`` element.

Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

