Example Usage
~~~~~~~~~~~~~

An ISO 8601 code for the ``period-end`` date of the reporting period (YYYY-MM-DD) is required:

.. code-block:: xml

		  <period-end iso-date="2013-03-31">2013-03-31</period-end>
    
Full example:

.. code-block:: xml

		<planned-disbursement updated="2013-03-31">
		  <period-end iso-date="2013-03-31">2013-03-31</period-end>
		  <period-start iso-date="2013-03-31">2013-03-31</period-start>
		  <value currency="EUR" value-date="2013-03-31">2000</value>
		</planned-disbursement>
