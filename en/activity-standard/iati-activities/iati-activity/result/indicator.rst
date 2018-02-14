Example Usage
~~~~~~~~~~~~~
Example usage of ``indicator``  in a ``result`` of an ``iati-activity``.

| This element is a parent for other child elements.  It is also contained within a ``result`` element.

| The ``@measure`` attribute declares a valid code (*1*) from the *IndicatorMeasure* codelist.
| The ``@ascending`` boolean of *1* also declares that the data is asscending.
| The ``@aggregation-status`` *1* boolean is included, for illustration of suitability for aggregation.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->

| The ``indicator`` element can be repeated in any ``result`` of an ``iati-activity``.

Changelog
~~~~~~~~~

2.03
^^^^
The optional attribute ``@aggregation-status`` was `added <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.
