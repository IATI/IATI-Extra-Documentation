Example Usage
~~~~~~~~~~~~~
Example usage of ``exactness`` within a ``location`` of an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*1*) from the *GeographicExactness* codelist.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location-single starts-->
	:end-before: <!--location ends-->


Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

1.04
^^^^

| New in 1.04
| This is used as a replacement for the deprecated location/coordinates/@precision attribute

