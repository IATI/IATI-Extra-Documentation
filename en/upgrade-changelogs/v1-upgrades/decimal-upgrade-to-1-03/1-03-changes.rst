1.03 Changes
============

Changes / Additions to IATI Standard for version 1.03

Schema Changes
--------------

Activities schema
~~~~~~~~~~~~~~~~~

Updated elements:

-  Version numbers now included in the document root. Versions match the
   version of the standard, not the document, although documents will
   only change in line with the standard.

-  added the
   optional \ `contact-info <http://iatistandard.org/activity-standard/contact-info/>`__/website
   element

-  added the
   optional \ `contact-info <http://iatistandard.org/activity-standard/contact-info/>`__/@type
   attribute

-  added the
   optional \ `contact-info <http://iatistandard.org/activity-standard/contact-info/>`__/job-title
   element

-  changed the following subelements
   of \ `contact-info <http://iatistandard.org/activity-standard/contact-info/>`__ to
   allow multiple-language versions explicitly (no change to parsing;
   purely semantic): organisation, person-name, job-title,
   mailing-address

-  added
   optional \ `recipient-region <http://iatistandard.org/activity-standard/recipient-region/>`__\ n/@vocabulary
   attribute

-  globally changed the @percentage attribute to allow decimals (e.g.
   ``55.5`` as well as ``50``)

-  globally changed the @currency attribute to allow decimals (e.g.
   ``99.99`` as well as ``99``)

-  added the
   optional \ `country-budget-item <http://iatistandard.org/activity-standard/country_budget_items/>`__ element

-  added the
   optional \ `capital-spend <http://iatistandard.org/activity-standard/capital_spend/>`__ element

-  added the
   optional \ `crs-add <http://iatistandard.org/activity-standard/crs-add/>`__ element
   and its child elements

-  added
   the \ `activity-scope <http://iatistandard.org/activity-standard/activity-scope/>`__ element

-  added the
   optional \ `fss <http://iatistandard.org/activity-standard/fss/>`__ element
   and its child elements

Organisation schema
~~~~~~~~~~~~~~~~~~~

-  Version numbers now included in the document root. Versions match the
   version of the standard, not the document, although documents will
   only change in line with the standard.

-  globally changed the @currency attribute to allow decimals (e.g.
   ``99.99`` as well as ``99``)

Common schema
~~~~~~~~~~~~~

-  Version numbers now included in the document root. Versions match the
   version of the standard, not the document, although documents will
   only change in line with the standard.

-  Currency values are now allowed to be declared as decimals instead of
   integers.

-  Moved the @percentage attribute to common, so that it can be reused.

Registry Record schema
~~~~~~~~~~~~~~~~~~~~~~

-  Version numbers now included in the document root. Versions match the
   version of the standard, not the document, although documents will
   only change in line with the standard.

Codelist Changes
----------------

New Codelists
~~~~~~~~~~~~~

-  Activity Scope
   `http://iatistandard.org/codelists/activity\_scope/ <http://iatistandard.org/codelists/activity_scope/>`__

-  Aid Type Flag
   `http://iatistandard.org/codelists/aid-type-flag/ <http://iatistandard.org/105/codelists/aid-type-flag/>`__

-  Budget Identifier
   `http://iatistandard.org/codelists/budget\_identifier/ <http://iatistandard.org/codelists/budget_identifier/>`__

-  Budget Identifier
   Vocabulary\ `http://iatistandard.org/codelists/budget\_identifier\_vocabulary/ <http://iatistandard.org/codelists/budget_identifier_vocabulary/>`__

-  | Contact Type `http://iatistandard.org/codelists/contact-type/ <http://iatistandard.org/codelists/contact-type/>`__
   | Loan Repayment Period `http://iatistandard.org/codelists/loan-repayment-period/ <http://iatistandard.org/codelists/loan-repayment-period/>`__

-  Loan Repayment Type
   `http://iatistandard.org/codelists/loan-repayment-type/ <http://iatistandard.org/codelists/loan-repayment-type/>`__

-  Region Vocabulary
   `http://iatistandard.org/codelists/region-vocabulary/ <http://iatistandard.org/codelists/region-vocabulary/>`__

Updated Codelists
~~~~~~~~~~~~~~~~~

-  Document Category
   `http://iatistandard.org/codelists/document\_category/ <http://iatistandard.org/codelists/document_category/>`__

-  Condition Type
   `http://iatistandard.org/codelists/condition\_type/ <http://iatistandard.org/codelists/condition_type/>`__

-  Collaboration Type
   `http://iatistandard.org/codelists/collaboration\_type/ <http://iatistandard.org/codelists/collaboration_type/>`__

-  Flow Type
   `http://iatistandard.org/codelists/flow\_type/ <http://iatistandard.org/codelists/flow_type/>`__
