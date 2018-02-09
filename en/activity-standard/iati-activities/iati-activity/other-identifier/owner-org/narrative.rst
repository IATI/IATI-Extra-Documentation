Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``owner-org`` of an ``other-identifier``.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--other-identifier starts-->
	:end-before: <!--other-identifier ends-->

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.


Changelog
~~~~~~~~~

2.01
^^^^
| The ``owner-org`` element was added in version 2.01
