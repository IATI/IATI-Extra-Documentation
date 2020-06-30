Example Usage
~~~~~~~~~~~~~
| Example usage of ``language`` of a ``document-link`` in an ``iati-organisation``.

| The ``@language`` attribute declares a valid code (*en*) from the *Language* codelist.
| Note: This specifies the language of the document being linked to.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link-title starts-->
	:end-before: <!--document-link-title ends-->

| In some cases, a ``document-link`` may be in multiple languages.  This is expressed by repeating the ``language`` element.

.. code-block:: xml

	<document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report.odt">
		<title>
			<narrative>Annual Report 2013</narrative>
			<narrative xml:lang="fr">Rapport annuel 2013</narrative>
		</title>
		<category code="B01" />
		<language code="en" />
		<language code="fr" />
	</document-link>

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

| In 2.01 this element usage rules were changed, to allow it to be repeated.

1.02
^^^^
Addition of a ``@language`` element as a child of the ``document-link`` element:
document-link/language/text() (0..1) - The ISO 639 code for the language
of the document

.. meta::
  :order: 4
