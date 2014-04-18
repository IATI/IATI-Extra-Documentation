Example Usage
~~~~~~~~~~~~~
The ``budget`` element acts as a container for other sub elements

The attribute ``type`` should declare the relevant ``BudgetType`` code.  If omitted, then ``BudgetType`` *Original* (code 1) is assumed:

.. code-block:: xml

        <budget type="1">
        ....
        </budget>

Full example:

.. code-block:: xml

		<budget type="1">
		  <period-start iso-date="2014-01-01">Start of budget year 2014</period-start>
		  <value currency="EUR" value-date="2014-01-01">3000</value>
		  <period-end iso-date="2014-12-31">End of budget year 2014</period-end>
		</budget>
