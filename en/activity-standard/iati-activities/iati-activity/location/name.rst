Example Usage
~~~~~~~~~~~~~
Example usage of ``name`` within a ``location`` of an ``iati-activity``.:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 4, 6
	
Changelog
~~~~~~~~~

2.01
^^^^
| Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
