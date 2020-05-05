Migrating from versions 1.x to version 2.01
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. contents::

Overview
--------
This is an issue by issue guide for data publishers and data users of the IATI Standard.

It is aimed at people who are already familiar with the IATI Standard in it's version 1.x form, and are looking to find out what has changed and how it may or may not affect them when creating or using data built to the 2.01 version of the IATI Standard.

It is recommended that you inspect each point in turn to decide if you need to take any action.

Readers of this document should not assume that the ordering of issues in the document implies a hierarchy of importance. Different data users/publishers will find some issues more relevant/important than others.


Organisation and Activity Identifiers
=====================================
**What does version 2.01 of the IATI Standard require?**

IATI organisation identifiers should:

* be globally unique
* be constructed from a consistent methodology
* be compatible with other data standards

Specifically, a valid organisation identifier:

* Must start with a valid agency prefix
* The agency prefix MUST be a valid code in the :doc:`IATI OrganisationRegistrationAgency codelist </codelists/OrganisationRegistrationAgency/>`
* MUST only contain alphanumeric characters and hyphen, underscore, colon or period

IATI activity identifiers

* must be globally unique
* must be persistent
* must be prefixed with an organisation identifier

It should be recognised that IATI organisation identifiers can change over time. i.e. they CAN NOT be persistent.
Therefore when a reporting organisation's identifier changes, the  previous reporting organisation identifier(s) should be reported in addition to the new one.

This will allow data users to continue to link activities to the organisation that reported them (because activity identifiers are constructed using the organisation identifier as part of the string, and once reported, an activity should maintain its original identifier).

In version 2.01 of the IATI Standard, therefore, we need a way to record the previous organisation identifier when this changes. We can do this using the :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>` element.

For information on the changes to that element see: :ref:`Update to other-identifier element <#update-to-other-identifier-element>`

In addition:

* ALL publishers of IATI data MUST have a valid organisation identifier reported in reporting-org/\@ref
* When using the \@ref attribute in participating-org/\@ref, transaction/provider-org/\@ref and transaction/receiver-org/\@ref must be a valid organisation identifier. If you do not have one, then the narrative element may be used to describe the organisation.
* The reporting-org element is MANDATORY.

  - ALL the following rules must apply to the organisation-identifier in reporting-org/\@ref
  - It is mandatory
  - The identifier MUST be the same as that recorded by the publisher on the IATI Registry

* The iati-identifier is MANDATORY

  - It MUST be globally unique among all activities published through the IATI Registry
  - Once an activity has been reported to IATI its identifier MUST NOT be changed in subsequent updates,
  - It MUST be prefixed with EITHER the organisation-identifier found in reporting-org/\@ref OR a previous reporting-org identifier reported in :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>`
  - The identifier MUST only contain alphanumeric characters and hyphen, underscore, colon or period

**What is the change?**

The biggest change is that all organisations must have an Organisation
Identifier that is prefixed with a valid code on the :doc:`IATI OrganisationRegistrationAgency codelist </codelists/OrganisationRegistrationAgency/>`

This means that a number of publishers will have to:

* Change their organisation identifier
* Continue to report existing activities using the same activity identifier, but also report their previous Organisation Identifier using the :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>` element.

In addition, if they wish to use IATI as their registration agency, they will need to agree their new identifier on the :doc:`IATIOrganisationIdentifier codelist </codelists/IATIOrganisationIdentifier/>`

Wherever \@ref is used to talk about organisations in the standard, those references must be a valid organisation identifier (as defined above).

**Where is this applicable?**


This is fundamental to the creation and use of IATI data and applies throughout the IATI Standard

**What happens if we do not do this?**

While the schema will not be able to test for valid Organisation and Activity identifiers, it is possible to machine write tests to check for some compliance. However if your data does not meet these standards then it becomes difficult for others to use.


Update to other-identifier element
==================================

**What is the change?**


In versions 1.x of the IATI Standard the other-identifier element could be used to specify an alternative, non-IATI identifier for the activity.

In version 2.01 of the IATI Standard the definition of the element has changed to allow an number of types of alternative identifiers.

In version 2.01 of the IATI Standard the element has been re-constructed
 - The \@owner-ref and \@owner-name attributes have been removed.
 - New attributes other-identifier/\@type and other-identifier/\@ref are added
 - The \@type attribute is used to specify the type of identifier being given.
 - The \@ref attribute is used for the identifier itself.
 - There is a child element :doc:`other-identifier/owner-org </activity-standard/iati-activities/iati-activity/other-identifier/owner-org/>` where information about the organisation that crafted the identifier can be given. This field is set up so that multilingual text can be supplied,

In version 2.01 of the IATI Standard a new :doc:`OtherIdentifierType </codelists/OtherIdentifierType/>` codelist is introduced.

**Where is this applicable?**

In the Activity schema

**Why has this been done?**

This change is in part to be able to deal with organisations changing their organisation identifiers. Because an iati-identifier needs to be unique and (once reported to IATI) will never change, and because it is constructed using an organisation identifier, when organisation identifiers change, data users still need to be able to relate activities to organisations.

To solve this, a previous reporting-org identifier can be reported in the
:doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>` element. This then allows us to require that an iati-identifier must be prefixed with:

-  EITHER the organisation-identifier found in reporting-org/\@ref
-  OR a previous reporting-org identifier reported in :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>`

For more information see:
`Organisation and Activity Identifiers <http://support.iatistandard.org/entries/52824355-Version-2-01-Iteration-3-9-Organisation-and-Activity-Identifiers>`__ proposal on the support forum.

To make this element work, a new OtherIdentifierType codelist has been
constructed, and the entire element has been re-constructed.

**Example**

See: :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>`

**What happens if we do not do this?**

- Anyone reporting other-identifier in versions 1.x of the IATI Standard will need to reconstruct the way they report the data. They can continue to report the same data, but just need to reformat it.
- Data users should be aware that parsing :doc:`other-identifier </activity-standard/iati-activities/iati-activity/other-identifier/>` is different in 2.01.
- Data publishers may take advantage of the opportunities to report other types of identifier that were not previously available to them.
- Data may fail validation against the relevant 2.01 schema if the changes are not taken into consideration.


Changes introduced between versions 1.04 and 1.05 have also been included in 2.01
=================================================================================
As 2.01 of the IATI Standard was being prepared there was a decimal upgrade to version 1.05 that ran in parallel. All changes to the Standard between version 1.04 and 1.05 have been carried over into 2.01


Element Order
=============
**What does version 2.01 of the IATI Standard require?**

Data elements must be published in the order specified by the schema.

**What is the change?**

In versions 1.x of the IATI Standard, data elements could be published in any order and still be valid when checked against the relevant schema.

In 2.01 you MUST publish data elements in the order specified by the schema to pass schema validation.

**Why has this been done?**

By enforcing order on the schema we can also enforce the number of times certain elements may occur in the data. This should drive up data quality by making it easier for data publishers to know if they have got their data right using simple validation tests. While this will not cover all the complexities of the the IATI Standard, it will substantially increase the number of data elements than can be checked in this way.

**Where is this applicable?**

In both the Organisation and Activity Standards

**Example**

Element order can be found by:

-  :doc:`inspecting the schema directly </schema/>`

Or via our GitHub repository:

-   `Activity schema <https://raw.githubusercontent.com/IATI/IATI-Schemas/version-2.01/iati-activities-schema.xsd>`__
-  `Organisation schema <https://raw.githubusercontent.com/IATI/IATI-Schemas/version-2.01/iati-organisations-schema.xsd>`__
-  `Common schema <https://raw.githubusercontent.com/IATI/IATI-Schemas/version-2.01/iati-common.xsd>`__

The order is also reflected in the left hand `navigation of the 2.01 website <http://iatistandard.org/201/>`__

Tables generated from the schema can be found at:

-  `Activity summary table <http://iatistandard.org/201/activity-standard/summary-table/>`__
-  `Organisation summary table <http://iatistandard.org/201/organisation-standard/summary-table/>`__

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema.


Mandatory Fields in Activity Standard
=====================================
**What does version 2.01 of the IATI Standard require?**

Certain elements are now mandatory within any iati-activity record.

**What is the change?**

There are more mandatory items. More elements and attributes are made
mandatory by the schema.

Each Activity record MUST contain:

-  a valid activity identifier;  (element (iati-identifier) presence
   tested by schema - validity could be tested by software)
-  a valid reporting organisation identifier; (element (reporting-org)
   presence tested by schema - validity could be tested by software)
-   a funding or implementing organisation; (element (participating-org)
   presence tested by schema - role=funding OR implementing could be
   tested by software)
-  a title and description; (elements (title/narrative,
   description/narrative) presence tested by schema)
-  a start date; (element (activity-date) and attribute (iso-date)
   presence tested by schema, type="1" could be tested by software ) an
   activity status;  (element (activity-status) presence tested by schema)
-  a sector; (presence could be tested by software)
-  a recipient-country or recipient-region (presence could be tested by
   software)

**Participating organisation**

-  At least one occurrence of iati-activity/participating-org is
   MANDATORY - enforced by the schema
-  For each occurrence of participating-org \@role is MANDATORY  -
   enforced by the schema
-  For each occurrence of participating-org \@ref or
   participating-org/narrative is MANDATORY - not enforceable by the
   schema

for discussion go to
`Validation and guidance <http://support.iatistandard.org/entries/41047217-Modify-participating-org-Validation-and-guidance>`__ on the support forum.

**Title**

-  iati-activity/title is MANDATORY  - enforced by the schema
-  It is recommended that the title contains a meaningful summary of the
   activity - not enforceable by the schema

for discussion go to
`Modify title : validation and guidance <http://support.iatistandard.org/entries/41584666-Modify-title-validation-and-guidance>`__ on the support forum.

**Description**

-  The iati-activity/description is MANDATORY  - enforced by the schema
-  It is recommended that the description contains a meaningful
   description of the activity -not enforceable by the schema

for discussion go to
`Modify description : validation and guidance <http://support.iatistandard.org/entries/41584706-Modify-description-validation-and-guidance>`__ on the support forum.

**Activity Date**

-  At least one occurrence of iati-activity/activity-date is MANDATORY
    - enforced by the schema
-  All activities MUST contain a start date: either planned or actual -
   not enforceable

for discussion go to
`Modify activity-date : validation and guidance <http://support.iatistandard.org/entries/41089758-Modify-activity-date-validation-and-guidance>`__ on the support forum.

**Sector / Transaction Sector**

-  Sector may now be reported at transaction level instead of activity
   level. For details see `Replicate more activity-level elements at transaction level <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-2-3-7-Replicate-more-activity-level-elements-at-transaction-level>`__ on the support forum.
-  At least one occurrence of sector OR transaction/sector is MANDATORY
   - not enforceable
-  sector/\@code OR transaction/sector/\@code is MANDATORY  - enforced by
   the schema
-  If Sector/\@vocabulary is not present then the DAC 5-digit vocabulary
   is assumed
-  Use of DAC codes (either 5-digit or 3-digit) is recommended

for discussion go to
`Modify sector : validation and guidance <http://support.iatistandard.org/entries/22993317-Modify-sector-validation-and-guidance>`__ on the support forum.

**budgets / planned-disbursement**

budgets and planned-disbursements now contain mandatory elements when
used.

**Budget dates**

- The budget element should be repeated for each year of the activity's
   duration - not enforceable
- If the budget element is present then

  * period-start/\@iso-date is MANDATORY and must be a valid ISO format (enforced by the schema)
  * period-end/\@iso-date is MANDATORY and must be a valid ISO format (enforced by the schema)
  * period-end/\@iso-date must be after period-start/\@iso-date (not enforceable by the schema)
  * Each budget should cover a period no longer than 1 year (not enforceable by the schema)

for discussion go to
`Modify budget/period-start and budget/period-end : make mandatory <http://support.iatistandard.org/entries/22900321-Modify-budget-period-start-and-budget-period-end-make-mandatory>`__ on the support forum.

In addition, when other non-mandatory elements are used, the schema may dictate whether or not child elements must be present, the number of times they may occur, and the presence of attributes. You can find the detail in the :doc:`relevant schema documents </schema/>`

The 'occurs' column of the `standard overview table <http://iatistandard.org/201/activity-standard/summary-table/>`__ also indicates where both elements and attributes are required, and how often they may occur.

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Mandatory Fields in Organisation Standard
=========================================
**What does version 2.01 of the IATI Standard require?**

Certain elements are now mandatory within any iati-organisation record.

**What is the change?**

There are more mandatory items. More elements and attributes are made
mandatory by the schema.

Each Organisation record MUST contain:

-  a valid organisation identifier;  (element (:doc:`organisation-identifier </organisation-standard/iati-organisations/iati-organisation/organisation-identifier/>`) presence tested by schema)
-  a name; (element (:doc:`name/narrative </organisation-standard/iati-organisations/iati-organisation/name/narrative/>`) presence tested by schema)
-  a valid reporting organisation identifier (element (:doc:`reporting-org </organisation-standard/iati-organisations/iati-organisation/reporting-org/>`)
   presence tested by schema - validity could be tested by software)

In addition, when other non-mandatory elements are used, the schema may dictate whether or not child elements must be present, the number of times they may occur, and the presence of attributes.  You can find the detail in the relevant :doc:`schema documents </schema/>`.

The 'occurs' column of the `standard overview table <http://iatistandard.org/201/organisation-standard/summary-table/>`__ also indicates where both elements and attributes are required, and how often they may occur.

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Declaring the Version of the IATI Standard being used
=====================================================
**What does version 2.01 of the IATI Standard require?**

You MUST correctly report the version of the standard you are using.

**What is the change?**

In the Activity Standard

-  From version 2.01, the \@version attribute of `iati-activities <http://iatistandard.org/201/activity-standard/iati-activities/>`__
   is mandatory
-  In version 1.x the \`\`iati-activity\`\`element had an \@version
   attribute. This is no longer the case in version 2.01 (it has been
   removed).
-  The values for \@version must be on the `version codelist <http://iatistandard.org/201/codelists/Version/>`__.

In the Organisation Standard

-  From version 2.01, the \@version attribute of `iati-organisations <http://iatistandard.org/201/organisation-standard/iati-organisations/>`__ is mandatory
-  In version 1.x the \`iati-organisation\` element had an \@version
   attribute. This is no longer the case in version 2.01 (it has been
   removed).
-  The values for \@version must be on the `version codelist <http://iatistandard.org/201/codelists/Version/>`__.

**Where is this applicable?**

In both the Organisation and Activity standards

**Example**

For examples see:

-  `iati-activity example <http://iatistandard.org/201/activity-standard/iati-activities/>`__
-  `iati-organisation example <http://iatistandard.org/201/organisation-standard/iati-organisations/>`__

**What happens if we do not do this?**

If you omit iati-activities/\@version or iati-organisations/\@versions the
data will fail validation against the relevant 2.01 schema.

If you include iati-activity/\@version or iati-organisation\@version the
data will fail validation against the relevant 2.01 schema.

If you do not use a value for \@version from the `version codelist <http://iatistandard.org/201/codelists/Version/>`__. data
users may have difficulty processing your data.


Using Namespaces
================
**What does version 2.01 of the IATI Standard require?**

Data publishers are allowed to add data using their own defined namespaces to add additional data to an IATI data file. They must do this in such a way that their data is still valid against the relevant schema.

**What is the change?**

Because ordering has been enforced in the schema, any namespace elements are now expected to be positioned as the last child of the relevant parent element.

**Where is this applicable?**

In both the Organisation and Activity standards

This applies to any use of namespaces

**Example**

For examples see:

-  `iati-activity example <https://github.com/IATI/IATI-Schemas/blob/version-2.01/tests/activity-tests/should-pass/03-top-level-extensibility.xml>`__
-  `iati-organisation example <https://github.com/IATI/IATI-Schemas/blob/version-2.01/tests/organisation-tests/should-pass/02-top-level-extensibility.xml>`__

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Segmentation and file size
==========================
**What does version 2.01 of the IATI Standard require?**


-  In order to ensure that all all IATI-XML files can be handled by all consuming systems it is proposed that a limit of 40MB is placed on the size of any single XML file.
-  Publishers are still encouraged to segment their data into meaningful chunks, BUT the guidance to segment by country is no longer necessarily considered to be best practice.
-  (NB the rule that the activity iati-identifier must be unique still applies. i.e. the same activity should not be reported in two different files by the same publisher)

**What is the change?**

Previous guidance has been to segment data by country where possible/useful. This was an arbitrary decision.

**What happens if we do not do this?**

Files larger than 40MB are difficult for data users to use - even at 40MB this is still difficult for many users. If your files are too large it is possible that applications wanting to use your data may not be able to do so.


Free Text Fields
================
**What is the change?**

In version 2.01 free text is handled very differently than it is in
versions 1.x

Every element in versions 1.x where free text can be supplied has
changed in version 2.01.

Text is no longer reported directly in the element itself, instead every
affected element gets a new 'narrative' child element, where the text
can be supplied. The narrative element can be repeated in order to
supply translations in different languages.  See **Handling Translations**

There are many elements that contain data specified by a code value
where free text can no longer be supplied at all. See **Descriptive text
is no longer allowed on data specified by codes (with some exceptions)**

**Why has this been done?**

The change has been made to improve how multilingual reporting can
occur, and to improve clarity where codes are reported.

**Where is this applicable?**

In both the Organisation and Activity Standards

Even where publishers do not supply translations of their text data,
they are still required to alter the way they report free text.

**Example**

How to declare a title

In 1.x

.. code-block:: xml

	<title>Some title here</title>

in 2.01

.. code-block:: xml

	<title>
		<narrative>Some title here</narrative>
	</title>

**See also**

Examples of how this change works can be seen on (for example):

-  :doc:`activity title </activity-standard/iati-activities/iati-activity/title/>`
-  :doc:`organisation name </organisation-standard/iati-organisations/iati-organisation/name/>`

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Handling Translations
=====================
**What does version 2.01 of the IATI Standard require?**

The standard wants to allow publishers to easily declare multilingual translations for text data, and for data users to be able to easily access those translations. In 2.01 the way in which this done should make it easier for data users to handle.

**What is the change?**

In version 1.x elements that allowed text to be declared (e.g. title) could be repeated for different languages.

In version 2.01 instead of repeating the parent element  (e.g. title) , those elements now have a <narrative> child element, which can repeated for different languages.

The narrative element uses the xlm:lang attribute to declare the language of the supplied text. If omitted then the text is assumed to be in the default language declared in the document root element.

**Where is this applicable?**

For a full list of elements where this now applies, see: Including nested, multi-lingual text elements for all elements containing free text in this post:
`Multi-lingual text fields <http://support.iatistandard.org/entries/52106219-Version-2-01-Iteration-3-4-Multi-lingual-text-fields>`__ on the support forum.

**Example**

Examples of how this change works can be seen on (for example):

-  :doc:`activity title </activity-standard/iati-activities/iati-activity/title/>`
-  :doc:`organisation name </organisation-standard/iati-organisations/iati-organisation/name/>`

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Descriptive text is no longer allowed on data specified by codes (with some exceptions)
=======================================================================================
**What does version 2.01 of the IATI Standard require?**

Where published data is defined by codes, the code is authoritative, and the associated look up value should not supplied.

There are two exceptions:  recipient-country and recipient-region, where descriptive text is allowed when a publishing organisation does not agree with the definition given by the ISO 3166-1 part of the ISO 3166 standard

**What is the change?**

In version 1.x of the standard, a number of elements allowed the reporting of a code (usually in an attribute) and free text.  Where both a code and text was supplied it was impossible for a data user to know which field was authoritative.

In 2.01 the code is authoritative, and the ability to add free text has been removed from a number of elements.

**Where is this applicable?**

For a list of elements where this applies see:

Scrapping text of purely code elements -
`Multi-lingual text fields <http://support.iatistandard.org/entries/52106219-Version-2-01-Iteration-3-4-Multi-lingual-text-fields>`__ on the support forum.

**Example**

In version 1.x this was allowed:

.. code-block:: xml

	<activity-status code="2" >Implementing</activity-status>

as was;

.. code-block:: xml

	<activity-status code="2" >implementing</activity-status>

and;

.. code-block:: xml

	<activity-status code="2" >any text here</activity-status>

and even;

.. code-block:: xml

	<activity-status code="2" >Post Completion</activity-status>

In version 2.01, all of the above would fail validation against the schema as text is not allowed at all in this element. To indicate an activity status of implementing you would simply declare:

.. code-block:: xml

  <activity-status code="2" />

**Exceptions**

Both the recipient-region and recipient-country elements still allow both a code and descriptive text to be specified. This is to cover the cases where the organisation publishing the data may not agree with name of a country or region given by the lookup codelists IATI uses.

Data users should be aware that where the narrative element has been supplied then that publishers prefers the name supplied to be associated with it's data.

**Example**

To declare a recipient country of Kosovo, both of these are acceptable:

.. code-block:: xml

  <recipient-country code="XK" />

Here, a lookup against the relevant codelist (:doc:`Country </codelists/Country/>`)
   would return a country name of 'Kosovo'

If you prefer to declare a different name that differs from the ISO 3166-1 part of the ISO 3166 standard  (e.g. Kosovo (As per UNSCR 1244)) then do this:

.. code-block:: xml

	<recipient-country code="XK">
		<narrative>Kosovo (As per UNSCR 1244)</narrative>
	</recipient-country>

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Language Neutral Codelists
==========================
**What is the change?**

A number of codes on several codelists have been changed, in order to
make them language neutral.

In general:

-  Codes have changed from english strings to numbers
-  The english string now becomes the 'name' associated with that code
-  Where 'name' information was previously available, this is moved into
   a 'description' field

**Where is this applicable?**

A list of the affected codelists, and the differences between version 1.x and 2.01 are detailed under **Codelist Changes** on the :doc:`2.01 Changes </upgrades/integer-upgrade-to-2-01/2-01-changes>` page of the website.

**What happens if we do not do this?**

Data will not be referenceable against the relevant code list, making it difficult to use.

Allow multiple languages to be specified for a single document (document-link)
==============================================================================
**What is the change?**

In version 1.x of the IATI Standard, you were only allowed to use one document-link/language child element per document-link parent.

In version 2.x of the IATI Standard, you can specify as many document-link/language elements as you need.

**Where is this applicable?**

In both the Activity and Organisation standard.

**Why has this been done?**

In recognition that some documents are multilingual

**What happens if we do not do this?**

Nothing. This change is an opportunity to produce more accurate data.


New Elements
============
**What is the change?**

In version 2.01 of the IATI Standard there is a new element
iati-activity/contact-info/department

In version 2.01 of the IATI Standard there are many new 'narrative' elements introduced as child elements to specify free text: see Free Text Fields above

In version 2.01 of the IATI Standard there is a new element iati-organisation/total-budget/budget-line

In version 2.01 of the IATI Standard there is a new element
iati-organisation/recipient-org-budget/budget-line

In version 2.01 of the IATI Standard there is a new element
iati-organisation/recipient-country-budget/budget-line

Usage

-  budget-line should be used in addition to total-budget/value,
   recipient-org-budget/value and/or recipient-country-budget/value. NB
   that it does not replace the existing reporting guidelines
-  budget-line/\@ref as a reporting organisation reference for the budget
   line
-  budget-line/narrative for a description of the budget line (repeated
   for multiple languages)
-  budget-line/value

**See also**

Additionally, new child elements have been introduced to the existing

-  iati-activity/transaction element: Additional elements in the
   transactions
-  iati-organisation/document-link elements: Additional elements in
   Organisation documents (document-link)

**Why has this been done?**

A number of publishers have requested the facility to add department
information to contact details.

A number of publishers have requested the facility to add granularity to
organisation-level budgets.

Free text has been altered to improve the ability to report data in many
languages.

**What happens if we do not do this?**

In the case of the narrative element, these are required when using
freetext

The other new elements are all optional.


Renamed, Moved and Removed Elements
===================================
**What is the change?**

In versions 1.x of the IATI Standard there is an element
iati-organisation/iati-identifier

In version 2.01 of the IATI Standard this element has been renamed as
iati-organisation/organisation-identifier

In versions 1.x of the IATI Standard there is an element:
iati-activity/crs-add/aid-type-flag. This element has an associated
codelist: AidTypeFlag

In version 2.01 of the IATI Standard this element has been renamed:
iati-activity/crs-add/other-flags, and the AidTypeFlag codelist has been
renamed CRSAddOtherFlags

In versions 1.x of the IATI Standard
iati-activities/iati-activity/activity-website element is it's own
element.

In version 2.01 of the IATI Standard, to report an activity website you
would do so using a document-link element, and it's child 'category' (usually code *A12*) to specify the document is a web site.  Additionally, the FileFormat code *text/html* should be used:

.. code-block:: xml

   <document-link format="text/html" url="http:www.example.org/activity/1234">
     <title>
       <narrative>Activity website</narrative>
     </title>
     <category code="A12" />
     <language code="en" />
   </document-link>




**What happens if we do not do this?**

If elements and attributes are published with the old properties, then
data will fail validation against the relevant 2.01 schema


Using Recipient-Region and Recipient Country
============================================
**What does version 2.01 of the IATI Standard require?**

From the schema (recipient-country):

"Multiple countries and regions can be reported, in which case the percentage attribute MUST be used to specify the share of total commitments across all reported countries and regions.

The country can also be specified at transaction rather than activity level. If transaction/recipient-country AND/OR

transaction/recipient-region are used THEN ALL transaction elements MUST
contain a recipient-country and/or

recipient-region element AND iati-activity/recipient-region and
iati-activity/recipient-region MUST NOT be used AND each

transaction MUST only contain one recipient-country or
recipient-region."

It should be clear that:

-  recipient-region should only be used to indicate that the region as a
   whole is a recipient, not as an added description to a named
   recipient-country
-  if both elements are used percentages must be reported and they
   should add up to 100% across all recipient- elements

**What is the change?**

In versions 1.x of the IATI Standard, data publishers were told to
report EITHER recipient-country or recipient-region, but not both.

In version 2.01 of the IATI Standard, data publishers may report BOTH
recipient-country AND recipient-region with a percentage split.

In versions 1.x of the IATI Standard, it was not possible to report
regions or countries at transaction level.

In version 2.01 of the IATI Standard, regions or countries can be
reported at transaction level.

In version 2.,01 of the standard, you MUST NOT report regions and
countries at BOTH activity and transaction level

**Example**

See:

-  :doc:`Country </activity-standard/iati-activities/iati-activity/recipient-country/>`
-  :doc:`Region </activity-standard/iati-activities/iati-activity/recipient-region/>`

**See also**

Additional elements in transactions (sector, recipient-country,
recipient-region) below

**What happens if we do not do this?**

Nothing. This change is an opportunity to produce more accurate data.


Additional elements in transactions (sector, recipient-country, recipient-region)
=================================================================================
**What is the change?**

In version 2.01 of IATI activity standard the elements of sector, recipient-country and recipient-region have been added as child elements for any transaction. Each of these elements takes the same format as when used at activity level except that the \@percentage attribute is missing.

**Where is this applicable?**

Only in the Activity standard

**Why has this been done?**

In order to provide more accurate reporting of multi-country and multi-sector activities, and to allow for the changing of the activity-level sector over time without compromising previously reported sector-specific commitments and disbursements, it is proposed to add the following fields at transaction level (in addition to activity-level):
 
N.B. If any of these elements are used at transaction level, they must not be used at activity level within the same activity.

N.B. Percentage splits at transaction level are not allowed. If you wish to do this, you should break the transaction up into more transactions, each of which reports more specific information.

For more information see:
`Replicate more activity-level elements at transaction level <http://support.iatistandard.org/entries/52106549-Version-2-01-Iteration-3-7-Replicate-more-activity-level-elements-at-transaction-level>`__ on the support forum.

**What happens if we do not do this?**

Nothing. This change is an opportunity to produce more accurate data.


Additional elements in Organisation documents (document-link)
=============================================================
**What is the change?**

There is now a document-link/recipient-country element ONLY in the Organisation standard. This is to allow multiple countries to be reported per document-link.

**Where is this applicable?**

Only in the Organisation standard

**Why has this been done?**

In order for organisation-level documents to be classified by country.

**What happens if we do not do this?**

Nothing. This change is an opportunity to produce more accurate data.


Formatting of Dates (and datetimes)
===================================
**What does version 2.01 of the IATI Standard require?**

To ensure that IATI data can be utilised, dates and datetimes should be formatted in a consistent way.

In version 2.01 a date should be a valid xsd:date, and a datetimes
should be a valid xsd:dateTime

**What is the change?**

In versions 1.x of the IATI Standard dates and date formats were specified with reference to ISO 8601 standard, and it was not always clear how that standard should be interpreted and used.

In version 2.01 a date should be a valid xsd:date, and a datetimes
should be a valid xsd:dateTime

**Why has this been done?**

In the past IATI has not given clear guidance about the specific formats of the ISO 8601 standard that can be used. It is clear that the data types built into the XML standard, xsd:date and xsd:dateTime, are both well suited and
sufficient for the needs of data publishers and data users.

By specifying this requirement, it also allows dates and datetimes in
the data to be easily validated.

**Where is this applicable?**

In both Activity and Organisation standard.

Wherever a date or a datetime is required (search the schema for xsd:date xsd:dateTime) it should be a valid value.

For most publishers their existing date/datetime data will be valid.
Testing your data against schema validation will easily show if your
dates need altering (re-formatting)

Affected attributes:

dates:

-  all \@iso-date attributes
-  fss/\@extraction-date attribute
-  all \@value-date attributes

datetimes:

-  all \@generated-datetime attributes
-  all  \@last-updated-datetime attributes

**Example**

Examples of how this change works can be seen on (for example):

-  -  :doc:`<Activity standard - activity date </activity-standard/iati-activities/iati-activity/activity-date/>`
-  :doc:`<Organisation standard - period start </organisation-standard/iati-organisations/iati-organisation/total-budget/period-start/>`

**What happens if we do not do this?**

If your dates and datetimes are not in the correct formats, schema validation will fail. If your dates already meet xsd:date and xsd:dateTime formats, then you do not to take any action.


URL validation
==============
**What is the change?**

In version 1.x of the IATI Standard,  the schema data type used for some
data fields where a URL was expected was set as xsd:string.

In version 2.01 of the IATI Standard,  the schema data type used for
some data fields where a URL is expected is now set as xsd:anyURI

**Example**

'website' is a child element of contact-info.

In version 1.x the following would validate against the schema:

.. code-block:: xml

	<website>any string here</website>

In version 2.01, in order to validate against the schema the data you supply must fit the requirements of xsd:anyURI

N.B. xsd:anyURI does not guarantee that a valid URL will be supplied.

**Why has this been done?**

To make validation of the data at the schema level easier

**What happens if we do not do this?**

Nothing UNLESS you have been publishing data that does not meet the restrictions of xsd:anyURI. URL data that was recognised as a string, but not as xsd:anyURI will now fail validation against the relevant 2.01 schema


Location Changes
================
**What does version 2.01 of the IATI Standard require?**

If you are currently using a version of the IATI Standard lower than 1.04 AND report details of sub-national geographic locations, you MUST adopt all the changes specified in the upgrade from version 1.03 of the IATI Standard to version 1.04.

**What is the change?**

Significant changes to the way that location data could be reported were
introduced in the upgrade of the standard from version 1.03 to version
1.04.

However, to ensure backwards compatibility, nothing was removed, but some elements and attributes were deprecated (i.e. still available for use, but no longer recommended).

In addition more elements and attributes were added.

Anything deprecated in 1.x has not been carried over into 2.01 (it has,
in effect, been removed)

If you currently report location information BUT have NOT switched to the supported way of doing so in line with version 1.04 of the IATI Standard, you will need to adjust the way you report location information in 2.01

A detailed guide to what has changed and what you need to do can be
found in the :doc:`location summary guide </upgrades/decimal-upgrade-to-1-04/location-summary/>`

In version 2.01, these elements are no longer available:

-  location/coordinates
-  location/gazetteer-entry
-  location/location-type

In version 2.01, these attributes are no longer available:

-  location/\@percentage
-  location/administrative/\@country
-  location/administrative/\@adm1
-  location/administrative/\@adm2

**What happens if we do not do this?**

Data will fail validation against the relevant 2.01 schema


Changes to the Planned Disbursement element (planned-disbursement)
==================================================================
**What is the change?**

In versions 1.x of the IATI Standard there is a planned-disbursement/\@updated attribute

In version 2.01 of the IATI Standard the  planned-disbursement/\@updated attribute is no longer available (it has been removed)

In version 2.01 of the IATI Standard the planned-disbursement/\@type
attribute, that uses the BudgetType codelist is added

In version 2.01 of the IATI Standard, if a planned-disbursement is given, then the planned-disbursement/period-start element is mandatory and a date must be supplied using its \@iso-date attribute.

In versions 1.x of the IATI Standard the description in the schema of the planned-disbursement/period-end stated that "This element must be present"

In version 2.01 of the IATI Standard the planned-disbursement/period-end
element is optional.

**Why has this been done?**

The planned-disbursement element contain indicative information that is
subject to change. The standard does not expect an audit trail of these
changes to be reported.

While, for example, the budget element handles this correctly by simply indicating (through budget/\@type) whether the budget is original or revised, a planned-disbursement currently requires a date on which the data was last updated (planned-disbursement/\@updated). This is not necessary, so it is being removed and instead the \@type attribute is added.

Making the start date mandatory (if the element is used) will improve data quality and enable publishers and data users to better check that their data is complete. See: `Modify planned-disbursement/period-start : Alter guidance AND make start-date mandatory <http://support.iatistandard.org/entries/22915067-Modify-planned-disbursement-period-start-Alter-guidance-AND-make-start-date-mandatory>`__ on the support forum.

Making the planned-disbursement/period-end element optional allows
publishers more scope to report planned disbursements that do not have a
defined end date.

**What happens if we do not do this?**

If you continue to use the \@updated attributes your data will fail
validation against the relevant 2.01 schema

The \@type attribute is optional.


Removal of the \@type attribute on some description elements
============================================================
**What is the change?**

In version 1.x of the IATI Standard all description elements have a \@type attribute.

In version 2.01 of the IATI Standard this is only applicable to iati-activity/description, therefore the following attributes have been removed:

-  country-budget-items/budget-item/description/\@type
-  result/description/\@type
-  result/indicator/description/\@type

**What happens if we do not do this?**

If you currently use \@type on any of the elements detailed above and do not change that when creating 2.01 data, your data will fail validation against the schema. Data users should be aware that if they expect to gather data from those fields they should no longer be present.


Embedded codelists - Codelists added and removed
================================================
**What is the change?**

As part of the 2.01 IATI Standard upgrade, the Vocabulary codelist was  split into two new codelists. The following embedded codelists were added:

* Policy Marker Vocabulary
* Sector Vocabulary

and the following embedded codelists were removed:

* Vocabulary

**See also**

**Codelist Changes** on the :doc:`2.01 Changes </upgrades/integer-upgrade-to-2-01/2-01-changes>`

**Why has this been done?**

The Vocabulary codelist has over time become unfit for it's original purpose as more and more elements have required their own tailored vocabulary choices. Where vocabularies are used, they are often tailored to that particular element.

**What happens if we do not do this?**

You will need to re-organise the way you present data using the new vocabularies. If you do not do this your data may not be useable by data users.


Embedded codelists - New Codes
==============================
**What is the change?**

As part of the 2.01 IATI Standard upgrade, the following embedded codelists were updated.

* Aid Type Flag: Renamed to CRSADDOtherFlags codelist
* Activity Date Type: Amended codes
* Document Category: New codes
* Gazetteer Agency: Amended codes
* Organisation Role: Amended codes
* Policy Marker Vocabulary (was Vocabulary): Amended codes
* Related Activity Type: New code
* Sector Vocabulary (was Vocabulary): Amended codes
* Transaction Type: Amended codes
* Vocabulary: Removed / split codelist

**See also**

**Codelist Changes** on the :doc:`2.01 Changes </upgrades/integer-upgrade-to-2-01/2-01-changes>`


Embedded codelists - descriptions of code values
================================================
**What is the change?**

Embedded codelist descriptions have been reviewed and updated.

In some cases, description text has been added, where it was previously
missing.

**Where is this applicable?**

In all embedded codelists.

You can see the changes in this code commit:
https://github.com/IATI/IATI-Codelists/commit/33b2174f8c2aeb42f277f8ad9d715b31233179bc

**See also**

**Codelist Changes** on the :doc:`2.01 Changes </upgrades/integer-upgrade-to-2-01/2-01-changes>`

**Why has this been done?**

It was recognised that various description texts were out-of-date or not clear.  This has been an opportunity to update these.


Non-Embedded Codelists
======================
**What is the change?**

As part of the 2.01 IATI Standard upgrade, the following non-embedded codelists were created.

New Non-Embedded Codelists
* Other Identifier Type
* Version
* IATIOrganisationIdentifier

and the following Non-Embedded Codelists were removed:
* OrganisationIdentifier

**See also**

:doc:`Non-Embedded Codelist Changelog </upgrades/nonembedded-codelist-changelog/>`


Update of Schema description texts
==================================
**What is the change?**

Descriptive text in the schema has been reviewed and updated.

In some cases, description text has been added, where it was previously missing.

Descriptive text no longer contains URLs (in effect they have been removed). See: `Removing urls from schema descriptions <http://support.iatistandard.org/entries/47188607-Removing-urls-from-schema-descriptions>`__ on the support forum.

**Where is this applicable?**

In the Activity schema, the Organisation schema and the Common schema.

**Why has this been done?**


It was recognised that various description texts were out-of-date or not clear.  This has been an opportunity to update these.

URLs are no longer maintained in schema text in order to maintain those links more appropriately. As part of that decision, a machine readable way of mapping attributes to codelists has been created to help developers. See:`Mapping between codelists and schemas <http://support.iatistandard.org/entries/27805388-Mapping-between-codelists-and-schemas>`__ on the support forum.


Tied and partially tied values
==============================
New guidance has been added

See: `Tied and partially tied values <http://support.iatistandard.org/entries/55170393-Tied-and-partially-tied-values>`__ on the support forum.


Modify guidance on participating-org/\@role : Definition of funding organisation
=========================================================================================================
See: `Modify guidance on participating-org/@role : Definition of funding organisation <http://support.iatistandard.org/entries/41583626-Modify-guidance-on-participating-org-role-Definition-of-funding-organisation>`__ on the support forum.
