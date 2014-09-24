Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-country`` element.

| Note: the ``narrative`` element is optional and should only be used to provide any essential clarification additional to name available in the ``Country`` codelist.  

| In this example, it is shown just once.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 3

| Note: The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``xml:lang`` attribute.  Example not shown.
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
