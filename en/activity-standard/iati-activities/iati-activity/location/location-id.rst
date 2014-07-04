Example Usage
~~~~~~~~~~~~~
Example usage of ``location-id`` within context of ``location``.

| This example declares a ``GeographicVocabulary`` code *G1* (Geonames) and a relevant ``code``  from that vocabulary: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 2
	
If the G2 vocabulary (Open Street Map) is used the code value should be of the form <OSM element>/<OSM identifier>

The OSM element will be a node, way or relation. Examples:

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
