Example Usage
~~~~~~~~~~~~~
Example ``title`` for an ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--title starts-->
	:end-before: <!--title ends-->
	:emphasize-lines: 1, 5	
	  
Changelog
~~~~~~~~~
2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

