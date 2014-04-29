Organisation file
=================

Definition
----------
The *organisation file* contains the data that relates to the **IATI organisation standard**.

| It is an XML file, containing all the relevant **IATI organisation standard** fields for the publishing organisation.

| The **IATI organisation standard** allows publishers to report on information for multiple organisations: a government agency may report on behalf of other agencies; an INGO may report on behalf of its national associates; a private company may report on behalf of its subsidiaries.

Considerations
--------------
When using the **IATI organisation standard** to produce the *organisation file*, the following should be considered:

* An IATI publisher should publish one *organisation file*.

* An *organisation file* should contain at least one ``iati-organisation``

* It should be updated at least annually.

* It must be valid XML.

* The *organisation file* must have ``iati-organisations`` as the root element - to contain all other elements.

* The ``generated-datetime`` attribute of ``iati-organisations`` - a date/time stamp for when this *activity-file* was generated - is highly recommended.

* A link to the organisation file should be published on the **IATI Registry**.  

* Ideally, this link would be to an *organisation file* on the publisher website or open data portal.  However, third party tools are available to generate and host files on behalf of publishers.

* When creating the *organisation file* it is recommended to avoid spaces and non-ascii characters in file names and urls.  For example: 

** ``iatiorganisation.xml`` is preferable to ``IATI Organisation.xml``  

** ``http://example.org/files/iatidata/iatiorganisation.xml`` is preferable to ``http://example.org/files/iati data/IATI Organisation.xml``.


Further guidance
----------------

* :doc:`The organisation standard </organisation-standard/overview>`
* The IATI Registry
