Result
======

Definition
----------
The **IATI activity standard** enables the publishing of information on measurable results from an ``iati-activity``, through use of the ``result`` element via: 

* ``result`` - a container for reporting outputs, outcomes, impacts and other results that stem directly from the ``iati-activity``.

 
Considerations
--------------
When using the **IATI activity standard** to declare *result*, the following should be considered:

* Any ``iati-activity`` can have multiple ``result`` elements.
* A ``result`` must have a ``title`` and should include a ``description`` to clarify the information being detailed.
* Every ``result`` must include an ``indicator``, which in turn details a period of time, and then a ``target`` and ``actual`` measure.
* An ``indicator`` must have a ``title`` and should include a ``description`` to clarify the information being detailed.
* An ``indicator`` can be repeated within any ``result``.
* It is also recommended to include a ``baseline`` measure for each ``result`` recorded.
* Any ``target``, ``actual`` and ``baseline`` can have attached a ``comment`` to provide additional narrative or information.
* The free-text instances of ``title``, ``description`` and ``comment`` can be repeated for multiple languages, using ``@xml:lang``.
* The free-text instances of ``title``, ``description`` and ``comment`` should avoid use of text in CAPITALS, where possible. 

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* Any freetext title, description or comment must be included in the child ``narrative`` element, which can be repeated for different languages. 
