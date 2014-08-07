Standard Ruleset
================
The Standard Ruleset is a collection of rules that cover some of the basic requirements of the IATI Standard. It covers for example, the ordering of dates, and checks on the format of an iati-identifier. 

The ruleset consists of two types of rules:

* ``Starts with`` - conditions around the formation of the ``iati-identifier``
* ``Date order`` - logics around the ordering of various date elements.

These rules are applicable to various elements - as illustrated:

//iati-activity
===============

* ``iati-identifier`` should start with the value in ``reporting-org/@ref``

* ``activity-date[@type='start-actual']`` must be before ``activity-date[@type='end-actual']``

* ``activity-date[@type='start-planned']`` must be before ``activity-date[@type='end-planned']``

* ``activity-date[@type='start-actual']`` must be today, or in the past.

* ``activity-date[@type='end-actual']`` must be today, or in the past.


//transaction
=============

* ``transaction-date`` must be today, or in the past.

* ``value-date`` must be today, or in the past.


//planned-disbursement
======================

* ``period-start`` must be before ``period-end``


//result/indicator/period
=========================

* ``period-start`` must be before ``period-end``




Using the Standard Ruleset
--------------------------

Publishers are able to assess individual organisation and activity files with the Standard Ruleset via the IATI Validator tool.

Additionally, the IATI Dashboard checks all published data against the Standard Ruleset, and presents the results per publisher.
