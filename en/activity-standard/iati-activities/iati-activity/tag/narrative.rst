Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``tag`` parent element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--tag starts-->
	:end-before: <!--tag ends-->
	:emphasize-lines: 2, 5

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute:


Changelog
~~~~~~~~~

2.03
^^^^
| The optional ``narrative`` element within a ``tag`` element  was `added <https://discuss.iatistandard.org/t/non-statistical-secondary-sectors-excluded-2-03/849>`__.
