Organisations
=============

Definition
----------
Within the **IATI organisation standard** three types of *organisations* can be declared:

* ``reporting-org`` - the organisation publishing the data help within the *organisation file*. 
* ``iati-organisation`` - the organisation that the data is about
* ``recipient-org`` - the organisation in receipt of budgets specified in ``recipient-org-budget``


Considerations
--------------
When using the **IATI organisation standard** to declare *organisations*, the following should be considered:

* In many cases, an *organisation file* will contain information from the perspective of a single ``iati-organisation``.  Most commonly, this will be the same as the ``reporting-org``

* However, it is possible for multiple ``iati-organisation`` to be described in a single *organisation file*.

* ``reporting-org`` and ``iati-organisation`` should include reference to their associated unique ``iati-identifier``

* For ``reporting-org``, inclusion of the ``OrganisationType`` code is recommended.

* An ``iati-organisation`` can also include a ``name`` element - free text title of the organisation

* Single or multiple ``recipient-org`` entries can be recorded.

* For each ``recipient-org`` multiple forward looking ``recipient-org-budget`` can be recorded.


Further guidance
----------------

* :doc:`reporting-org </organisation-standard/iati-organisations/iati-organisation/reporting-org/>`
* :doc:`iati-organisation </organisation-standard/iati-organisations/iati-organisation/>`
* :doc:`name </organisation-standard/iati-organisations/iati-organisation/name/>`
* :doc:`recipient-org-budget </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/>`
   


