################
Standard Ruleset
################
The Standard Ruleset is a collection of rules that cover most of the requirements of the IATI Standard and that a computer could, in principle, test. Typically, these are rules about the data that cannot be enforced by the IATI schema alone. It covers for example, the ordering of dates, percentages adding to 100, checks on the format of an iati-identifier and others.

We have created a generic framework that allows us to express many of these rules in a way that machines can understand and humans can interpret by reading a simple error message.

The IATI Validator V2 uses these rules to programmatically validate IATI files. The code used to interpret these rules and validate an IATI file are part of the validator GitHub repository `IATI/js-validator-api <https://github.com/IATI/js-validator-api>`_.

There are some things given in definitions of elements that really only a human can interpret, such as "Is a title meaningful?". The Standard Ruleset does not even try to deal with cases such as this. 


Using the Standard Ruleset
***************************
The current Standard Ruleset is a collection of rules that can be used to test the data in a single ``iati-activity`` or ``iati-organisation`` record.

IATI data is often found as large files containing collections of (for example) activities, so to test a file of IATI data against the Standard Ruleset means running the tests on each ``iati-activity`` or ``iati-organisation`` record in that file.

Every ``iati-activity`` or ``iati-organisation`` record has the option to use different elements of the IATI Standard, and to also repeat certain elements, so in defining a Standard Ruleset it is necessary to include rules that may or may not need to apply for each individual ``iati-activity`` or ``iati-organisation`` record.

If we take a ``transaction`` from an ``iati-activity`` record as an example, we can see that this element does not have to be reported. However, it may also be reported many times. There are rules in the Standard Ruleset to check that some of the data reported in transactions makes sense, so these tests could either be run many times, or not at all on a single ``iati-activity`` record. 

Hence, the minimum and maximum number of tests undertaken on an ``iati-activity`` or ``iati-organisation`` can fluctuate according to the content.


Full list of IATI Rules
^^^^^^^^^^^^^^^^^^^^^^^

The full list of IATI rules are defined in a `JSON file <https://github.com/IATI/IATI-Rulesets/blob/version-2.02/rulesets/standard.json>`_ as part of our `Single Source of Truth <https://iatistandard.org/en/guidance/developer/ssot/>`_ that can be consumed programmatically. The list below has been generated from that source. You can see the error/warning message in plain English and also an id link that would direct you to the source JSON. You will see in the JSON file there that there is a severity reference. All MUST statements are defined as errors (rules) and all SHOULD statement are defined as warnings (recommended guidance).
