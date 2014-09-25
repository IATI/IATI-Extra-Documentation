Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``activity-date`` element.

| Note: In this example, free text ``narrative`` has been included with the just one ``activity-date`` element.  This is entirely optional, and best applied when such text can add additional clarification to the ``activity-date``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->	
	:end-before: <!--activity-date ends-->
	:emphasize-lines: 2	

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.

| One example illustrated below:
		
.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->	
	:end-before: <!--activity-date ends-->
	:emphasize-lines: 3
	
Changelog
~~~~~~~~~
2.01
^^^^
| The ``narrative`` element was introduced in 2.01. 
