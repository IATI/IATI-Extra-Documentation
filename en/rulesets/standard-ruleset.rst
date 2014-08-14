Standard Ruleset
================
The Standard Ruleset is a collection of rules that cover some of the basic requirements of the IATI Standard. It covers for example, the ordering of dates, and checks on the format of an iati-identifier. 

Using the Standard Ruleset
--------------------------

The current Standard Ruleset is applicable to a single ``iati-activity``.

Each test, detailed below, can be repeated within an ``iati-activity``, depending upon the scope and scale of elements of the **IATI Activity Standard** used.

For example, an activity with a single ``transaction`` would only be subject to two tests (detailed below).  For each and every time a ``transaction`` is repeated within an ``iati-activity``, these tests would be undertaken subsequently.  

Hence, the minimum and maximum number of tests undertaken on an ``iati-activity`` can fluctuate according to the content.

This could also be duplicated, if the tests are run on a single *IATI activity file*, which contains multiple ``iati-activity`` instances.

Contents of the Ruleset
-----------------------

The ruleset consists of two types of rules:

* ``Starts with`` - conditions around the formation of the ``iati-identifier``
* ``Date order`` - logics around the ordering of various date elements.

These rules are applicable to various elements:

