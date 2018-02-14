Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``receiver-org`` element of a ``planned-disbursement``.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute.  Example not shown.


Changelog
~~~~~~~~~

2.02
^^^^
Added the optional ``receiver-org`` element, including the ``narrative`` element.
