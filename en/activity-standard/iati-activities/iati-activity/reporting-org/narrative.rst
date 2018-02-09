Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``reporting-org`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--reporting-org starts-->
	:end-before: <!--reporting-org ends-->

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--reporting-org starts-->
	:end-before: <!--reporting-org ends-->

Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
