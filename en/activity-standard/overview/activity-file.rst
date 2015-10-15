Activity file
=============

Definition
----------
The *activity file* contains the data defined by the **IATI activity standard**.

It is an XML file, containing the relevant **IATI activity standard** fields for the publishing organisation.


Considerations
--------------
When using the **IATI activity standard** to produce an *activity-file*, the following should be considered:

* An IATI publisher should publish at least one activity file.
* An activity file should contain at least one ``iati-activity``
* It should be updated at least annually.
* It must be :doc:`well-formed XML </key-considerations/structured>`.
* It must validate against the relevant version of the :doc:`IATI activity schema </schema/>` 
* Any *activity file* must have ``iati-activities`` as the root element - to contain all other elements.
* The ``generated-datetime`` attribute of ``iati-activities`` - a date/time stamp for when the *activity-file* was generated - is highly recommended. 
* The ``generated-datetime`` is declared at the ``iati-activities`` level.  Is not necessarily the same as the ``last-updated-datetime`` for the individual ``iati-activity`` records within it.
* Across a set of *activity files* published by a single organisation, individual ``iati-activity``, referenced via a unique ``iati-identifier``, should not be duplicated.
* A link to the activity file(s) should be published on the **IATI Registry**.
* Ideally, this link would be to an activity file(s) on the publisher website or open data portal.  However, third party tools are available to generate and host files on behalf of publishers.
* When creating the *activity file* it is recommended to avoid spaces and non-ascii characters in file names and urls.  For example:
	* ``iatiactivity.xml`` is preferable to ``IATI Activity.xml``.  
	* ``http://example.org/files/iatidata/iatiactivity.xml`` is preferable to ``http://example.org/files/iati data/IATI Activity.xml``.


2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* It is recommended that a single *activity-file* does not exceed 40MB in file size.
* Data publishers are encouraged to segment their data into 'meaningful chunks'. Prior to version 2.01 they were encouraged to segment their data by country and/or regions. This is no longer necessarily considered to be best practice.
* The order of the elements presented in an *activity-file* must follow the order set out in the schema.
* The version of the IATI standard being used must be declared via the ``version`` attribute of the ``iati-activities`` element.  This must be a valid value on the *Version* codelist.

Further Guidance 
----------------
* For *well-formed XML* tests, see the `W3C XML Validator <http://www.w3schools.com/xml/xml_validator.asp>`_

* The `IATI Validator <http://validator.iatistandard.org/>`_ tests data against the relevant version of the **IATI activity schema**.
