Example Usage
~~~~~~~~~~~~~
An ISO 8601 code for the ``period-end`` date of the reporting period (YYYY-MM-DD) is required:

.. code-block:: xml

    <period-end iso-date="2014-12-31">End of budget year 2014</period-end>
    
Full example:

.. code-block:: xml

		<budget type="1">
		  <period-start iso-date="2014-01-01">Start of budget year 2014</period-start>
		  <value currency="EUR" value-date="2014-01-01">3000</value>
		  <period-end iso-date="2014-12-31">End of budget year 2014</period-end>
		</budget>
