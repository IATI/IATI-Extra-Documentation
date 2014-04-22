Example Usage
~~~~~~~~~~~~~
The ``transaction`` element acts as a container for other sub elements.

At the ``transaction level, the attribute ``ref`` can be used to describe reference to this ``transaction`` in another system:

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

Example:

.. code-block:: xml

    <transaction ref="1234">
      <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
      <transaction-type code="IF">Incoming Funds</transaction-type>
      <value currency="EUR" value-date="2012-01-01">1000</value>   
      <description>Transaction description text</description>
      <provider-org provider-activity-id="BB-BBB-123456789-1234AA" ref="BB-BBB-123456789">Agency B</provider-org>
      <receiver-org receiver-activity-id="AA-AAA-123456789-1234" ref="AA-AAA-123456789">Agency A</receiver-org>
    </transaction>

Full example with additional elements, some of which can override the value set in ``iati-activity``: 

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
    
An ``iati-activity`` can have multiple ``transaction`` elements:

.. code-block:: xml

    <transaction ref="XYZ">
      <aid-type code="A01">General budget support</aid-type>
      <flow-type code="10">ODA</flow-type>
      <provider-org provider-activity-id="BB-BBB-123456789-1234" ref="BB-BBB-123456789">Agency B</provider-org>
      <receiver-org receiver-activity-id="CC-CCC-123456789-1234" ref="CC-CCC-123456789">Agency C</receiver-org>
      <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
      <value currency="EUR" value-date="2012-01-31">1000</value>
      <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
      <tied-status code="3">Partially tied</tied-status>
      <transaction-date iso-date="2012-01-31">2012-01-31</transaction-date>
      <transaction-type code="C">Commitment</transaction-type>
      <description>Description text</description>
    </transaction>
    <transaction ref="ABC">
      <aid-type code="A01">General budget support</aid-type>
      <flow-type code="10">ODA</flow-type>
      <provider-org provider-activity-id="BB-BBB-123456789-1234" ref="BB-BBB-123456789">Agency B</provider-org>
      <receiver-org receiver-activity-id="CC-CCC-123456789-1234" ref="CC-CCC-123456789">Agency C</receiver-org>
      <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
      <value currency="EUR" value-date="2012-01-01">1000</value>
      <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
      <tied-status code="3">Partially tied</tied-status>
      <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
      <transaction-type code="C">Commitment</transaction-type>
      <description>Description text</description>
    </transaction>
    <transaction ref="1234">
      <aid-type code="A01">General budget support</aid-type>
      <flow-type code="10">ODA</flow-type>
      <provider-org provider-activity-id="BB-BBB-123456789-1234AA" ref="BB-BBB-123456789">Agency B</provider-org>
      <receiver-org receiver-activity-id="AA-AAA-123456789-1234" ref="AA-AAA-123456789">Agency A</receiver-org>
      <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
      <value currency="EUR" value-date="2012-01-01">1000</value>
      <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
      <tied-status code="3">Partially tied</tied-status>
      <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
      <transaction-type code="IF">Incoming Funds</transaction-type>
      <description>Transaction description text</description>
    </transaction>    
