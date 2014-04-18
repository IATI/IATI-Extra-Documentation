Example Usage
~~~~~~~~~~~~~
The ``planned-disbursement`` element acts as a container for other sub elements:

The attribute ``updated`` should declare the date the ``planned-disbursement`` was last changed:

.. code-block:: xml

		<planned-disbursement updated="2013-03-31">
        ....
		</planned-disbursement>

Full example:

.. code-block:: xml

		<planned-disbursement updated="2013-03-31">
		  <period-end iso-date="2013-03-31">2013-03-31</period-end>
		  <period-start iso-date="2013-03-31">2013-03-31</period-start>
		  <value currency="EUR" value-date="2013-03-31">2000</value>
		</planned-disbursement>
