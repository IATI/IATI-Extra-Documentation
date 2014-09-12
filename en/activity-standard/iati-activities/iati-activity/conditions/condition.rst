Example Usage
~~~~~~~~~~~~~
Example ``condition`` child element of ``conditions`` of an ``iati-activity``.

| This example declares ``ConditionType`` code *1* (*Policy*) with the ``type`` attribute

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 2, 5

| Note: multiple conditions are expressed by repeating the ``condition`` element.	

Changelog
~~~~~~~~~

1.04
^^^^

| It was always the intention of the standard that a condition could be specified in different languages but the schema has never allowed it.
| This has now been fixed.
