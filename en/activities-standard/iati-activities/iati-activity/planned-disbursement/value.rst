Example Usage
~~~~~~~~~~~~~

A date of value for currency conversions must also be provided as ISO 8601 (YYYY-MM-DD):

.. code-block:: xml

		 <value currency="EUR" value-date="2013-03-31">2000</value>

Full example:

.. code-block:: xml

		<planned-disbursement updated="2013-03-31">
		  <period-end iso-date="2013-03-31">2013-03-31</period-end>
		  <period-start iso-date="2013-03-31">2013-03-31</period-start>
		  <value currency="EUR" value-date="2013-03-31">2000</value>
		</planned-disbursement>

The ISO 4217 code for the ``currency`` in which the ``planned-disbursement`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.


Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
