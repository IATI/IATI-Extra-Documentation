Example Usage
~~~~~~~~~~~~~
Example usage of ``exactness`` within a ``location`` of an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*1*) from the *GeographicExactness* codelist.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 17


Changelog
~~~~~~~~~

2.01
^^^^
| Freetext is no longer allowed within this element.

1.04
^^^^

| New in 1.04
| This is used as a replacement for the deprecated location/coordinates/@precision attribute

