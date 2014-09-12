Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``policy-marker`` element.

| The ``narrative`` element should be used specially when the *99* (*Reporting Organisation*) vocabulary is declared.

.. code-block:: xml
	:emphasize-lines: 2
	
	<policy-marker vocabulary="99" code="10">
		<narrative>Policy Marker Text</narrative>
	</policy-marker>

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute.  Example not shown.
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
