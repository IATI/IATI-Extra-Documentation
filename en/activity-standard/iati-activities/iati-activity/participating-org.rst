Example Usage
~~~~~~~~~~~~~
Example ``participating-org`` in an ``iati-activity``.

| An example organisation ``@ref`` of *BB-BBB-123456789* is declared.
| The ``@role`` attribute declares a valid code (*2*) from the *OrganisationRole* codelist.
| The ``@type`` attribute declares a valid code (*40*) from the *OrganisationType* codelist.
| The ``@activity-id`` attribute declares an IATI activity identifier.
| The ``@crs-channel-code`` attribute declares the CRS Channel Code for the participating organisation.

.. code-block:: xml
	:emphasize-lines: 1, 3

	<participating-org ref="BB-BBB-123456789" role="2" type="40" activity-id="BB-BBB-123456789-1234">
		<narrative>Name of Agency B</narrative>
	</participating-org>

As demonstrated in the the above example, it is strongly recommended that the name of the organisation is provided (using the narrative child element) in addition to a valid organisation identifier. Where an organisation identifier is not present the name (using the narrative child element) is mandatory.

| The ``participating-org`` element can be repeated in any ``iati-activity``.
| In this example, three ``participating-org`` are declared.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--participating-org starts-->
	:end-before: <!--participating-org ends-->
	:emphasize-lines: 1, 3, 4, 6, 7, 10

Changelog
~~~~~~~~~

2.03
^^^^
| The definition of the ``@ref`` attribute was `updated <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851>`__.
| The ``@crs-channel-code`` attribute was `added <https://discuss.iatistandard.org/t/crs-channels-of-delivery-included-2-03/857>`__.

2.02
^^^^
| The ``activity-id`` attribute was `added <http://support.iatistandard.org/entries/82377659-Add-activity-id-attribute-to-participating-org-element>`__.

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

| The ``OrganisationRole`` codelist was changed to numeric codes
