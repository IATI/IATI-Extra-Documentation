Example Usage
~~~~~~~~~~~~~
Example declaring just the ``AidType`` code *A02*:

.. code-block:: xml

       <aid-type code="A02"/>
       
Additionally, a text description of the ``AidType`` code can be provided:

.. code-block:: xml

        <aid-type code="A02">Sector Budget Support</aid-type>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang``:

.. code-block:: xml

        <aid-type code="A02" xml:lang="fr">Soutien budgetaire sectoriel</aid-type>    
       
Full example:

.. code-block:: xml
    
    <transaction ref="1234">
      <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
      <transaction-type code="IF">Incoming Funds</transaction-type>
      <value currency="EUR" value-date="2012-01-01">1000</value>   
      <description>Transaction description text</description>
      <provider-org provider-activity-id="BB-BBB-123456789-1234AA" ref="BB-BBB-123456789">Agency B</provider-org>
      <receiver-org receiver-activity-id="AA-AAA-123456789-1234" ref="AA-AAA-123456789">Agency A</receiver-org>
      <aid-type code="A01">General budget support</aid-type>
      <flow-type code="10">ODA</flow-type>
      <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
      <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
      <tied-status code="3">Partially tied</tied-status>
    </transaction>
