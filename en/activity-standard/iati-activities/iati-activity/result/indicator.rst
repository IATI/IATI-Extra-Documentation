Example Usage
~~~~~~~~~~~~~
The ``indicator`` element acts as a container for other elements.

It is also contained within a ``result`` element.  

Example usage of ``indicator`` in context of ``result`` element.

Example ``indicator`` with the ``IndicatorMeasure`` code of *1* (Unit). 

This example also declares that the data is ``ascending``, via a boolean:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 4, 20


The ``indicator`` element can be repeated within any ``result`` element:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--multi-indicator result starts-->
	:end-before: <!--multi-indicator result ends-->
	:emphasize-lines: 4, 14, 15, 25
		
		
