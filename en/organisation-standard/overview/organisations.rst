Organisations
=============

Definition
----------
Within the IATI organisation standard three types of organisations can be declared:

* ``reporting-org`` - the organisation publishing the organisation file and associated data. 
* ``iati-organisation`` - the organisation that the data is about
* ``recipient-org`` - the organisation in reciept of budgets specificed in the data


Considerations
--------------
In many cases, an organisation file will contain information from the perspectitive of a single ``iati-organisation``.  Most commonly, this will be the same as the ``reporting-org``

However, it is possible for multiple ``iati-organisation`` to be reported.

``reporting-org`` and ``iati-organisation`` should include reference to their associated unique identifier - 

An ``iati-organisation`` can also include a ``name`` element - free text title of the organisation

Single or multiple ``recipient-org`` entries can be recorded.  

For each ``recipient-org`` multiple forward looking budgets can be recorded.


Further guidance
----------------

.. toctree::
   :titlesonly:
   :glob:
   
   organisation-standard/iati-organisations/iati-organisation/reporting-org/
   organisation-standard/iati-organisations/iati-organisation/iati-organisation/
   organisation-standard/iati-organisations/iati-organisation/name/
   organisation-standard/iati-organisations/iati-organisation/recipient-org-budget/
   


