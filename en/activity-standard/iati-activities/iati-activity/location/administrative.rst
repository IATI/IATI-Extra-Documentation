Example Usage
~~~~~~~~~~~~~
Example usage of ``administrative`` within a ``location`` of an ``iati-activity``.

| This example declares a ``GeographicVocabulary`` code *G1* (*Geonames*) with the ``vocabulary`` attribute.

| An example value of *1453782* from that vocabulary is declared in the ``code`` attribute.

| An example value of *1* is declared for the ``level`` attribute. 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 13

Changelog
~~~~~~~~~

1.04
^^^^

| In 1.04 the @country, @adm1 and @adm2 attributes were deprecated. The new attributes replace the function of the previous ones.
