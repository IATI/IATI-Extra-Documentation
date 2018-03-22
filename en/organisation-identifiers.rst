Organisation Identifiers
========================

The **IATI standard** allows for the recording of information on all *organisations* that participate in any part of the lifecycle of an aid activity: inter alia donors, beneficiaries, extending and implementing agencies.

Crucial to this, is a common process through which to identify and declare identifiers for these organisations.


Introduction
~~~~~~~~~~~~
*Organisational identifiers* have two uses in IATI.

In the **IATI organisation standard**:

* They are used to identify organisations as reporting organisations (``reporting-org``), as receiving budgets (``recipient-org``), and of course as an ``iati-organisation``.
* They form the ``iati-identifier`` - used to declare a globally unique identifier for the specific ``iati-organisation``

In the **IATI activity standard**:

* They are used to identify organisations as reporting organisations (``reporting-org``), receiving funds (``receiver-org``), providing funds (``provider-org``), or otherwise involved in ``iati-activities`` (using ``participating-org``)
* They form the basis of the ``iati-identifier`` - used to declare a globally unique activity identifier for the specific ``iati-activity``  - composed of the reporting organisation Organisation ID, and an Activity ID.


Two components of IATI Organisation Identifiers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|image0|

The two components of **IATI Organisation Identifiers**

The **IATI Organisational Identifier** scheme is based on re-using existing known identifiers for an *organisation*. 

Identifier strings consist of two components:

#. The **namespace code** - a code that creates and maintains a given organisational identifier registry
#. The **base identifier** – re-use of an existing identifier from that namespace/registry

1 and 2 are separated by a dash ``-``.

The namespace code (1) may contain a dash ``-``.


Worked example
~~~~~~~~~~~~~~
``GB-COH`` is the **namespace code** to the UK Companies Registrar which issues numerical company identifiers to legally constituted limited companies in the United Kingdom of Great Britain and Northern Ireland:

* `Companies House. <http://www.companieshouse.gov.uk/>`__.

``06368740`` is the company number (base identifier) issued to Development Initiatives Poverty Research Limited. 

* `Development Initiatives Poverty Research Limited record on Companies House. <http://data.companieshouse.gov.uk/doc/company/06368740>`__. 

Combining these we get an **IATI Organisational Identifier** of: ``GB-COH-06368740``


Organisation Registration Agencies
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
To assist with creating and de-referencing **IATI Organisation Identifiers**, the codelist :doc:`/codelists/OrganisationRegistrationAgency` is available.

This codelist provides the **namespace** codes for a number of Registration Agencies.  This list is non-embedded in the **IATI Standard**, which means changes and additions may be made at short notice, outside of published decimal and integer upgrade schedules. If a Registation Agency that you wish to use is not on this list, please contact support@iatistandard.org.


Guidance on selecting an Organisation Registration Agencies (namespace)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
An **IATI Organisation Identifier** should:

* **Use an existing registration number/identifier** that has been given to an organisation by an official registry of organisations (for example, a national company registrar, or drawn from a government register of charities). Registries that provide machine readable access to the data about organisations are generally preferred over those that do not (subject to (3) below).

* **Use a namespace/registry code from the existing IATI list of namespaces and registration agency codes**. This is currently available as :doc:`a codelist <codelists/OrganisationRegistrationAgency/>`. If no existing code is available then you should contact IATI Support with details of the registration agency you wish to re-use a code from in order to have a code set up.
 
* **Where an organisation has multiple registration numbers, prefer those identifiers which uniquely pick out the organisation itself, rather than properties of the organisation**. For example, a VAT/Tax registration number describes that an entity is registered for tax, but may not map directly onto a single legal entity – as – for example – groups of companies may share a VAT registration number. For this reason, an identifier such as ``GB-COH-123456`` would be preferred to ``GB-VAT-987765``. 

* **Where an organisation is not identified in an official national registry, but it is identified on the (deprecated since v1.04 of the standard) ``OrganisationIdentifier`` codelist, these codes should be used as given.**.

* **Where none of the above provide an appropriate identifier, third-parties may provide appropriate lists of organisations**.  Consult with IATI Support to identify appropriate identifier lists.

* **Where no other identifiers are held or available**, please contact IATI support.

If you are unsure of which registration agency to prefer, please consult IATI Support. If no authoritative registration agency information is currently collected (e.g. internal identifiers and supplier numbers are recorded, but no external identifiers) IATI publishers are encouraged to identify opportunities to collect an authoritative public identifier.


Example Usage
~~~~~~~~~~~~~

Once determined, the **IATI Organisational Identifier** can be used:

* **IATI organisation standard**: as the ``iati-identifier``, in the ``@ref`` attribute of ``reporting-org`` and ``recipient-org-budget/recipient-org``.

* **IATI activity standard**: in the ``@ref`` attribute of ``reporting-org`` and ``participating-org``, and should be used in ``@ref`` attribute of ``transaction/provider-org`` and ``transaction/recipient-org``.

The string value name within any organisational identifier XML tag is provided for convenience of consuming applications only, and should not be treated as definitive.

.. |image0| image:: Organisational-ID-Diagrams.png
   :target: Organisational-ID-Diagrams.png
