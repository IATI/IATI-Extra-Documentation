IATI Activity
=============

Definition
----------
An ``iati-activity`` a distinct grouping of data that collects and describes various facts of an "activity".


Considerations
--------------
Every ``iati-activity`` must have a globally unique ``iati-identifier``

Publishers can decide on how best to structure and segment their organisation around ``iati-activity``

It is possible to link different ``iati-activity`` via one or multiple of:

* ``hierarchy`` groupings can be used to structure one or many ``iati-activity`` within a specific organisation. 
* ``related-activity`` can express activities that have parental or sibling linkages.
* via ``transactions``, monies can be linked together, with a specific ``iati-activity`` being quoted.

A publisher can set a default language and currency, that is then used throughout the ``iati-activity``.  This can be overriden in at any point however.


Further guidance
----------------

