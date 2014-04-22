Notes
~~~~~

The monetary value of the transaction in the specified currency –
negative for repayments or reduced/cancelled commitments.

Example Usage
~~~~~~~~~~~~~
Example using a ISO 8601 date (YYYY-MM-DD) date for ``value-date``;

.. code-block:: xml

    <value value-date="2012-01-01">1000</value>

The ISO 4217 code for the currency in which the project is denominated
should be declared, only if different to default ``default-currency`` in ``iati-activity``

.. code-block:: xml

    <value currency="EUR" value-date="2012-01-01">1000</value>

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

Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of
integers.
