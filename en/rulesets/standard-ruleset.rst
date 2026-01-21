################
Standard Ruleset
################

The Standard Ruleset is a collection of rules that complement the `IATI XML Schemas <https://github.com/IATI/IATI-Schemas>`_. Between them, they assess most of the requirements of the IATI Standard. The Standard Ruleset provides rules about the data that cannot be enforced by schema. For example, they include the ordering of dates, percentages adding to 100, and checks on the format of an iati-identifier.

Some aspects of the IATI Standard cannot be assessed automatically, such as "Is a title meaningful?". These rules are outside of the scope of the IATI XML Schemas and the Standard Rulesets, and should be assessed manually as part of publication. 

The `IATI Validator <http://validator.iatistandard.org>`_ uses these rules to programmatically validate IATI files. The code used to interpret these rules and validate an IATI file are part of the validator GitHub repository `IATI/js-validator-api <https://github.com/IATI/js-validator-api>`_.

Any errors, omissions or bugs should be reported via `GitHub <https://github.com/IATI/IATI-Rulesets/issues>`_ or to `IATI Support <https://iatistandard.org/en/contact/>`_


Using the Standard Ruleset
***************************
The Standard Ruleset is a collection of rules that can be used to test the data in a single ``iati-activity`` or ``iati-organisation`` .

IATI data is often found as large files containing collections of (for example) activities, so to test a file of IATI data against the Standard Ruleset means running the tests on each ``iati-activity`` or ``iati-organisation``  in that file.

Every ``iati-activity`` or ``iati-organisation``  has the option to use different elements of the IATI Standard, and to also repeat certain elements, so in defining a Standard Ruleset it is necessary to include rules that may or may not need to apply for each individual ``iati-activity`` or ``iati-organisation`` .

If we take a ``transaction`` from an ``iati-activity``  as an example, we can see that this element does not have to be reported. However, it may also be reported many times. There are rules in the Standard Ruleset to check that some of the data reported in transactions makes sense, so these tests could either be run many times, or not at all on a single ``iati-activity`` . 

Hence, the number of tests undertaken on an ``iati-activity`` or ``iati-organisation`` can vary according to the content.

Relationship to the IATI Standard
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Where the standard says that something MUST be the case, these are defined in the Standard Ruleset as rules, which will produce an Error if the condition is not met. 

Where the standard says that something SHOULD be the case, these are defined in the Standard Ruleset as guidance, which will produce a Warning if the condition is not met. 


Full list of IATI Rules
^^^^^^^^^^^^^^^^^^^^^^^

The full list of IATI rules are defined in a `JSON file <https://github.com/IATI/IATI-Rulesets/blob/version-2.03/rulesets/standard.json>`_ as part of our `Single Source of Truth <https://iatistandard.org/en/guidance/developer/ssot/>`_ that can be consumed programmatically. The list below has been generated from that source. You can see the error/warning message in plain English and also an id link that would direct you to the source JSON. You will see in the JSON file there that there is a severity reference. 

