IATI Codelist Management
========================

The IATI codelists are key to making IATI data from different publishers
comparable. Codelists contain a list of values and each value is assigned a code, e.g. the country Uganda has the code 'UG'. All codes are alphanumeric. Codes help reduce the amount of human error when entering data and having set values helps with data analysis.

Over time, Codelists need to be updated when codes need to be added, removed, or changed. We use GitHub as a tool to manage our Codelists, and you are able to track the changes. By managing Codelists in GitHub, we have the ability to track very minor changes and to 'tag' major releases.

The structure of the codelists themselves is governed by a schema that
is versioned and maintained in the GitHub repository for each version of
the standard. e.g. for v2.02:
https://github.com/IATI/IATI-Codelists/blob/version-2.02/codelist.xsd

There are **four types** of Codelist in IATI: Core, Non-Core, Replicated, and External. Each of these are managed in a different way:

.. _core_codelist:

Embedded Codelists - Core
------------------

Core Codelists contain conforming values for a particular **decimal Version** of the IATI Standard, the contents of which are managed by the IATI Technical Team. Core Codelists contain codes that involve functional logic that impacts the way in which the Standard is interpreted and processed.

These are Codelists that are core to IATI: changing them has a big on impact on all those publishing and using IATI data.

Embedded codelists are  managed via GitHub at:
https://github.com/IATI/IATI-Codelists/

**Modification Schedule: Embedded Codelists - Core**

Codes in Core Codelists may be:

- Added - at a Minor or Major Upgrade, through the applicable consultation process
- Modified - at a Minor or Major Upgrade, through the applicable consultation process
- Withdrawn - at a Minor or Major Upgrade, through the applicable consultation process
- Removed - at a Major Upgrade, through the applicable consultation process

See more information about the IATI Upgrade process here: http://reference.iatistandard.org/203/upgrades/

Examples of Core Codelists include: Transaction Type, Organisation Type.

.. _non_core_codelist:

Non-Embedded Codelists - Non-Core
----------------------

Non-Core Codelists contain conforming values for a particular **integer** version of the IATI Standard, the contents of which are managed by the IATI Technical Team. Non-Core Codelists contain Codes that qualify data, not processes.

These Codelists usually provide lookup information, e.g. Description Type, Geographic Location, Indicator Vocabularies. An addition or modification has a minor impact on the sense and use of the data.

Non-Core Codelists are managed via GitHub at:
https://github.com/IATI/IATI-Codelists-NonEmbedded

**Modification Schedule: Non-Embedded Codelists - Non-Core**

Codes in Non-Core Codelists may be:

- Added - at any point in time, subject to applicable notification and/or consultation via `IATI Discuss  <https://discuss.iatistandard.org/c/standard-management/non-embedded-codelist-amendments>`__
- Modified - at any point in time, subject to applicable notification and/or consultation via `IATI Discuss <https://discuss.iatistandard.org/c/standard-management/non-embedded-codelist-amendments>`__
- Withdrawn - at any point in time, subject to applicable notification and/or consultation via `IATI Discuss <https://discuss.iatistandard.org/c/standard-management/non-embedded-codelist-amendments>`__
- Removed - at a Major Upgrade, through the applicable consultation process via `IATI Discuss <https://discuss.iatistandard.org/c/standard-management/non-embedded-codelist-amendments>`__

Examples of Non-Core Codelists include: Sector Vocabulary, Condition Type, Result Type.

Non-Embedded Codelists - Replicated
----------------------

Replicated Codelists contain values for the IATI Standard. The contents are generally managed by a third-party organisation, in exceptional circumstances an additional code can be added. The IATI Technical Team maintain a corresponding copy in a document that conforms to the Codelist Schema.

**Modification Schedule: Non-Embedded Codelists - Replicated**

Codes in Replicated Codelists may be:

- Added - at any point in time, subject to applicable notification by the third-party
- Modified - at any point in time, subject to applicable notification by the third-party
- Withdrawn - at any point in time, subject to applicable notification by the third-party
- Removed - never

Examples of Replicated Codelists include: DAC 5-Digit, Organisation Registration Agency

Non-Embedded Codelists - External
----------------------

External Codelists are a collection of codes managed by a third-party organisation. The IATI Technical Team does not maintain a correspoding copy in a document that conforms to the Codelist Schema.

**Modification Schedule: Non-Embedded Codelists - External**

Codes in External Codelists may be:

- Added - at any point in time
- Modified - at any point in time
- Withdrawn - at any point in time
- Removed - at any point in time

Examples of Exteral Codelists include: Earmarking Modalities

Changing Codelist Type
----------------------

A Codelist may have its type changed. The points at which this may occur are defined by the following modification schedule:

**Modification Schedule: Codelist Type**

A Codelist may have its type changed through the applicable consultation process via the following steps:

- External to Replicated - at a Minor or Major upgrade
- Replicated to Non-Core - at a Minor or Major upgrade
- Non-Core to Core - at a Minor or Major upgrade
- Core to Non-core - at a Minor or Major upgrade
- Non-Core to Replicated - at a Minor or Major upgrade
- Replicated to External - at a Minor or Major upgrade

Should a Codelist Type change require multiple steps, such as 'Non-Core to External' requireing 'TBC to Replicated' followed by 'Replicated to External', the restriction stated by the final step

 
Code status, addition and withdrawal dates
------------------------------------------
All new codes added to codelist from the release of version 2.02 (December 2015) will feature ``status="active"`` and ``activation-date`` attributes in the underlying GitHub source code repositories.  Similarly, codes withdrawn from the release of version 2.02 (December 2015) will feature ``status="withdrawn"`` and ``withdrawal-date`` attributes.

Complete vs Incomplete Codelists
--------------------------------

Some codelists, such as the ISO country codes, are not ‘complete’ lists
of all possible values that might be used. In the case of countries,
publishers may use extra user defined codes (such as 'XK' for Kosovo) or valid
historical values that are not on our maintained list.

For other codelists, such as the DescriptionType codelist, if the value
is not on the codelist the data doesn’t make any sense - it is invalid.
This is an example of a 'complete' codelist.

We distinguish between these two types of codelists by the use of an xml
attribute: ``complete="1"``
