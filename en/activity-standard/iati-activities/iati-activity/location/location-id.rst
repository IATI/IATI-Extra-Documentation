Example Usage
~~~~~~~~~~~~~
Example usage of ``location-id`` within a ``location`` of an ``iati-activity``..

| This example declares a ``GeographicVocabulary`` code *G1* (Geonames), using the ``vocabulary`` attribute.

| An example value of *1453782* from that vocabulary is declared in the ``code`` attribute.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 3
	
Note: If the ``vocabulary`` *G2* (*Open Street Map*) is used, then the ``code`` value should be of the form <OSM element>/<OSM identifier>

The OSM element will be a node, way or relation. 

| Examples:

* node/1234567
* way/1234567
* relation/1234567

.. code-block:: xml

    <location-id vocabulary="G2" code="node/25524229" />


Changelog
~~~~~~~~~

1.04
^^^^

| New in 1.04
| The location-id element was introduced in 1.04 to replace the gazetteer-entry element which was deprecated in 1.04
