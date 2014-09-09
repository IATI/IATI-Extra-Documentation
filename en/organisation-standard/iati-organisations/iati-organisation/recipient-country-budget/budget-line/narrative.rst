Example Usage
~~~~~~~~~~~~~
The ``narrative`` sub-element can be used to declare freetext for the ``budget-line`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 10, 14

| Note: The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisations``, by using the ``xml:lang`` attribute.  Example not shown.

	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``budget-line`` element was introduced in 2.01.
