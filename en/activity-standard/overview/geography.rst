Geography
=========

Definition
----------
Within the **IATI activity standard** there are three ways to describe the *geography* of an ``iati-activity``:

* ``recipient-country`` - the country that will benefit from the ``iati-activity``.
* ``recipient-region`` - geopolitical region (above the country level) that will benefit from the ``iati-activity``.
* ``location`` - a geographical location of the ``iati-activity``.

In addition, the following can also be utilised:

* ``activity-scope`` - to classify the geographic coverage of the the ``iati-activity``.


Considerations
--------------
When using the **IATI activity standard** to describe *geography*, the following should be considered:

* When describing the ``recipient-country`` the relevant *Country* code must be used.
* When describing the ``recipient-region`` the relevant *Region* code must be used.
* It is possible to have multiple ``recipient-country`` in an ``iati-activity``
* It is possible to have multiple ``recipient-region`` in an ``iati-activity``
* When declaring multiple ``recipient-country`` or ``recipient-region`` then a ``@pecentage`` must be declared.  These must sum to 100%.
* If a ``recipient-country`` is known, then a ``recipient-region`` is not expected.
* If a ``recipient-country`` is not known, then a ``recipient-region`` is expected.
* The ``activity-scope`` element should only be used once.  It must use a relevant *ActivityScope* code.


2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* It is not desirable to include the freetext name of any ``recipient-country`` or ``recipient-region``.  Only in exceptional circumstances - where the publishing organisation **must** provide different text to the name on the relevant *Country* or *Region* codelist.
* It is feasible to have both a ``recipient-country`` and ``recipient-region`` in the same ``iati-activity``.  In such cases, the ``@percentage`` must be declared, and sum to 100 across both elements.
* Both a ``recipient-country`` and ``recipient-region`` can also be published as child elements of a ``transaction``.  When this is done, it is expected that **all** ``transaction`` include such data, whilst the relevant element is subsequently **not** included at the ``iati-activity`` level.
