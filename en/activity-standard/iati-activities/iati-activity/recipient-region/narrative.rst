Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-region`` element.

| Note: Both the ``recipient-region`` and ``recipient-country`` elements still allow both a ``@code`` and descriptive text to be specified. This is to cover the isolated cases where the organisation publishing the data may not agree with name of a country or region given by the lookup codelists IATI uses.  Example in the case of a ``recipient-region`` element.

.. code-block:: xml
	:emphasize-lines: 2
	
	<recipient-region code="589" vocabulary="1">
		<narrative>Middle East, regional (As per WHO Eastern Mediterranean Region)<narrative>
	</recipient-region>

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.

Changelog
~~~~~~~~~

2.01
^^^^
| The ``recipient-region`` element was introduced in 2.01.
