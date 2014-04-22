Example Usage
~~~~~~~~~~~~~
Example of ``transaction-type`` declaring just ``TransactionType`` code *IF* (Incoming Funds)

.. code-block:: xml

        <transaction-type code="IF">Incoming Funds</transaction-type>

Additionally, a text description of the ``TransactionType`` code can be provided:

.. code-block:: xml

        <transaction-type code="IF">Incoming Funds</transaction-type>

Where this text description is in a language that differs from the default, then this should be declared accordingly:

.. code-block:: xml

        <transaction-type code="IF" xml:lang="en">Incoming Funds</transaction-type>
        
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
