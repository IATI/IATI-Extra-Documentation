Example Usage
~~~~~~~~~~~~~
| Example usage of ``language`` of a ``document-link`` in an ``iati-activity``.

| The ``@language`` attribute declares a valid code (*en*) from the *Language* codelist.
| Note: This specifies the language of the document being linked to.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 7

| In some cases, a ``document-link`` may be in multiple languages.  This is expressed by repeating the ``language`` element.

.. code-block:: xml
	:emphasize-lines: 7, 8
	
	<document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report.odt">
		<title>
			<narrative>Project Report 2013</narrative>	   
			<narrative xml:lang="fr">Rapport de projet 2013</narrative>
		</title>
		<category code="A01" />
		<language code="en" />
		<language code="fr" />
	</document-link>

Changelog
~~~~~~~~~

1.02
^^^^
Addition of a ``@language`` element as a child of the ``document-link`` element:
document-link/language/text() (0..1) - The ISO 639 code for the language
of the document

