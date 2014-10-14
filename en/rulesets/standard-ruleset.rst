Standard Ruleset
================
The Standard Ruleset is a collection of rules that cover some of the basic requirements of the IATI Standard. Typically, these are rules about the data that cannot be enforced by the schema alone. It covers for example, the ordering of dates, and checks on the format of an iati-identifier.

Each rule is constructed to be something that a human should be able to understand.

Some rules are constructed in such a way that a computer could both read the rule, and then check that the rule applies, although software may need to be written to perform achieve this. For example a computer can check that dates have been supplied, and that one is earlier in time than the other. A computer cannot really usefully check that 'a title is meaningful'. 

Therefore we can split the Standard Ruleset into Machine Readable and Non-Machine Readable Rules

Using the Standard Ruleset
^^^^^^^^^^^^^^^^^^^^^^^^^^

The current Standard Ruleset is a collection of rules that can be used to test the data in a single ``iati-activity`` or ``iati-organisation`` record.
IATI data is often found as large files containing collections of (for example) activiites, so to test a file of IATI data against the Standard Ruleset means running the tests on each ``iati-activity`` or ``iati-organisation`` record in that file.

Every ``iati-activity`` or ``iati-organisation`` record has the option to use different elements of the IATI Standard, and to also repeat certain elements, so in defining a Standard Ruleset it is necessary to include rules that may or may not need to apply for each individual ``iati-activity`` or ``iati-organisation`` record.

If we take a ``transaction`` from an ``iati-activity`` record as an example, we can see that this element does not have to be reported. However, it may also be reported many times. There are rules in the Standard Ruleset to check that some of the data reported in transactions makes sense, so these tests could either be run many times, or not at all on a single ``iati-activity`` record. 

Hence, the minimum and maximum number of tests undertaken on an ``iati-activity`` or ``iati-organisation`` can fluctuate according to the content.

Non-Machine Readable Rules
^^^^^^^^^^^^^^^^^^^^^^^^^^

reporting-org/\@ref
-------------------

* The agency prefix MUST be a valid code in the IATI code list
* The identifier MUST be the same as that recorded by the publisher on the IATI Registry

participating-org/\@ref
-----------------------

* When using this attribute, it must be a valid organisation identifier.

transaction/provider-org/\@ref
------------------------------

* When using this attribute, it must be a valid organisation identifier.

transaction/receiver-org/\@ref
------------------------------

* When using this attribute, it must be a valid organisation identifier.

iati-identifier
---------------

* It MUST be globally unique among all activities published through the IATI Registry
* Once an activity has been reported to IATI its identifier MUST NOT be changed in subsequent updates
* It MUST be prefixed with EITHER the organisation identifier found in ``reporting-org/@ref`` OR a previous ``reporting-org identifier`` reported in ``other-identifier``

budget
------

* The budget element should be repeated for each year of the activity's duration
* Each budget should cover a period no longer than 1 year

sector
------

* Sector MUST be reported at either activity level or transaction level but not both
* At transaction level, only one sector per vocabulary should be reported

recipient-country and recipient-region
--------------------------------------

* Either recipient-country or recipient-region MUST be reported at activity level or transaction level but not both.


Machine Readable Rules
^^^^^^^^^^^^^^^^^^^^^^

These rules are defined in a `JSON file <https://github.com/IATI/IATI-Rulesets/blob/version-2.01/rulesets/standard.json>` as part of our :doc:`Single Source of Truth </developer/ssot/>` that can be consumed programatically. The list below has been generated from that source.
