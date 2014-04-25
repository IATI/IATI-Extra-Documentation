Example Usage
~~~~~~~~~~~~~
Example ``language``, using ``Language`` codes *en* (English):

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->

In this example, the ``document-link`` is provided in two ``language``, with the relevant ``Language`` codes:

.. literalinclude:: ../../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->


Changelog
~~~~~~~~~

1.02
^^^^

Addition of a ``language`` element as a child of the ``document-link`` element:
document-link/language/text() (0..1) - The ISO 639 code for the language
of the document

1.01
^^^^

This element did not exist
