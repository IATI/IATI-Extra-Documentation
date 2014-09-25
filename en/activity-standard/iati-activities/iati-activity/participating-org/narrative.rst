Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``participant-org`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--participating-org starts-->
	:end-before: <!--participating-org ends-->
	:emphasize-lines: 2, 5, 8	

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.

| One example illustrated below:
		
.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--participating-org starts-->
	:end-before: <!--participating-org ends-->
	:emphasize-lines: 9
	
Changelog
~~~~~~~~~

2.01
^^^^
| The ``narrative`` element was introduced in 2.01.
