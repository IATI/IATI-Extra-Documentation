IATI Codelist Management
========================

The IATI codelists are key to making IATI data from different publishers
comparable.

These lists need to be managed to deal with additions, amendments, bugs,
and deletions. We use GitHub as a tool to manage our change control
process. By placing codelists in GitHub, we have the ability to track
very minor changes and to 'tag' major releases.

The structure of the codelists themselves is governed by a schema that
is versioned and maintained in the GitHub repository for each version of
the standard. e.g. for v2.02:
https://github.com/IATI/IATI-Codelists/blob/version-2.02/codelist.xsd

In managing the codelists we make a distinction between 'embedded' and
'non-embedded' codelists. In addition, we may refer to these lists as
either 'complete' or 'incomplete'.

.. _embedded_codelist:

Embedded Codelists
------------------

These are 'functional' codelists that are core to IATI. Changing them
has a big impact on all those publishing and using IATI data. For example, adding, removing
or renaming something on the transaction-types codelist
http://iatistandard.org/codelists/transaction_type/ could
be very disruptive.

Embedded codelists are  managed via GitHub at:
https://github.com/IATI/IATI-Codelists/

-  Any changes to these codelists should be handled through a formal
   decimal or integer upgrade process.
   (http://dev.iatistandard.org/upgrades/).
   (except bug fixes - see below)
-  Releases are tagged in line with the IATI Standard versions. This
   means you can grab a snapshot of e.g. everything to do with version
   1.03.
-  There are branches for each version of the standard. These can change
   between decimal and integer releases of the standard ONLY for bug
   fixes, typos, and translations. Users can chose to track changes to
   those branches if they like but our documentation (from v1.04
   onwards) will always track the corresponding branch.
-  During an upgrade to the standard, the new version of a new branch is
   created for development.

.. _non_embedded_codelist:

Non-Embedded Codelists
----------------------

These 'non-functional' codelists usually provide lookup information on
e.g. currencies, languages in use, countries, etc. Often they are
derived from third party lists and an addition or modification has a
minor impact on the sense and use of the data.

Non-embedded codelists are managed via GitHub at:
https://github.com/IATI/IATI-Codelists-NonEmbedded

-  We aim to make changes to these lists quickly to allow data users to
   take advantage of the changes immediately. These changes can be made
   outside of a formal decimal or integer upgrade process.
-  Releases would be tagged in line with standard but the minor changes
   will be available on the master branch of this repository.

Updates to Non-embedded Codelists
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Potential changes to Non-embedded Codelists may come to the team via:

-  Personal requests/Support tickets
-  Email notifications
-  Announcements from the source organisations
-  Automatic detection of changes to external sources compared with our own lists.

All proposals will be added to the The `Non-embedded Codelist-Amendments Forum <http://support.iatistandard.org/forums/23076626-Non-embedded-Codelist-Amendments>`__

The IATI Technical Team hold regular team meetings once a week. All outstanding proposals will be discussed at that meeting. The IATI Technical Lead (Bill Anderson) has the ultimate responsibility for decisions taken.

If a decision has been made to make a change to a non-embedded list the `IATI Standard discussion thread <http://discuss.iatistandard.org/c/iati-standard>`__ will be notified (within 1 working day) about the change that is to be made and the date that the change will take effect (usually within 7 calendar days). The proposal will be marked as 'Planned' on the support forum. At this point people have the right to disagree. Discussion should take place via the `IATI Standard discussion thread <http://discuss.iatistandard.org/c/iati-standard>`__. Unresolved matters can be taken to the following team meeting.

In most circumstances the decision to alter these codelists is straightforward. In rare cases, the team may decide to seek further clarification, or to consult further on whether or not to adopt a change. If so, a timetable outlining the process and time scales will be issued.

Once a change has been agreed, a GitHub issue will be created and will be linked to from the forum post.

When the change has been made and accepted into the master branch of the `Non-embedded Codelist repository <https://github.com/IATI/IATI-Codelists-NonEmbedded>`__, the change will be 'live' to anyone who consumes these codelists directly from Github or via the API. 

At this point the technical team will:

 * Update the `Non-Embedded Codelist changelog record <http://iatistandard.org/upgrades/nonembedded-codelist-changelog>`__
 * Regenerate the IATI Standard Website.
 * Mark the forum post as 'Done'

A :doc:`summary of all changes to all non-emebedded </upgrades/nonembedded-codelist-changelog/>` codelists is published on the IATI Standard website. They can also be found via the list of commits to the GitHub repository.

Special Cases
*************

File Format
  The IATI Technical Team will use its judgement to assess the importance of a change to the file format list and whether or not an announcement is required (i.e. the list may alter to stay inline with the external source, but announcements will not necessarily be made).

Organisation Registration Agency
  Because there is a need to add registration agencies quickly, so that people can do their work, and because we anticipate many additions that will not be of interest to most people, we will add values to this list without making announcements. Values to be added will be agreed at the weekly team meeting.
 
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

