Example Usage
~~~~~~~~~~~~~
The ``narrative`` element can be used to declare freetext for the ``description`` child element of ``location``.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location-single starts-->
	:end-before: <!--location-single ends-->
	:emphasize-lines: 8

| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute.  Example not shown.
