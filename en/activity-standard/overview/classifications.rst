Classifications
===============

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI activity standard** it is expected that *classifications* information is provided for any ``iati-activity``

Namely:

* ``sector`` - the thematic catgory (or set of categories) an ``iati-activity`` operates with

Additionally, the following classifications enable the publication of various codes (often associated with CRS++ reporting)

* ``policy-marker``
* ``collaboration-type``
* ``default-finance-type``
* ``default-flow-type``
* ``default-aid-type``
* ``default-tied-status``


Considerations
--------------
When using the **IATI activity standard** to declare *documents*, the following should be considered:

* An ``iati-activity`` can have singlular or multiple ``sector`` 
* When multiple ``sector`` are described, then a ``percentage`` should be declared for each.  This should sum to 100% for each ``iati-activity``.
* A ``vocabulary`` can be declared when describing a ``sector``.  This should be on the ``Vocabulary`` codelist.
* If no ``vocabulary`` is declared, then the :doc:`DAC 5 digit codelist </codelists/Sector>` is assumed.
* A ``reporting-org`` can declare their own ``vocabulary``, via using the *RO* (Reporting Org) ``Vocabulary`` code.
* Multiple or singular ``policy-marker`` can also be described.  Unlike ``sector``, a percentage is not required.
* The classifications of ``default-finance-type``, ``default-flow-type``, ``default-aid-type`` and ``default-tied-status`` apply to the whole ``iati-activity``.  These can be overridden within a single ``transaction`` via using any of ``finance-type`` , ``flow-type`` , ``aid-type`` and/or ``tied-status``.

