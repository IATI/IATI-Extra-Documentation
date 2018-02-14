Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``policy-marker`` element.

| The ``narrative`` element should be used only when the *99* (*Reporting Organisation*) *PolicyMarkerVocabulary* is declared.

.. code-block:: xml

	<policy-marker vocabulary="99" code="10" significance="3">
		<narrative>Policy Marker Text</narrative>
	</policy-marker>

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.

Changelog
~~~~~~~~~

2.01
^^^^
| The ``narrative`` element was introduced in 2.01.
