Example Usage
~~~~~~~~~~~~~
Example usage of ``indicator``  in a ``result`` of an ``iati-activity``.

| This element is a parent for other child elements.  It is also contained within a ``result`` element.

| The ``@measure`` attribute declares a valid code (*1*) from the *IndicatorMeasure* codelist.
| The ``@ascending`` boolean of *1* also declares that the data is asscending.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->

| The ``indicator`` element can be repeated in any ``result`` of an ``iati-activity``.
