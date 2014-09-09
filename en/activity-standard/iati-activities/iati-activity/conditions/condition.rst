Example Usage
~~~~~~~~~~~~~
Example ``condition`` attached, with ``ConditionType`` code *1* (*Policy*):

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 2
	
From version 1.04, the schema allows the ``xml:lang`` attribute to also be included in the sub-element ``condition``
|
| Example of an ``iati-activity`` with two ``conditions``, declared in the default language of *en*,  and also *fr*:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml	
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 2, 3, 4, 5

Changelog
~~~~~~~~~

1.04
^^^^

| It was always the intention of the standard that a condition could be specified in different languages but the schema has never allowed it.
| This has now been fixed.
