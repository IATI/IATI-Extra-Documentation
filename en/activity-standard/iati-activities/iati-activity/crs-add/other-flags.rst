Example Usage
~~~~~~~~~~~~~
Example usage of ``other-flags`` of ``crs-add`` for an ``iati-activity``.

| This example declares ``CRSAddOtherFlags`` code *1* (*Free standing technical cooperation*) with the usage of ``code`` attribute.

| A ``significance`` boolean of *1* indicates that this flag is reported.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->
	:emphasize-lines: 2


Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
