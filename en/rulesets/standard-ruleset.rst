Standard Ruleset
================
The Standard Ruleset is a collection of rules that cover some of the basic requirements of the IATI Standard. It covers for example, the ordering of dates, and checks on the format of an iati-identifier. 

Using the Standard Ruleset
^^^^^^^^^^^^^^^^^^^^^^^^^^

The current Standard Ruleset is applicable to a single ``iati-activity`` or ``iati-organisation``.

Each test, detailed below, can be repeated within an ``iati-activity`` (or ``iati-organisation``), depending upon the scope and scale of elements of the **IATI Activity Standard** (or **IATI Organisation Standard**) used.

For example, an activity with a single ``transaction`` would only be subject to two tests (detailed below).  For each and every time a ``transaction`` is repeated within an ``iati-activity``, these tests would be undertaken subsequently.  

Hence, the minimum and maximum number of tests undertaken on an ``iati-activity`` or ``iati-organisation`` can fluctuate according to the content.

This could also be duplicated, e.g. if the tests are run on a single *IATI activity file*, which contains multiple ``iati-activity`` instances.

Non-Machine Readable Rules
^^^^^^^^^^^^^^^^^^^^^^^^^^

(these are defined on this page)

reporting-org/\@ref
-------------------

* The agency prefix MUST be a valid code in the IATI code list
* The identifier MUST be the same as that recorded by the publisher on the IATI Registry

iati-identifier
---------------

* It MUST be globally unique among all activities published through the IATI Registry
* Once an activity has been reported to IATI its identifier MUST NOT be changed in subsequent updates
* It MUST be prefixed with EITHER the organisation identifier found in ``reporting-org/@ref`` OR a previous ``reporting-org identifier`` reported in ``other-identifier``

budget
------

* The budget element should be repeated for each year of the activity's duration
* Each budget should cover a period no longer than 1 year

Machine Readable Rules
^^^^^^^^^^^^^^^^^^^^^^

(these are defined in a JSON file that can be consumed programatically, but are also displayed here)
