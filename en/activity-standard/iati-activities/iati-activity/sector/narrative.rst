Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``sector`` element.

| The ``narrative`` element should be used specially when the *99* (Reporting Organisation) or *98* (Reporting Organisation 2) *SectorVocabulary* are declared.

.. code-block:: xml
	:emphasize-lines: 2
	
	<sector vocabulary="98" vocabulary-uri="http://example.com/vocab.html" code="A1" percentage="100">
		<narrative>A description of the sector</narrative>
	</sector>

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.

Changelog
~~~~~~~~~

2.01
^^^^
| The ``narrative`` element was introduced in 2.01.
