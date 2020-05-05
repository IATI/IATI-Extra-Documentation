1.05 Changelog
^^^^^^^^^^^^^^

Changes / Additions to IATI Standard for version 1.05

.. contents::

Schema Changes
==============
A full diff of all schema changes in 1.05 can be found in the `IATI GitHub <https://github.com/IATI/IATI-Schemas/compare/version-1.04...version-1.05#files_bucket>`__

.. _1_05_activities_schema_changes:

Activities schema
-----------------

*Location/Location ID: Updated description text*
````````````````````````````````````````````````
Element: :doc:`location/location-id </activity-standard/iati-activities/iati-activity/location/location-id>` (`discussion  <http://support.iatistandard.org/entries/50424779-Add-a-description-in-the-schema-to-planned-disbursement-element>`__)


*Planned Disbursement: Updated description text*
````````````````````````````````````````````````
Element: :doc:`planned-disbursement </activity-standard/iati-activities/iati-activity/planned-disbursement>` (`discussion  <https://github.com/IATI/IATI-Extra-Documentation/issues/205>`__)

In 1.04:
 
.. list-table::
   :widths: 15 30
   :header-rows: 1

   * - Element
     - Description
   * - location/location-id
     - For administrative areas this identifier should only be used if the location being defined is the administrative area itself. For describing the administrative area/s within which a location falls the location/administrative element should be used.

Description amended in 1.05:

.. list-table:: 
   :widths: 20 40
   :header-rows: 1

   * - Element
     - Description
   * - location/location-id
     - A unique code describing the location according to a recognised gazetteer or administrative boundary repository. Administrative areas should only be reported here if the location being defined is the administrative area itself. For describing the administrative area/s within which a more specific location falls the location/administrative element should be used.

Organisations schema
--------------------
No substantial changes were made in 1.05, aside from essential version references.

Common schema
-------------
No substantial changes were made in 1.05, aside from essential version references.

XML supplementary schema
------------------------
No substantial changes were made in 1.05, aside from essential version references.

Registry record schema
----------------------
No substantial changes were made in 1.05, aside from essential version references.


Codelist Changes
================

New Codelists
-------------
No new codelists were added in 1.05


Embedded codelist updates
-------------------------

*Activity Status: New code*
```````````````````````````
Codelist: :doc:`Activity Status </codelists/ActivityStatus>` 
(`discussion <http://support.iatistandard.org/entries/43247528-Activity-Status-Suspended->`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 6
     - Suspended
     - (none)

*Description Type: New code*
````````````````````````````
Codelist: :doc:`DescriptionType </codelists/DescriptionType>` 
(`discussion <http://support.iatistandard.org/entries/22922878-Description-type-extend-the-codelist>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 4
     - Other
     - For miscellaneous use. A further classification or breakdown may be included in the narrative.

*Document Category: New codes*
``````````````````````````````
Codelist:  :doc:`DocumentCategory </codelists/DocumentCategory>` 
(`discussion <http://support.iatistandard.org/entries/86661313-Document-Types->`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - B11
     - Sector strategy
     - (none)
   * - B12
     - Thematic strategy
     - (none)
   * - B13
     - Country-level Memorandum of Understanding
     - (none)
   * - B14
     - Evaluations policy
     - (none)
   * - B15
     - General Terms and Conditions
     - (none)     

*Related Activity Type: New code*
`````````````````````````````````  
Codelist: :doc:`RelatedActivityType </codelists/RelatedActivityType>` 
(`discussion <http://support.iatistandard.org/entries/54201556-related-activity-new-code>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 5
     - Third Party
     - A report by another organisation on the same activity (excluding activities reported as part of financial transactions - eg. provider-activity-id - or a co-funded activity using code = 4).

*Related Activity Type: Amended code*
`````````````````````````````````````
Codelist: :doc:`RelatedActivityType </codelists/RelatedActivityType>` 
(`discussion <http://support.iatistandard.org/entries/54201556-related-activity-new-code>`__)

In 1.04:

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 4
     - Multifunded
     - A multifunded, or co-funded activity. The identifier should be globally unique and shared by all reporters of this activity.

Name and description changed in 1.05:

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 4
     - Co-funded
     - An activity that receives funding from more than one organisation.

*Transaction Type: Amended code*
````````````````````````````````
Codelist: :doc:`TransactionType </codelists/TransactionType>` 
(`discussion <http://support.iatistandard.org/entries/50777388-Description-For-Transcation-Type-Incoming-Funds-Is-Incorrect>`__)

In 1.04:

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - IF
     - Incoming Funds
     - Funds received from an external funding source (eg a donor).
     
Description changed in 1.05:

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - IF
     - Incoming Funds
     - Funds received (whether from an external source or through internal accounting) for specific use on this activity.
               
*Vocabulary: New code*
``````````````````````
Codelist: :doc:`Vocabulary </codelists/Vocabulary>` 
(`discussion <http://support.iatistandard.org/entries/22916773>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - RO2
     - Reporting Organisation (2)	
     - Where reporting organisations have more than one vocabulary that they wish to reference.
     
     
*Policy Marker: New code*
`````````````````````````
Codelist: :doc:`PolicyMarker </codelists/PolicyMarker>` (`discussion <http://support.iatistandard.org/entries/52320903-New-Policy-Markers-Significance-Codes>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 9
     - Reproductive, Maternal, Newborn and Child Health (RMNCH)
     - (none)

Non-embedded codelist updates
-----------------------------

*Policy Significance: New code*
```````````````````````````````
Codelist: :doc:`PolicySignificance </codelists/PolicySignificance>` (`discussion <http://support.iatistandard.org/entries/52320903-New-Policy-Markers-Significance-Codes>`__)

.. list-table::
   :widths: 15 20 30
   :header-rows: 1

   * - Code
     - Name
     - Description
   * - 4
     - Explicit primary objective
     - (none)

As part of this process, the `non-embedded codelist changelog <upgrades/nonembedded-codelist-changelog>`__ was also updated

Documentation Changes
=====================

Overview pages
--------------

*Activity Standard - Dates Overview*
````````````````````````````````````
Overview page: :doc:`Activity Standard - Dates Overview </activity-standard/overview/dates/>` (`discussion <http://support.iatistandard.org/entries/43247528-Activity-Status-Suspended->`__)

.. list-table::
   :widths: 20 40
   :header-rows: 1

   * - Page
     - Additional guidance 
   * - Activity Standard - Dates Overview.	 
     - ActivityStatus code 6 indicates a temporary suspension of an activity. In this state an activity is assumed not to be current, but future, forward-looking budgets are still assumed to be applicable.
     
*Activity Standard - Classifications Overview*
``````````````````````````````````````````````    
Overview page: :doc:`Activity Standard - Classifications Overview </activity-standard/overview/classifications/>` (`discussion <http://support.iatistandard.org/entries/55170393-Tied-and-partially-tied-values>`__) (`discussion <http://support.iatistandard.org/entries/52320903-New-Policy-Markers-Significance-Codes>`__)

.. list-table::
   :widths: 20 40
   :header-rows: 1

   * - Page
     - Additional guidance 
   * - Activity Standard - Classifications Overview	 
     - If an activity is either wholly "tied" or "untied" it is recommended that the appropriate ``default-tied-status`` code is used / If an activity is "partially tied" it is recommended that the reported commitment/s are split into "tied" and "untied" amounts and ``tied-status`` is reported at ``transaction`` level. (NB that tied status should be reported for commitments only.)
   * - Activity Standard - Classifications Overview	 
     - Activity Standard - Classifications Overview  When using ``policy-marker`` and the ``Policy Significance`` code *4* (Explicit primary objective) - this SHOULD ONLY be used in conjunction with ``Policy Marker`` code *9* (Reproductive, Maternal, Newborn and Child Health) 

Codelist pages
--------------     

*Policy Significance*
`````````````````````
Codelist: :doc:`PolicySignificance </codelists/PolicySignificance>` (`discussion <http://support.iatistandard.org/entries/52320903-New-Policy-Markers-Significance-Codes>`__)

.. list-table::
   :widths: 20 40
   :header-rows: 1

   * - Page
     - Additional guidance 
   * - Policy Significance codelist 
     - Policy Significance code = 4 (Explicit primary objective) SHOULD ONLY be used in conjunction with :doc:`Policy Marker </codelists/PolicyMarker/>` code = 9 (Reproductive, Maternal, Newborn and Child Health)
