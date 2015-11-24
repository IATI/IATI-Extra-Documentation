Example Usage
~~~~~~~~~~~~~
Example ``participating-org`` in an ``iati-activity``.

| An example organisation ``@ref`` of *BB-BBB-123456789* is declared.
| The ``@role`` attribute declares a valid code (*2*) from the *OrganisationRole* codelist.
| The ``@type`` attribute declares a valid code (*40*) from the *OrganisationType* codelist.
| The ``@activity-id`` attribute declares an IATI activity identifier.

.. code-block:: xml
	:emphasize-lines: 1, 3
	
	<participating-org ref="BB-BBB-123456789" role="2" type="40" activity-id="BB-BBB-123456789-1234">
		<narrative>Name of Agency B</narrative>
	</participating-org>
	
| The ``participating-org`` element can be repeated in any ``iati-activity``.
| In this example, three ``participating-org`` are declared.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--participating-org starts-->
	:end-before: <!--participating-org ends-->
	:emphasize-lines: 1, 3, 4, 6, 7, 10		

Changelog
~~~~~~~~~

2.02
^^^^
| The ``activity-id`` attribute was `added <http://support.iatistandard.org/entries/82377659-Add-activity-id-attribute-to-participating-org-element>`__.


2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

| The ``OrganisationRole`` codelist was changed to numeric codes
