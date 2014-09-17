Example Usage
~~~~~~~~~~~~~
| Example usage of ``language`` of a ``document-link`` in an ``iati-organisation``.
| 
| This example declares the ``Language`` code *en* using the ``language`` attribute.
| Note: This specifies the language of the document being linked to.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link-title starts-->
	:end-before: <!--document-link-title ends-->
	:emphasize-lines: 7

	
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
