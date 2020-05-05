2.02 Changelog
^^^^^^^^^^^^^^

Changes / additions to IATI Standard for version 2.02

Note: Version 2.02 was released on Monday 7th December 2015.

.. contents::

.. _2_02_schema_changes:

Schema Changes
==============

A full diff of all schema changes in 2.02 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Schemas/compare/version-2.01...version-2.02#files_bucket>`__


Activities schema
-----------------

Addition of @humanitarian attribute within the `iati-activity <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/>`__ element. (`Discussion <http://support.iatistandard.org/entries/106937796-Humanitarian-Flag>`__)

Addition of @activity-id attribute within the `participating-org <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/participating-org/>`__ element. (`Discussion <http://support.iatistandard.org/entries/82377659-Add-activity-id-attribute-to-participating-org-element>`__)

Addition of @vocabulary-uri attribute within the `recipient-region <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/recipient-region/>`__ element. (`Discussion <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__)

Addition of @vocabulary-uri attribute within the `sector <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/sector/>`__ element. (`Discussion <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__)

The element `humanitarian-scope <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/humanitarian-scope/>`__ was added (`Discussion <http://support.iatistandard.org/entries/105778163-Humanitarian-Emergencies-and-Appeals>`__)

Addition of @vocabulary-uri attribute within the `policy-marker <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/policy-marker/>`__ element. (`Discussion <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__)

The occurrence rule for the @significance attribute within the `policy-marker <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/policy-marker/>`__ element was amended. (`Discussion <http://support.iatistandard.org/entries/105777943-Humanitarian-Policy-Markers>`__)

Addition of @status attribute within the `budget <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/budget/>`__ element. (`Discussion <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__)

The element `provider-org <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/provider-org/>`__ (a sub-element of `planned-disbursement <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/>`__) was added (`Discussion <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__)

The element `receiver-org <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/receiver-org/>`__ (a sub-element of `planned-disbursement <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/>`__) was added (`Discussion <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__)

The definition for the element `period-start <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/period-start/>`__ (a sub-element of `planned-disbursement <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/>`__) was amended (`Discussion <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__)

The definition for the element `period-end <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/period-end/>`__ (a sub-element of `planned-disbursement <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/planned-disbursement/>`__) was amended (`Discussion <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__)

Addition of @humanitarian attribute within the `transaction <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/>`__ element. (`Discussion <http://support.iatistandard.org/entries/106937796-Humanitarian-Flag>`__)

Addition of @type attribute within the `provider-org <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/provider-org>`__ element (itself a sub-element of `transaction <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/>`__). (`Discussion <http://support.iatistandard.org/entries/81683876-provider-receiver-og-adding-type>`__)

Addition of @type attribute within the `receiver-org <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/receiver-org>`__ element (itself a sub-element of `transaction <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/>`__). (`Discussion <http://support.iatistandard.org/entries/81683876-provider-receiver-og-adding-type>`__)

Addition of @vocabulary-uri attribute within the `transaction/sector <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/sector/>`__ element. (`Discussion <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__)

Addition of @vocabulary-uri attribute within the `transaction/region <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/transaction/region/>`__ element. (`Discussion <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__)

The element `document-date <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/document-link/document-date>`__ (a sub-element of `document-link <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/document-link/>`__) was added (`Discussion <http://support.iatistandard.org/entries/92707776-Document-Dates>`__)

The element `reference <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/reference/>`__ (a sub-element of `result/indicator <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/>`__) was added (`Discussion <http://support.iatistandard.org/entries/79784435-Results-Require-unambiguous-indicator-reference>`__)

The element `location <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/target/location>`__ (a sub-element of `result/indicator/period/target/ <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/target/>`__) was added (`Discussion <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__)

The element `dimension <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/target/dimension>`__ (a sub-element of `result/indicator/period/target/ <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/target/>`__) was added (`Discussion <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__)

The element `location <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/location>`__ (a sub-element of `result/indicator/period/actual/ <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/>`__) was added (`Discussion <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__)

The element `dimension <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/dimension>`__ (a sub-element of `result/indicator/period/actual/ <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/result/indicator/period/actual/>`__) was added (`Discussion <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__)

The element `channel-code <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/crs-add/channel-code/>`__ a sub-element of `crs-add/ <http://iatistandard.org/202/activity-standard/iati-activities/iati-activity/crs-add/>`__) was added (`Discussion <http://support.iatistandard.org/entries/83678719-DAC-Channel-of-Delivery>`__)


Organisation schema
-------------------

Addition of @status attribute within the `total-budget <http://iatistandard.org/202/organisation-standard/iati-organisations/iati-organisation/total-budget/>`__ element. (`Discussion <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__)

Addition of @status attribute within the `recipient-org-budget <http://iatistandard.org/202/organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/>`__ element. (`Discussion <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__)

The element `recipient-region-budget <http://iatistandard.org/202/organisation-standard/iati-organisations/iati-organisation/recipient-region-budget/>`__ was added (`Discussion <http://support.iatistandard.org/entries/79323113-Org-Standard-recipient-region-budget>`__)

The element `total-expenditure <http://iatistandard.org/202/organisation-standard/iati-organisations/iati-organisation/total-expenditure/>`__ was added (`Discussion <http://support.iatistandard.org/entries/83404469-Add-Total-Expenditure-Element-To-Organisation-File>`__)

The element `document-date <http://iatistandard.org/202/organisation-standard/iati-organisations/iati-organisation/document-link/document-date>`__ (a sub-element of `document-link <h/organisation-standard/iati-organisations/iati-organisation/document-link/>`__) was added (`Discussion <http://support.iatistandard.org/entries/92707776-Document-Dates>`__)



.. _2_02_documentation_changes:

Documentation Changes
=====================

New overview pages
------------------

The following overview pages have been added:

- :doc:`/activity-standard/overview/humanitarian-reporting`
- :doc:`/activity-standard/overview/self-defined-vocabularies`


Amended and new documentation elsewhere on the reference site
-------------------------------------------------------------

A full diff of all documentation changes in 2.02 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Extra-Documentation/compare/version-2.01...version-2.02#files_bucket>`__


.. _2_02_codelist_changes:

Codelist Changes
================

A full diff of all **embedded** codelist changes in 2.02 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Codelists/compare/version-2.01...version-2.02#files_bucket>`__

Codelist schema
---------------

Within the raw codelist XML definitions, each ``codelist-item`` now supports the addition of ``status``, ``activation-date`` and ``withdrawal-date`` attributes. (`Discussion <http://support.iatistandard.org/entries/106345386-Add-a-withdrawn-flag-to-code-names-to-indicate-deprecation>`__)

New Codelists
-------------

Embedded:

- :doc:`/codelists/BudgetStatus` (`Discussion <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__)


Non-Embedded:

- :doc:`/codelists/HumanitarianScopeType` (`Discussion <http://support.iatistandard.org/entries/105778163-Humanitarian-Emergencies-and-Appeals>`__)
- :doc:`/codelists/HumanitarianScopeVocabulary` (`Discussion <http://support.iatistandard.org/entries/105778163-Humanitarian-Emergencies-and-Appeals>`__)
- :doc:`/codelists/IndicatorVocabulary` (`Discussion <http://support.iatistandard.org/entries/79784435-Results-Require-unambiguous-indicator-reference>`__)
- :doc:`/codelists/CRSChannelCode` (`Discussion <http://support.iatistandard.org/entries/83678719-DAC-Channel-of-Delivery>`__)


Updated Codelists
-----------------

Embedded:

- Added code 11 (Incoming Commitments) to :doc:`/codelists/TransactionType` (`discussion <http://support.iatistandard.org/entries/82769745-Add-Incoming-Commitment-to-the-Transaction-Type-codelist>`__)
- Added code 99 (Reporting Organisation) to :doc:`/codelists/RegionVocabulary` (`discussion <http://support.iatistandard.org/entries/82936169-Allow-Organisations-To-Use-Their-Own-Internally-Defined-Regions->`__)
- Added codes 7 (SDG Goal), 8 (SDG Target), 9 (SDG Indicator), 10 (Humanitarian Global Clusters  (Inter-Agency Standing Committee)) to :doc:`/codelists/SectorVocabulary` (discussion `post 1 <http://support.iatistandard.org/entries/105792233-Make-sector-vocabulary-codelist-SDG-ready->`__ and `post 2  <http://support.iatistandard.org/entries/106937886-Humanitarian-Clusters>`__)


Non-Embedded:

- Added code '2.02' to :doc:`/codelists/Version`
