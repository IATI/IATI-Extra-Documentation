Example Usage
~~~~~~~~~~~~~
Example ``condition`` child element of ``conditions`` of an ``iati-activity``.

| The ``@type`` attribute declares a valid code (*1*) from the *ConditionType* codelist.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 2, 5

| The ``condition`` element can be repeated in any ``conditions`` of an ``iati-activity``.

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.

1.04
^^^^
| It was always the intention of the standard that a condition could be specified in different languages but the schema has never allowed it.
| This has now been fixed.
