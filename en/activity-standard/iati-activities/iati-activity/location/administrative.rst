Example Usage
~~~~~~~~~~~~~
Example usage of ``administrative`` within a ``location`` of an ``iati-activity``.

| The ``@vocabulary`` attribute declares a valid code (*G1*) from the *GeographicVocabulary* codelist.
| An example value of *1453782* from that vocabulary is declared in the ``@code`` attribute.
| An example value of *1* is declared for the ``@level`` attribute.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location-single starts-->
	:end-before: <!--location ends-->

Note: Multiple administrative levels can be reported by repeating the ``administrative`` element:

.. code-block:: xml

	<location ref="AF-KAN">
	   <location-id vocabulary="G1" code="1453782" />
	   <name>Location name</name>
	   <description>Location description</description>
	   <activity-description>A description that qualifies the activity taking place at the location</activity-description>
	   <administrative level="0" code="1149361" vocabulary="G1" />
	   <administrative level="1" code="1453782" vocabulary="G1" />
	   <point srsName="http://www.opengis.net/def/crs/EPSG/0/4326">
	    <pos>31.616944 65.716944</pos>
	   </point>
	   <exactness code="1"/>
	   <location-reach code="1" />
	   <location-class code="2"/>
	   <feature-designation code="PRNQ"/>
	  </location>

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

The @county, @adm1 and @adm2 attributes were `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#location-removed-attributes>`__.

1.04
^^^^

| In 1.04 the @country, @adm1 and @adm2 attributes were deprecated. The new attributes replace the function of the previous ones.
