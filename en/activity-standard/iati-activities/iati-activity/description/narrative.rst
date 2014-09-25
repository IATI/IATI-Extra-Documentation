Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``description`` parent element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->
	:emphasize-lines: 2, 6, 10 	
	
The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute:
		
.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->
	:emphasize-lines: 3, 7, 11
	
	
Changelog
~~~~~~~~~
2.01
^^^^
| The ``narrative`` element was introduced in 2.01.
