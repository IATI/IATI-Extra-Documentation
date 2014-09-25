Example Usage
~~~~~~~~~~~~~
Example ``organisation`` within ``contact-info`` of an ``iati-activity``

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--contact-info starts-->
	:end-before: <!--contact-info ends-->
	:emphasize-lines: 2, 4

Changelog
~~~~~~~~~

2.01
^^^^
| Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
