Example Usage
~~~~~~~~~~~~~
| Example usage of ``language`` in context of ``document-link`` element.
| NB: This specifies the language of the document being linked to.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link-title starts-->
	:end-before: <!--document-link-title ends-->
	:emphasize-lines: 7

| It may be appropriate to repeat the ``document-link`` element if the document is available in other languages:
| Note: This specifies the language of the document being linked to.  In this example, the ``title`` element still uses ``xml:lang`` to declare the title in two languages.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link-lang starts-->
	:end-before: <!--document-link-lang ends-->
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
