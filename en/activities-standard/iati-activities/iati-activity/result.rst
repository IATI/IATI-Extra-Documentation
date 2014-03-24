Example Usage
~~~~~~~~~~~~~

Container element for a result set. The type attribute can be used to
describe whether it is an output, outcome, or impact indicator.

A flag to indicate whether the data in this result set is
suitable for aggregation. Boolean ``1`` means that the data can be
aggregated. If aggregation-status is omitted, then ``1`` is assumed.

.. code-block:: xml

        <result type="1" aggregation-status="0">
          <indicator ascending="true" measure="1">
            <title>Number of community volunteers who successfully completed a volunteer training program</title>
            <period> 
              <period-start iso-date="2013-01-01"/> 
              <period-end iso-date="2013-03-31"/> 
              <target value="320"/> 
              <actual value="359"/> 
            </period> 
          </indicator>
        </result>
