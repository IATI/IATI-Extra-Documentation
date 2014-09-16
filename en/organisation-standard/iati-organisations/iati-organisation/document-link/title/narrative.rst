Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``title`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 3

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``xml:lang`` attribute.

| Note: This relates to the language of the text in the XML.
		
.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link-title starts-->
	:end-before: <!--document-link-title ends-->
	:emphasize-lines: 4
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
