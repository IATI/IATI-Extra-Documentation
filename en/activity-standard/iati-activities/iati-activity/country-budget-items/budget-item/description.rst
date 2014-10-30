Example Usage
~~~~~~~~~~~~~
Example usage of ``description`` of ``budget-item`` element, a child element of ``country-budget-items``.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--country-budget-items starts-->
	:end-before: <!--country-budget-items ends-->
	:emphasize-lines: 3, 5, 8, 10
	
Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element, but only in particular use-cases.

| The @type attribute was `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#description-removed-attributes>`__.

