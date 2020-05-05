2.01 Headlines
^^^^^^^^^^^^^^

The changes / additions to IATI Standard for version 2.01 represent a number of actions for those publishing and using IATI data.  

This page provides a headline checklist of the core "breaking" changes, linking to further guidance and information.  Alongside these, there are `several changes to elements and codelists <http://iatistandard.org//upgrades/integer-upgrade-to-2-01/2-01-changes/>`__ - this document serves to provide a starter point.

.. contents::

Mandatory changes
==================
For those moving from version 1.0x to 2.01 of the IATI Standard, the following changes must be observed.

Standard wide
-------------
The following changes are "breaking" changes from 1.0x and 2.01, in both the **IATI Activity** and **IATI Organisation** standards:

.. list-table::
   :widths: 20 40 50
   :header-rows: 1

   * - Change
     - 1.0x
     - 2.01
   * - Element Order 
     - Elements could be presented in any order.
     - Elements must be presented in a `strict order in both the Activity and Organisation standards <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#element-order>`__.
   * - **Mandatory Fields**
     - There were a limited number of mandatory elements.
     - There are more mandatory elements in both the `Activity <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#mandatory-fields-in-activity-standard>`__  and `Organisation <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#mandatory-fields-in-organisation-standard>`__  standard.     
   * - **Using free text**
     - Free text could be added to any element.
     - The way in which free text is reported has been changed to standardise multilingual reporting. `This requires formatting changes to all text fields <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#free-text-fields>`__.  In addition, this impacts on the ways in which multilingual `translations are handled across the standard <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#handling-translations>`__..       
   * - **Descriptive text for codes**
     - Fields defined by codes allow for accompanying descriptions.
     - With the exception of countries and regions, the `descriptions associated with codes can no longer be reported <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#mandatory-fields-in-organisation-standard>`__ .    
   * - **Date formatting**
     - Date formatting was less strict.
     - `Date formatting is strictly observed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#formatting-of-dates-and-datetimes>`__ ..  A date must be a expressed in a valid *xsd:date* format.  Datetimes should be a valid *xsd:dateTime*. 
   * - **Organisation Identifier**
     - The organisation identifier used for the publishing organisation was not validated.
     - The organisation identifier used for the publishing organisation must be prefixed with a `valid Organisation Registration Agency code <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#organisation-and-activity-identifiers>`__ . 

          
Activity standard
-----------------
The following "breaking" changes apply specifically to the **IATI Activity Standard**

.. list-table::
   :widths: 20 40 50
   :header-rows: 1

   * - Change
     - 1.0x
     - 2.01
   * - **Language Neutral Codelists** 
     - The codes for Organisation role; Type of Activity Date; Transaction Type; Sector Vocabulary; Gazetteer Agency were aplha characters, derived from English language words.
     - The codes for Organisation role; Type of Activity Date; Transaction Type; Sector Vocabulary; Gazetteer Agency have to be changed to numeric, `making them language neutral <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#language-neutral-codelists>`__.


Organisation standard
---------------------
The following "breaking" changes apply specifically to the **IATI Organisation Standard**

.. list-table::
   :widths: 20 40 50
   :header-rows: 1

   * - Change
     - 1.0x
     - 2.01
   * - **Renamed Element** 
     - A mandatory element named iati-identifier was in use.
     - The iati-identifier element is now organisation-identifier.  `This must be renamed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/migrating/#element-order>`__.
