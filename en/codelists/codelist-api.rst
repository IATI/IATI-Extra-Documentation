Codelist API
============

IATI provides two machine readable ways for people to consume the codelists
needed to create and interpret IATI data.

You can:

1. use the Codelist API to request a codelist via a URL

2. From version 1.04 of the IATI standard upwards, you can work directly with our GitHub repositories


API Calls
^^^^^^^^^

To download a codelist. Select your endpoint (see below) and then specify the codelist name and the format:

<endpoint><codelist name>.<extension (xml/json/csv)>

Codelist Mappings
^^^^^^^^^^^^^^^^^

There exists a machine readable mapping from attributes to the codelist they should be on.
This is available on GitHub as an XML file:
https://github.com/IATI/IATI-Codelists/blob/version-2.01/mapping.xml

It is also available as XML and JSON from the codelist API:

.. code::

    http://iatistandard.org/{105,201}/codelists/downloads/clv{1,2,3}/mapping.{xml,json}

Endpoints
^^^^^^^^^

The codelists used in each version of the standard are derived from different endpoints as a result of the historical management of the codelist API. From May 2014, these are now under in-house control at IATI.

Therefore anyone relying on the services at:

* http://datadev.aidinfolabs.org/data/, or
* http://data.aidinfolabs.org/data/

is strongly advised to migrate to the new endpoints given below. 

* v1.01 of the standard - used datadev - change to http://codelists102.archive.iatistandard.org/data/
* v1.02 of the standard - used datadev - change to - http://codelists102.archive.iatistandard.org/data/
* v1.03 of the standard - used data - change to - http://codelists103.archive.iatistandard.org/data/

.. _codelist_api_1.04:

Codelists in Version 1.x after v1.03 (e.g. v1.04, v1.05) of the standard
------------------------------------------------------------------------

In v1.04 of the standard a new codelists structure was introduced. See **Why create a new structure for codelists?** below. 

We call this 'codelist version 2 (CLv2)'. This forms the 'single source of truth' from which codelists in various forms can be produced.

As this new structure would force a change on data users/producers to alter their routines for consuming codelists, we use the single source of truth to 
generate codelists in the previous format that they are used to. We named that format 'codelist version 1 (CLv1)'.

Data users/producers can choose which format they wish to consume via the API. To stick with the old format, use CLv1.

The codelists matching the highest decimal version of the version 1.x standard will always be found using either:

  * http://iatistandard.org/codelists/downloads/clv1/, or
  * http://iatistandard.org/codelists/downloads/clv2/
  
To 'lock in' to a particular version of the codelists (above v1.03) you may specify
  * http://iatistandard.org/<version>/codelists/downloads/clv1/ 

For example: (note: use version number without the decimal point)
  * http://iatistandard.org/104/codelists/downloads/clv1/ will always return v1.04 codelists
  * http://iatistandard.org/105/codelists/downloads/clv1/ will always return v1.05 codelists
  
By locking into a specified version in this way, you can always guarantee you are getting the lists associated with that particular version of the standard, and 
not accidentally move up to a new version when a new version is released.

From version 1.04 onwards, developers might also choose to work directly with GitHub to get the data (see below).

New Codelist version (CLv3) in Version 2.01 of the IATI Standard
----------------------------------------------------------------

Version 2.01 of the IATI Standard sees a significant change to the way multilingual text can be reported. (see http://iatistandard.org/201/upgrades/integer-upgrade-to-2-01/migrating/#handling-translations) 

As codelists can also supply definitions and descriptions in multiple languages, we decided to bring the XML format of the codelists into line with rest of the standard.

This change applies to the 'source' XML files from which the codelist API, the documentation on the website, and so on, is generated.

We are changing the format of the source XML in the IATI-Codelists and IATI-Codelists-NonEmbedded repositories. This is the third change we have made to the codelist format over the lifetime of IATI, so we are calling this CLv3 (Code List format version 3). The XML schema that defines the new format is available here: https://github.com/IATI/IATI-Codelists/blob/version-2.01/codelist.xsd

Anyone **who fetches their codelists directly from GitHub** will be affected by this change.

Developers dealing with version 1.04, 1.05 (and any subsequent version 1.x decimal versions) data with need to work with both the CLv2 format in the IATI-Codelists repository on the version-1.x branch, AND the CLv3 version of the IATI-Codelists-NonEmbedded repository (master branch)

However, the old XML formats (CLv1,CLv2) are still available from the web API. Since the API is versioned, the new CLv3 XML will only be served via the API to those explicitly requesting it.

To compare the old style XML with the new see for example:

| Old style XML (CLv2):
| http://iatistandard.org/201/codelists/downloads/clv2/xml/ActivityDateType.xml

| New Style XML (CLv3):
| http://iatistandard.org/201/codelists/downloads/clv3/xml/ActivityDateType.xml

Working with GitHub Directly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The codelist source is now on GitHub:

Embedded Codelists
------------------
As of version 1.04, each version of the standard has it's own branch in this repository. Branches are named version-<version-number> e.g. version-1.05.
So, for example, the version 1.05 codelists can be found at:

- https://github.com/IATI/IATI-Codelists/tree/version-1.05/xml

Non-Embedded Codelists
----------------------
These values on these lists can change independently of IATI versions. The latest versions are always on the 'master' branch.

- https://github.com/IATI/IATI-Codelists-NonEmbedded/tree/master/xml

This repository now uses the Codelist Version 3 format.

We use this source to create all derived versions, (CSV, JSON and all forms of codelist version 1, and codelist version 2 files, as well as all the documentation on the iatistandard.org website)

If you wish to use the new style XML, or are prepared to run the supplied python scripts for converting to a different format of your choice, you can fetch the codelists from GitHub directly.

Developers dealing with version 1.04, 1.05 (and any subsequent version 1.x decimal versions) data with need to work with both the CLv2 format in the IATI-Codelists repository on the version-1.x branch, AND the CLv3 version of the IATI-Codelists-NonEmbedded repository (master branch)


Why did we create a new structure for codelists for verison 1.04?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
As part of our move towards creating a :doc:`Single Source of Truth </developer/ssot/>` for the IATI Standard, we have started to take a different approach to codelists. See background paper previously circulated: https://docs.google.com/document/d/1oeH-8BFB__2IYF4MLnUwx2LcXZCVd5e-iYsXtQ4ViTk/edit

As this work progressed, it became evident that for the codelists to work in that environment we would need to make a few changes. As a result:

1. The newer codelist files are more consistent: 
 
 * they don't include the element name as a tag name
 * all have language information described the same way as IATI XML. 

2. There is also a codelist schema that all the source XML validates against - https://github.com/IATI/IATI-Codelists/blob/version-1.04/codelist.xsd.

3. Finally, more metadata, including a description, is now included in the codelists.

If you rely on the codelist API you should also read the notes on **Codelist API Compatibility in version 1.04 of the IATI Standard and above** below.


Codelist API Compatibility in version 1.04 of the IATI Standard and above
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
For version 2.01 data, a more sustainable approach would be to migrate your codelist handling routines to deal with the latest CLv3 format.

If moving from a version before 1.04 to a higher 1.x decimal version you might first consider moving your data to version 2.01 instead.
If you decide to upgrade to a higher 1.x version, you should consider going to the highest decimal version your data can accommodate.
If you do this you may not need to alter the way you deal with codelists, but there are a few things that anyone relying on CLv1 should be aware of.

* The 'metadata' link/call is no longer available (instead, some of this is now available in the CLv2 style code lists, and some is stored in the github repository metadata to be consistent with the rest of the Single Source of Truth)
* Only the latest versions (those required in v1.04 of the standard and above) will be available through the API. If you need an older version use the static archives detailed above.
* URLs containing the version and/or language do not work. (for example in the past a url like: /data/codelist/AidTypeFlag/version/1.0/lang/en was possible. This will not work using the /codelists/downloads/clv1/ endpoint. Instead, translations, where available, are maintained in the codelist version 2 (CLv2) files.
* The 'fields' element is no longer provided in the index XML/JSON (See http://data.aidinfolabs.org/data/codelist.xml and compare with http://iatistandard.org/codelists/downloads/clv1/codelist.xml
* Version information is no longer provided in the XML.
* Specific changes to codelists:

  * :doc:`/codelists/BudgetIdentifier/` has different categories, and no 'sector' elements.
  * Names in the :doc:`/codelists/FileFormat/` list are no longer there as they make little sense, and the list now tracks the IANA source it is derived from directly.


