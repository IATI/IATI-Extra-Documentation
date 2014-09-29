Example Usage
~~~~~~~~~~~~~
Example usage of ``administrative`` within a ``location`` of an ``iati-activity``.

| The ``@vocabulary`` attribute declares a valid code (*G1*) from the *GeographicVocabulary* codelist.
| An example value of *1453782* from that vocabulary is declared in the ``@code`` attribute.
| An example value of *1* is declared for the ``@level`` attribute. 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 13

Changelog
~~~~~~~~~

2.01
^^^^
| Freetext is no longer allowed within this element.

1.04
^^^^

| In 1.04 the @country, @adm1 and @adm2 attributes were deprecated. The new attributes replace the function of the previous ones.
