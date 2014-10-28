Example Usage
~~~~~~~~~~~~~
Example ``person-name`` within ``contact-info`` of an ``iati-activity``

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--contact-info starts-->
	:end-before: <!--contact-info ends-->
	:emphasize-lines: 8, 10

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.
