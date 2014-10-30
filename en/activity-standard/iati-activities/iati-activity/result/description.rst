Example Usage
~~~~~~~~~~~~~
Example usage of ``description`` in a ``result`` of an ``iati-activity``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 5, 7

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

| The @type attribute was `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#description-removed-attributes>`__.
