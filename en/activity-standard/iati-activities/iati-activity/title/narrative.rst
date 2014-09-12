Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``title`` parent element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--title starts-->
	:end-before: <!--title ends-->
	:emphasize-lines: 2	

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute:
		
.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--title starts-->
	:end-before: <!--title ends-->
	:emphasize-lines: 3, 4
	
Note: It is recommended to provide a ``title`` in the language(s) spoken in the country(ies) where the ``iati-activity`` take place, or is aimed at.	
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
