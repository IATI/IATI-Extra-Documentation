Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-country`` element.

| Note: the ``narrative`` element is optional and should only be used to provide any essential clarification additional to the name available in the *Country* codelist.  

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-country-document-link starts-->
	:end-before: <!--multi-country-document-link ends-->
	:emphasize-lines: 9

| Note: The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``@xml:lang`` attribute.  Example not shown.
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``recipient-country`` element was introduced in 2.01.
