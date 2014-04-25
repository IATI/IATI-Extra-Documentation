Organisation file
=================

Definition
----------
The *organisation file* contains the data that relates to the **IATI organisation standard**.

It is an XML file, containing all the relevant fields for the publisher organisation.

The **IATI organisation standard** allows publishers to report on information for multiple organisations: a government agency may report on behalf of other agencies; an INGO may report on behalf of its national associates; a private company may report on behalf of its subsidiaries.

Considerations
--------------
An IATI publisher should publish one organisation file.

It should be updated at least annually.

It must be valid XML.

A link to the organisation file should be published on the IATI Registry.  
Ideally, this link would be to an organisation file on the publisher website or open data portal.  However, third party tools are available to generate and host files on behalf of publishers.

The *organisation file* must have ``iati-organisations`` as the root element - to contain all other elements.

Further guidance
----------------

* :doc:`The organisation standard </organisation-standard/overview>`
* The IATI Registry
