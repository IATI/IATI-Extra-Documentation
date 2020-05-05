2.01 Changelog
^^^^^^^^^^^^^^

Changes / additions to IATI Standard for version 2.01

Note: Version 2.01 was released on Tuesday 6 January 2015.

.. contents::

Schema Changes
==============

A full diff of all schema changes in 2.01 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Schemas/compare/version-1.05...version-2.01#files_bucket>`__

Activities schema
-----------------
*Activity Website: Removed Element*
```````````````````````````````````
Element: ``activity-website`` (`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - activity-website
     - (removed)

*Contact Info - Department: New Element*
````````````````````````````````````````
Element: :doc:`contact-info/department </activity-standard/iati-activities/iati-activity/contact-info/department>`
(`discussion <http://support.iatistandard.org/entries/44571616-Organisational-unit-within-contact-details>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - (none)
     - contact-info/department

*Description: Removed Attributes*
`````````````````````````````````
* Element: :doc:`country-budget-items/budget-item/description </activity-standard/iati-activities/iati-activity/country-budget-items/budget-item/description>`
* Element: :doc:`result/description </activity-standard/iati-activities/iati-activity/result/description/>`
* Element: :doc:`result/indicator/description </activity-standard/iati-activities/iati-activity/result/indicator/description/>`

(`discussion <http://support.iatistandard.org/entries/52106609-Version-2-01-Iteration-3-8-Miscellaneous>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#removal-of-the-type-attribute-on-some-description-elements>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - country-budget-items/budget-item/description/\@type
     - (removed)
   * - result/description/\@type
     - (removed)
   * - result/indicator/description/\@type
     - (removed)

*Document Link: Bug Fix*
````````````````````````
Inconsistencies in the document-link element were identified and applied, around the mandatory use of the language and title child elements.

* Element: :doc:`document-link </activity-standard/iati-activities/iati-activity/document-link>`
(`discussion <https://github.com/IATI/IATI-Schemas/pull/256>`__ )


*Freetext: Amended Elements*
````````````````````````````
The ability to add free text has been removed from the following elements:

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#descriptive-text-is-no-longer-allowed-on-data-specified-by-codes-with-some-exceptions>`__)

* Element: :doc:`activity-status </activity-standard/iati-activities/iati-activity/activity-status>`
* Element: :doc:`activity-scope </activity-standard/iati-activities/iati-activity/activity-scope>`
* Element: :doc:`collaboration-type </activity-standard/iati-activities/iati-activity/collaboration-type>`
* Element: :doc:`default-finance-type </activity-standard/iati-activities/iati-activity/default-finance-type>`
* Element: :doc:`default-flow-type </activity-standard/iati-activities/iati-activity/default-flow-type>`
* Element: :doc:`default-aid-type </activity-standard/iati-activities/iati-activity/default-aid-type>`
* Element: :doc:`default-tied-status </activity-standard/iati-activities/iati-activity/default-tied-status>`
* Element: :doc:`transaction/transaction-type </activity-standard/iati-activities/iati-activity/transaction/transaction-type>`
* Element: :doc:`transaction/flow-type </activity-standard/iati-activities/iati-activity/transaction/flow-type>`
* Element: :doc:`transaction/aid-type </activity-standard/iati-activities/iati-activity/transaction/aid-type>`
* Element: :doc:`transaction/finance-type </activity-standard/iati-activities/iati-activity/transaction/finance-type>`
* Element: :doc:`transaction/tied-status </activity-standard/iati-activities/iati-activity/transaction/tied-status>`
* Element: :doc:`transaction/disbursement-channel </activity-standard/iati-activities/iati-activity/transaction/disbursement-channel>`
* Element: :doc:`document-link/category </activity-standard/iati-activities/iati-activity/document-link/category>`
* Element: :doc:`document-link/language </activity-standard/iati-activities/iati-activity/document-link/language>`
* Element: :doc:`related-activity </activity-standard/iati-activities/iati-activity/related-activity>`
* Element: :doc:`crs-add/loan-terms/repayment-type </activity-standard/iati-activities/iati-activity/crs-add/loan-terms/repayment-type>`
* Element: :doc:`crs-add/loan-terms/repayment-plan </activity-standard/iati-activities/iati-activity/crs-add/loan-terms/repayment-plan>`
* Element: :doc:`location/exactness </activity-standard/iati-activities/iati-activity/location/exactness>`
* Element: :doc:`location/location-id </activity-standard/iati-activities/iati-activity/location/location-id>`
* Element: :doc:`location/administrative </activity-standard/iati-activities/iati-activity/location/administrative>`

*IATI Activity: Removed Attribute*
``````````````````````````````````
Element: :doc:`iati-activity </activity-standard/iati-activities/iati-activity/>` (`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-activity/\@version
     - (removed)

*Location: Removed Elements*
````````````````````````````
Element: :doc:`location </activity-standard/iati-activities/iati-activity/location>`
(`discussion <http://support.iatistandard.org/entries/51310806-Delete-don-t-just-deprecate-codes-in-2-01>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#location-changes>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - location/coordinates
     - (removed)
   * - location/gazetteer-entry
     - (removed)
   * - location/location-type
     - (removed)

*Location: Removed Attributes*
``````````````````````````````
Element: :doc:`location </activity-standard/iati-activities/iati-activity/location>`
(`discussion <http://support.iatistandard.org/entries/51310806-Delete-don-t-just-deprecate-codes-in-2-01>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#location-changes>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - location/\@percentage
     - (removed)
   * - location/administrative/\@country
     - (removed)
   * - location/administrative/\@adm1
     - (removed)
   * - location/administrative/\@adm2
     - (removed)

*Narrative: New Elements*
`````````````````````````
A ``narrative`` child element was added to the following elements, to enable the inclusion free text.

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: :doc:`reporting-org/narrative </activity-standard/iati-activities/iati-activity/reporting-org/narrative>`
* Element: :doc:`title/narrative </activity-standard/iati-activities/iati-activity/title/narrative>`
* Element: :doc:`description/narrative </activity-standard/iati-activities/iati-activity/description/narrative>`
* Element: :doc:`participating-org/narrative </activity-standard/iati-activities/iati-activity/participating-org/narrative>`
* Element: :doc:`activity-date/narrative </activity-standard/iati-activities/iati-activity/activity-date/narrative>`
* Element: :doc:`contact-info/organisation/narrative </activity-standard/iati-activities/iati-activity/contact-info/organisation/narrative>`
* Element: :doc:`contact-info/department/narrative </activity-standard/iati-activities/iati-activity/contact-info/department/narrative>`
* Element: :doc:`contact-info/person-name/narrative </activity-standard/iati-activities/iati-activity/contact-info/person-name/narrative>`
* Element: :doc:`contact-info/job-title/narrative </activity-standard/iati-activities/iati-activity/contact-info/job-title/narrative>`
* Element: :doc:`contact-info/mailing-address/narrative </activity-standard/iati-activities/iati-activity/contact-info/mailing-address/narrative>`
* Element: :doc:`recipient-country/narrative </activity-standard/iati-activities/iati-activity/recipient-country/narrative>`
* Element: :doc:`recipient-region/narrative </activity-standard/iati-activities/iati-activity/recipient-region/narrative>`
* Element: :doc:`location/name/narrative </activity-standard/iati-activities/iati-activity/location/name/narrative>`
* Element: :doc:`location/description/narrative </activity-standard/iati-activities/iati-activity/location/description/narrative>`
* Element: :doc:`location/activity-description/narrative </activity-standard/iati-activities/iati-activity/location/activity-description/narrative>`
* Element: :doc:`sector/narrative </activity-standard/iati-activities/iati-activity/sector/narrative>`
* Element: :doc:`country-budget-items/budget-item/description/narrative </activity-standard/iati-activities/iati-activity/country-budget-items/budget-item/description/narrative>`
* Element: :doc:`policy-marker/narrative </activity-standard/iati-activities/iati-activity/policy-marker/narrative>`
* Element: :doc:`transaction/description/narrative </activity-standard/iati-activities/iati-activity/transaction/description/narrative>`
* Element: :doc:`transaction/sector/narrative </activity-standard/iati-activities/iati-activity/transaction/sector/narrative>`
* Element: :doc:`transaction/recipient-country/narrative </activity-standard/iati-activities/iati-activity/transaction/recipient-country/narrative>`
* Element: :doc:`transaction/recipient-region/narrative </activity-standard/iati-activities/iati-activity/transaction/recipient-region/narrative>`
* Element: :doc:`document-link/title/narrative </activity-standard/iati-activities/iati-activity/document-link/title/narrative>`
* Element: :doc:`conditions/condition/narrative </activity-standard/iati-activities/iati-activity/conditions/condition/narrative>`
* Element: :doc:`result/title/narrative </activity-standard/iati-activities/iati-activity/result/title/narrative>`
* Element: :doc:`result/description/narrative </activity-standard/iati-activities/iati-activity/result/description/narrative>`
* Element: :doc:`result/indicator/title/narrative </activity-standard/iati-activities/iati-activity/result/indicator/title/narrative>`
* Element: :doc:`result/indicator/description/narrative </activity-standard/iati-activities/iati-activity/result/indicator/description/narrative>`
* Element: :doc:`result/indicator/baseline/comment/narrative </activity-standard/iati-activities/iati-activity/result/indicator/baseline/comment/narrative>`
* Element: :doc:`result/indicator/period/target/comment/narrative </activity-standard/iati-activities/iati-activity/result/indicator/period/target/comment/narrative>`
* Element: :doc:`result/indicator/period/actual/comment/narrative </activity-standard/iati-activities/iati-activity/result/indicator/period/actual/comment/narrative>`

*Other Flags: Renamed Element*
``````````````````````````````
The ``aid-type-flag`` element has been renamed to ``other-flags``.

Element: :doc:`crs-add/other-flags </activity-standard/iati-activities/iati-activity/crs-add/other-flags>`
(`discussion <http://support.iatistandard.org/entries/29705458-Confusion-Between-Aid-Type-Flag-Type-of-Aid->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - aid-type-flag
     - other-flags

*Other Identifier: New Child Elements*
``````````````````````````````````````
The following elements were added to the ``other-identifier`` element:

(`discussion <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-2-3-7-Replicate-more-activity-level-elements-at-transaction-level->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-transactions-sector-recipient-country-recipient-region>`__)

* Element: :doc:`other-identifier/owner-org </activity-standard/iati-activities/iati-activity/other-identifier/owner-org>`
* Element: :doc:`other-identifier/owner-org/narrative </activity-standard/iati-activities/iati-activity/other-identifier/owner-org/narrative>`

*Other Identifier: Removed / New Attributes*
````````````````````````````````````````````
Element: :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier>`
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - other-identifier/\@owner-name
     - (removed)
   * - other-identifier/\@owner-ref
     - (removed)
   * - (none)
     - other-identifier/\@ref
   * - (none)
     - other-identifier/\@type

*Planned Disbursement: Removed/Renamed Attributes*
``````````````````````````````````````````````````
Element: :doc:`planned-disbursement </activity-standard/iati-activities/iati-activity/planned-disbursement>`
(`discussion <http://support.iatistandard.org/entries/77495498-Align-planned-disbursement-with-budget>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#changes-to-the-planned-disbursement-element-planned-disbursement>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - (none)
     - planned-disbursement/\@type
   * - planned-disbursement/\@last-updated
     - (removed)

*Transaction: New Child Elements*
`````````````````````````````````
The following elements were added to the ``transaction`` element:

(`discussion <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-2-3-7-Replicate-more-activity-level-elements-at-transaction-level->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-transactions-sector-recipient-country-recipient-region>`__)

* Element: :doc:`transaction/sector </activity-standard/iati-activities/iati-activity/transaction/sector>`
* Element: :doc:`transaction/recipient-country </activity-standard/iati-activities/iati-activity/transaction/recipient-country>`
* Element: :doc:`transaction/recipient-region </activity-standard/iati-activities/iati-activity/transaction/recipient-region>`


Organisations schema
--------------------

*Budget Line: New Element*
``````````````````````````
A new ``budget-line`` element was added to the following elements.

(`discussion <http://support.iatistandard.org/entries/77259793-Org-Create-budget-line-element>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: :doc:`total-budget/budget-line </organisation-standard/iati-organisations/iati-organisation/total-budget/budget-line>`
* Element: :doc:`recipient-org-budget/budget-line </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/budget-line>`
* Element: :doc:`recipient-country-budget/budget-line </organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/budget-line>`

*Document Link: Bug Fix*
````````````````````````
Inconsistencies in the document-link element were identified and applied, around the mandatory use of the language and title child elements.

* Element: :doc:`document-link </organisation-standard/iati-organisations/iati-organisation/document-link>`
(`discussion <https://github.com/IATI/IATI-Schemas/pull/256>`__ )

*Document Link: New Child Element*
``````````````````````````````````
The ``recipient-country`` child element was added to the ``iati-organisation/document-link`` element:

Element: :doc:`document-link/recipient-country/narrative </organisation-standard/iati-organisations/iati-organisation/document-link/recipient-country/narrative>` (`discussion <http://support.iatistandard.org/entries/78420356-Org-Add-recipient-country-to-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#additional-elements-in-organisation-documents-document-link>`__)

*Freetext: Amended Elements*
````````````````````````````
The ability to add free text has been removed from the following element:

(`discussion <http://support.iatistandard.org/entries/41585166-General-Standardise-multi-lingual-text-fields>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#descriptive-text-is-no-longer-allowed-on-data-specified-by-codes-with-some-exceptions>`__)

* Element: :doc:`document-category </organisation-standard/iati-organisations/iati-organisation/document-category>`

*IATI Identifier: Renamed Element*
``````````````````````````````````
The ``iati-organisation/iati-identifier`` element has been renamed to ``iati-organisation/organisation-identifier``.

Element: :doc:`iati-organisation/organisation-identifier </organisation-standard/iati-organisations/ iati-organisation/organisation-identifier>`
(`discussion <http://support.iatistandard.org/entries/78421626-Org-Replace-iati-identifier-with-organisation>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-organisation/iati-identifier
     - iati-organisation/organisation-identifier

*Narrative: New Elements*
`````````````````````````
A ``narrative`` child element was added to the following elements, to enable the inclusion free text.

(`discussion <http://support.iatistandard.org/entries/44571616-Organisational-unit-within-contact-details>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#new-elements>`__)

* Element: :doc:`reporting-org/narrative </organisation-standard/iati-organisations/iati-organisation/reporting-org/narrative>`
* Element: :doc:`name/narrative </organisation-standard/iati-organisations/iati-organisation/name/narrative>`
* Element: :doc:`document-link/title/narrative </organisation-standard/iati-organisations/iati-organisation/document-link/title/narrative>`
* Element: :doc:`document-link/recipient-country/narrative </organisation-standard/iati-organisations/iati-organisation/document-link/recipient-country/narrative>`
* Element: :doc:`recipient-country-budget/recipient-country/narrative </organisation-standard/iati-organisations/iati-organisation/recipient-country-budget/recipient-country/narrative>`
* Element: :doc:`recipient-org-budget/recipient-org/narrative </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/recipient-org/narrative>`

*IATI Organisation: Removed Attribute*
``````````````````````````````````````
Element: :doc:`iati-organisation </organisation-standard/iati-organisations/iati-organisation/>` (`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 20 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - iati-organisation/\@version
     - (removed)

Common schema
-------------
Many substantial changes were made in 2.01. Both the organisation and activity schema draw on the common schema for
common definitions of elements and types. The changes in the common schema are reflected in the sections above, so are
not given in detail here. For further information see the CHANGES.txt file that can be found with the
:doc:`schema <schema>`

XML supplementary schema
------------------------
No substantial changes were made in 2.01, aside from essential version references.

Registry record schema
----------------------
No substantial changes were made in 2.01, aside from essential version references.

Codelist Changes
================

New Codelists
-------------

*IATI Organisation Identifier: New codelist*
````````````````````````````````````````````
The *IATIOrganisationIdentifier* codelist has been created.

Codelist: :doc:`IATIOrganisationIdentifier </codelists/IATIOrganisationIdentifier>`
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__)

*Other Identifier Type: New Codelist*
`````````````````````````````````````
Codelist: :doc:`OtherIdentifierType </codelists/OtherIdentifierType>`
(`discussion <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#update-to-other-identifier-adding-type-changing-definition-new-codelist>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - A1
     - Reporting Organisation’s internal activity identifier
     - (none)
   * - A2
     - CRS Activity identifier
     - (none)
   * - A3
     - Previous Activity Identifier
     - The standard insists that once an activity has been reported to IATI its identifier MUST NOT be changed, even if the reporting organisation changes its organisation identifier. There may be exceptional circumstances in which this rule cannot be followed, in which case the previous identifier should be reported using this code.
   * - A9
     - Other Activity Identifier
     - (none)
   * - B1
     - Previous Reporting Organisation Identifier
     - (none)
   * - B9
     - Other Organisation Identifier
     - (none)

*Policy Marker Vocabulary: New codelist*
````````````````````````````````````````
The *PolicyMarkerVocabulary* has been created, split from the deleted *Vocabulary* codelist.

Codelist: :doc:`SectorVocabulary </codelists/PolicyMarkerVocabulary>`
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)

*Sector Vocabulary: New codelist*
`````````````````````````````````
The *SectorVocabulary* has been created, split from the deleted *Vocabulary* codelist.

Codelist: :doc:`SectorVocabulary </codelists/SectorVocabulary>`
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)

*Version: New Codelist*
```````````````````````
Codelist: :doc:`Version </codelists/Version>`
(`discussion <http://support.iatistandard.org/entries/57866638-Tightening-up-on-version>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#declaring-the-version-of-the-iati-standard-being-used>`__)

.. list-table::
   :widths: 15 10 10 20
   :header-rows: 1

   * - Code
     - Name
     - Description
     - URL
   * - 1.01
     - (none)
     - (none)
     - http://iatistandard.org/101/
   * - 1.02
     - CRS Activity identifier
     - (none)
     - http://iatistandard.org/102/
   * - 1.03
     - (none)
     - (none)
     - http://iatistandard.org/103/
   * - 1.04
     - (none)
     - (none)
     - http://iatistandard.org/104/
   * - 1.05
     - (none)
     - (none)
     - http://iatistandard.org/105/
   * - 2.01
     - (none)
     - (none)
     -  http://iatistandard.org/201/


Embedded codelist updates
-------------------------

*Aid Type Flag: Renamed codelist*
`````````````````````````````````
The *AidTypeFlag* codelist has been renamed to *CRSAddOtherFlags*.

Codelist: :doc:`CRSAddOtherFlags </codelists/CRSAddOtherFlags>`
(`discussion <http://support.iatistandard.org/entries/29705458-Confusion-Between-Aid-Type-Flag-Type-of-Aid->`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#renamed-moved-and-removed-elements>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - AidTypeFlag
     - CRSAddOtherFlags

*Activity Date Type: Amended codes*
```````````````````````````````````
Codelist: :doc:`ActivityDateType Type </codelists/ActivityDateType>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - start-planned
     - 1
   * - start-actual
     - 2
   * - end-planned
     - 3
   * - end-actual
     - 4

*Document Category: New codes*
``````````````````````````````
Codelist: :doc:`DocumentCategory </codelists/DocumentCategory>`
(`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/l#new-codes-for-embedded-codelists>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - A12
     - Activity web page
     - (none)
   * - B16
     - Organisation web page
     - (none)
   * - B17
     - Country/Region web page
     - (none)
   * - B18
     - Sector web page
     - (none)

*Gazetteer Agency: Amended codes*
`````````````````````````````````
Codelist: :doc:`GazetteerAgency </codelists/GazetteerAgency>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - GEO
     - 1
   * - NGA
     - 2
   * - OSM
     - 3

*Organisation Role: Amended codes*
``````````````````````````````````
Codelist: :doc:`OrganisationRole </codelists/OrganisationRole>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - Funding
     - 1
   * - Accountable
     - 2
   * - Extending
     - 3
   * - Implementing
     - 4

*Policy Marker Vocabulary (was Vocabulary): Amended codes*
``````````````````````````````````````````````````````````
Codelist: :doc:`PolicyMarkerVocabulary </codelists/PolicyMarkerVocabulary>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - DAC
     - 1
   * - RO
     - 99

*Related Activity Type: New code*
`````````````````````````````````
Codelist: :doc:`RelatedActivityType </codelists/RelatedActivityType>`
(`discussion <http://support.iatistandard.org/entries/76684383-Redefine-activity-website-as-a-document-link>`__ | `guidance <http://support.iatistandard.org/entries/76862583-Referencing-another-publisher-s-report-of-the-same-activity>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 5
     - Third Party
     - A report by another organisation on the same activity (excluding activities reported as part of financial transactions - eg. provider-activity-id - or a co-funded activity using code = 4)


*Sector Vocabulary (was Vocabulary): Amended codes*
```````````````````````````````````````````````````
Codelist: :doc:`SectorVocabulary </codelists/SectorVocabulary>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - ADT
     - 1
   * - COFOG
     - 2
   * - DAC
     - 3
   * - DAC-3
     - 4
   * - ISO
     - 5
   * - NACE
     - 6
   * - NTEE
     - 7
   * - WB
     - 8
   * - RO
     - 99

*Transaction Type: Amended codes*
`````````````````````````````````
Codelist: :doc:`TransactionType </codelists/TransactionType>`
(`discussion <http://support.iatistandard.org/entries/41042407-Modify-code-list-activity-date-type-Language-neutral-conversion>`__ | `guidance <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__)

.. list-table::
   :widths: 15 20
   :header-rows: 1

   * - 1.0x
     - 2.01
   * - IF
     - 1
   * - C
     - 2
   * - D
     - 3
   * - E
     - 4
   * - IR
     - 5
   * - LR
     - 6
   * - R
     - 7
   * - QP
     - 8
   * - Q3
     - 9
   * - CG
     - 10

*Vocabulary: Removed / split codelist*
``````````````````````````````````````
The *Vocabulary* has been removed, and split into two new codelists: *SectorVocabulary* and *PolicyMarkerVocabulary*.

Codelist: :doc:`SectorVocabulary </codelists/SectorVocabulary>` | :doc:`SectorVocabulary </codelists/PolicyMarkerVocabulary>`
(`discussion <http://support.iatistandard.org/entries/78019646-Separate-vocabulary-codelists>`__)
