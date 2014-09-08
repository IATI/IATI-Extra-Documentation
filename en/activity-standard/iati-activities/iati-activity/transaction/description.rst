Example Usage
~~~~~~~~~~~~~
Example usage of ``description`` in context of ``transaction`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 3
	
Full example with additional elements which can override the default value set in ``iati-activity``:  

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 3
	
It may be appropriate to repeat the ``description`` in other languages using ``xml:lang`` attribute.  
In this example, the language *en* has been set in the ``iati-activity`` element:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--transaction multi-lang starts-->
	:end-before: <!--transaction multi-lang ends-->
	:emphasize-lines: 3, 4

