Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``humanitarian-scope`` element.

| The ``narrative`` element should be used only when the *99* (*Reporting Organisation*) *HumanitarianScopeVocabulary* is declared.

.. code-block:: xml

	<humanitarian-scope type="1" vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="5">
	  <narrative>Nepal Earthquake (April 2015)</narrative>
	</humanitarian-scope>

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.

Changelog
~~~~~~~~~

2.02
^^^^
| The ``humanitarian-scope`` and ``narrative`` elements were introduced in 2.02.
