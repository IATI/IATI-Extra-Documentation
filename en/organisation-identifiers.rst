Organisation Identifiers
========================

This guidance `draws from a
paper <https://docs.google.com/document/d/1o6ecOvr0_WA-hSLJ71dFw7cpYeC-fwGagkemty6fCbA/edit>`__
presented, discussed and consulted upon at the TAG meeting in May 2012.
However, this is currently draft guidance – subject to confirmation by
the Technical Advisory Group.

The IATI standard allows for the recording of information on all
organisations that participate in any part of the lifecycle of an aid
activity: inter alia donors, beneficiaries, extending and implementing
agencies.

Introduction
~~~~~~~~~~~~

Organisational identifiers have two uses in IATI.

-  They are used to identify organisations reporting activities,
   receiving funds, providing funds, or otherwise involved in activities
-  They form the basis of Activity Identifiers, who are composed of the
   reporting organisation Organisation ID, and an Activity ID.

Two components of IATI Org Identifiers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|image0|

The two components of IATI Organisation Identifiers

The IATI Organisational Identifier scheme is based on re-using existing
known identifiers for an organisation. Identifier strings consist of two
components:

#. The **namespace code** (a code that identifies a given organisational
   identifier registry)
#. The **base identifier** – re-use of an existing identifier from that
   namespace/registry

(1) and (2) are separated by a dash ‘-’.

The namespace code (1) may contain a dash ‘-’.

Worked example
~~~~~~~~~~~~~~

GB-COH is the `namespace code given by IATI
Support <https://docs.google.com/spreadsheet/ccc?key=0AnWngmdQt3stdFppMWdkcXJqVTRWTk9menR1N0FXNGc#gid=0>`__
to the UK Companies Registrar which issues numerical company identifiers
to legally constituted limited companies in the United Kingdom of Great
Britain and Northern Ireland. 06368740 is the company number (base
identifier) issued to Development Initiatives Poverty Research Limited.
Combining these we get an IATI Organisational Identifier of:
GB-COH-06368740

Sub-units
~~~~~~~~~

Where a registration scheme includes or allows separate identifiers for
sub-units (e.g. is able to refer to departments within an organisation),
then these may be included following a second ‘-’ delimiter. (e.g.
GB-COH-06368740-AidInfo)

Replacement considerations
~~~~~~~~~~~~~~~~~~~~~~~~~~

Where an existing base identifier contains ‘-’ (dash) then this should
be replaced with ‘\_’ (underscore).

Guidance on selecting the namespace or registration agency to use
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

An organisational identifier should:

#. **Use an existing registration number/identifier** that has been
   given to an organisation by an official registry of organisations
   (for example, a national company registrar, or drawn from a
   government register of charities). Registries that provide machine
   readable access to the data about organisations are generally
   preferred over those that do not (subject to (3) below).
#. **Use a namespace/registry code from the existing IATI list of
   namespaces and registration agency codes**. This is currently
   available at
   `http://bit.ly/iati-org-reg <http://bit.ly/iati-org-reg>`__ If no
   existing code is available then you should contact IATI Support with
   details of the registration agency you wish to re-use a code from in
   order to have a code set up. This list is currently maintained by the
   IATI secretariat over the short-term, with the hope that the wider
   open data community will adopt and develop a shared list of
   registration agency namespace codes in future.
#. **Where an organisation has multiple registration numbers, prefer
   those identifiers which uniquely pick out the organisation itself,
   rather than properties of the organisation**. For example, a VAT/Tax
   registration number describes that an entity is registered for tax,
   but may not map directly onto a single legal entity – as – for
   example – groups of companies may share a VAT registration number.
   For this reason, an identifier such as GB-COH-123456 would be
   preferred to GB-VAT-987765. If you are unsure of which registration
   agency to prefer, please consult IATI Support. If no authoritative
   registration agency information is currently collected (e.g. internal
   identifiers and supplier numbers are recorded, but no external
   identifiers) IATI publishers are encouraged to identify opportunities
   to collect an authoritative public identifier.
#. **Where an organisation is not identified in an official national
   registry, but it is identified in one of the recognised IATI
   Bi-lateral, Multi-lateral or INGO code lists, these codes should be
   used**. Multi-lateral and INGO numerical codes from these lists
   should be prefixed with DAC- The bi-lateral list (e.g. GB-1) will be
   deprecated in a future update of the standard and replaced with an
   official DAC provided code-list. In the meantime, non-prefixed
   bi-lateral code list values from IATIStandard.org can be used.
#. **Where none of the above provide an appropriate identifier,
   third-parties may provide appropriate lists of organisations**.
   Consult with IATI Support to identify appropriate identifier lists.
#. **Where no other identifiers are held or available, agree a registry
   code under ALT- with IATI Support for your organisation and use IDs
   within this namespace**. For example, if Development Initiatives were
   to only have internal supplier database identifiers for
   organisations, it could use codes of the form MISC-DEVINIT-123456. It
   would register MISC-DEVINIT with IATI Support, and ideally would
   provide some sort of reconciliation service to return the names and
   any additional information held that relates to each organisation ID.
#. **Where no identifier is held, make use of the @type attribute** to
   indicate the type of organisation (using the Organisation Type code
   list) and do not provide a @ref value.

Replacement patterns
~~~~~~~~~~~~~~~~~~~~

Where an existing base identifier contains ‘-’ (dash) then this should
be replaced with ‘\_’ (underscore).

Once determined, the organisational identity can be used in the @ref
attribute of reporting-org and participating-org, and should be used in
@ref attribute of transaction/provider-org and
transaction/recipient-org.

The string value name within any organisational identifier XML tag is
provided for convenience of consuming applications only, and should not
be treated as definitive.

.. |image0| image:: Organisational-ID-Diagrams.png
   :target: Organisational-ID-Diagrams.png
