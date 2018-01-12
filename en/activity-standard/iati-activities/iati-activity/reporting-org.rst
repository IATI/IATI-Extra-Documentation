Example Usage
~~~~~~~~~~~~~
Example ``reporting-org`` for an ``iati-activity``

| An example organisation ``@ref`` of *AA-AAA-123456789* is declared.
| The ``@type`` attribute declares a valid code (*40*) from the *OrganisationType* codelist.
| The optional ``@secondary-reporter`` boolean is included, for illustration.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--reporting-org starts-->
	:end-before: <!--reporting-org ends-->
	:emphasize-lines: 1, 4


Changelog
~~~~~~~~~

2.03
^^^^
| The definition of the ``@ref`` attributed was `updated <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851/>`__.
| The definition of the ``@secondary-reporter`` attributed was `updated <https://discuss.iatistandard.org/t/modify-definition-of-secondary-publisher-included-2-03/846>`__.

2.01
^^^^
| Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

1.04
^^^^
| The ``@secondary-reporter`` was introduced in 1.04.
