Codelist API
============

API Calls
^^^^^^^^^

To download a codelist. Select your endpoint (see below) and then specify the codelist name and the format:

<endpoint><codelist name>.<extension (xml/json/csv)>

Endpoints
^^^^^^^^^

The codelists used in each version of the standard are derived from different endpoints as a result of the historical management of the codelist API. We are finally taking in house control of them here at IATI.

Therefore anyone relying on the services at:

* http://datadev.aidinfolabs.org/data/, or
* http://data.aidinfolabs.org/data/

is strongly advised to migrate to the new endpoints given below. 

* v1.01 of the standard - uses datadev - change to http://codelists102.archive.iatistandard.org/data/
* v1.02 of the standard - uses datadev - change to - http://codelists102.archive.iatistandard.org/data/
* v1.03 of the standard - uses data - change to - http://codelists103.archive.iatistandard.org/data/

Codelists in Version 1.04 of the standard
-----------------------------------------

v1.04 of the standard - use either:

  * http://iatistandard.org/codelists/downloads/clv1/, or
  * Http://iatistandard.org/codelists/downloads/clv2/

In  v1.04 of the standard a new codelists structure has been introduced for those that want to take advantage of it's improved features (see below). We're calling this codelist version 2 (CLv2). This forms the 'single source of truth' from which codelists in the current/existing format (now known as codelist version 1, or CLv1) are derived.

To switch to the current versions of the codelists with the updates required for version 1.04 of the standard use http://iatistandard.org/codelists/downloads/clv1/ 
If you rely on the codelist API please read the notes on **Codelist API Compatibility in version 1.04 of the IATI Standard** below.

To switch to the new improved version (version 1.04 of the standard only) you can either:

1. Download the files using this endpoint http://iatistandard.org/codelists/downloads/clv2/, or
2. Work directly with GitHub to get the data (see below).

Working with GitHub Directly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The codelist source is now on GitHub:

- https://github.com/IATI/IATI-Codelists/tree/version-1.04/xml
- https://github.com/IATI/IATI-Codelists-NonEmbedded/tree/master/xml

We use this source to create all derived versions, (CSV, JSON and all forms of coldelist version 1 files, as well as all the documentation on the iatistandard.org website)

If you wish to use the new style XML, or are prepared to run the supplied python scripts for converting to a different format of your choice, you can fetch the codelists from GitHub directly.

Why create a new structure for codelists?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
As part of our move towards creating a :doc:`Single Source of Truth </developer/ssot/>` for the IATI Standard, we have started to take a different approach to codelists. See background paper previously circulated: https://docs.google.com/document/d/1oeH-8BFB__2IYF4MLnUwx2LcXZCVd5e-iYsXtQ4ViTk/edit

As this work progressed, it became evident that for the codelists to work in that environment we would need to make a few changes. As a result:

1. The newer codelist files are more consistent: 
 
 * they don't include the element name as a tag name
 * all have language information described the same way as IATI XML. 

2. There is also a codelist schema that all the source XML validates against - https://github.com/IATI/IATI-Codelists/blob/version-1.04/codelist.xsd.

3. Finally, more metadata, including a description, is now included in the codesists.

Codelist API Compatibility in version 1.04 of the IATI Standard
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If you wish to stay with the current codelist API system in 1.04 you will be able to do so, but there are a few things you should be aware of.

* The 'metadata' link/call is no longer available (instead, some of this is now available in the new style code lists, and some is stored in the github repository metadata to be consistent with the rest of the Single Source of Truth)
* Only the latest versions (those required in v1.04 of the standard) will be available through the API. If you need an older version use the static archives detailed above.
* URLs containing the version and/or language do not work. (for example in the past a url like: /data/codelist/AidTypeFlag/version/1.0/lang/en was possible. This will not work using the /codelists/downloads/clv1/ endpoint. Instead, translations, where available, are maintained in the codelist version 2 (CLv2) files.
* The 'fields' element is no longer provided in the index XML/JSON (See http://data.aidinfolabs.org/data/codelist.xml and compare with http://iatistandard.org/codelists/downloads/clv1/codelist.xml
* Version information is no longer provided in the XML.
* Specific changes to codelists:

  * :doc:`/codelists/BudgetIdentifier/` has different categories, and no 'sector' elements.
  * Names in the :doc:`/codelists/FileFormat/` list are no longer there as they make little sense, and the list now tracks the IANA source it is derived from directly.


