Organisations
=============

Definition
----------
Within the IATI organisation standard three types of organisations can be declared:

* ``reporting-org`` - the organisation publishing the organisation file and associated data. 
* ``iati-organisation`` - the organisation that the data is about
* ``recipient-org`` - the organisation in receipt of budgets specified in the data


Considerations
--------------
In many cases, an organisation file will contain information from the perspective of a single ``iati-organisation``.  Most commonly, this will be the same as the ``reporting-org``

However, it is possible for multiple ``iati-organisation`` to be reported.

``reporting-org`` and ``iati-organisation`` should include reference to their associated unique identifier - 

An ``iati-organisation`` can also include a ``name`` element - free text title of the organisation

Single or multiple ``recipient-org`` entries can be recorded.  

For each ``recipient-org`` multiple forward looking budgets can be recorded.


Further guidance
----------------

* :doc:`reporting-org </organisation-standard/iati-organisations/iati-organisation/reporting-org/>`
* :doc:`iati-organisation </organisation-standard/iati-organisations/iati-organisation/>`
* :doc:`name </organisation-standard/iati-organisations/iati-organisation/name/>`
* :doc:`recipient-org-budget </organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/>`
   


