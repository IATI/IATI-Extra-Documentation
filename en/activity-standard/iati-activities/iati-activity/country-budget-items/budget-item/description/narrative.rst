Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``description`` parent element.

.. literalinclude:: ../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 4, 9 	
	
The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.
	
	
Changelog
~~~~~~~~~

2.01
^^^^
| The ``narrative`` element was introduced in 2.01.
