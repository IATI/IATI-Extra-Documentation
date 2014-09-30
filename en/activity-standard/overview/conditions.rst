Conditions
==========

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI activity standard** conditions that relate to an ``iati-activity`` can be described:

* ``conditions`` - a container element to declare whether ``condition`` are attached.
* ``condition`` - the specific statement around a condition.


Considerations
--------------
When using the **IATI activity standard** to declare *conditions*, the following should be considered:

* An ``iati-activity`` does not require a ``conditions`` statement, if none are relevant.
* However, it is also valid to declare that no ``conditions`` are attached to a specific ``iati-activity`` via the ``attached`` attribute.
* For every ``condition`` a relevant ``ConditionType`` code is expected.
* When multiple ``condition`` exist, these can be presented separately within the same ``conditions`` element.
* The same ``condition`` can be presented in different languages via separate ``condition`` elements, using ``xml:lang``.
* The free-text to describe the condition should avoid jargon



