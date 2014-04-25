Activity file
=============

Definition
----------
The *activity file* contains the data that relates to the **IATI activity standard**.

It is an XML file, containing all the relevant fields for the publisher organisation.

Considerations
--------------
An IATI publisher should publish at least one activity file.

An activity file should contain at least one ``iati-activity``

It should be updated *at least* annually.

It must be valid XML.

A link to the activity file(s) should be published on the IATI Registry.  
Ideally, this link would be to an activity file(s) on the publisher website or open data portal.  However, third party tools are available to generate and host files on behalf of publishers.

The *activity file* must have ``iati-activities`` as the root element - to contain all other elements.

Further guidance
----------------

Reference pages:

* :doc:`summary-table </activities-standard/summary-table/>`
* :doc:`iati-activities </activities-standard/iati-activities/>`
* :doc:`iati-activity </activities-standard/iati-activities/iati-activity/>`
