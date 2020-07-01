Example Usage
~~~~~~~~~~~~~
Example of ``name`` of an ``iati-organisation``.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--name starts-->
	:end-before: <!--name ends-->
	:emphasize-lines: 1, 4

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

.. meta::
  :order: 1
