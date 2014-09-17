Example Usage
~~~~~~~~~~~~~
Example usage of ``indicator``  in a ``result`` of an ``iati-activity``.

| This element is a parent for other child elements.  It is also contained within a ``result`` element.  
| 
| This example declares ``IndicatorMeasure`` code of *1* (*Unit*), using the ``measure`` attribute. 
| A boolean *1* also declares that the data is ``ascending``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 10, 41
		
| The ``indicator`` element can be repeated in any ``result`` of an ``iati-activity``.
