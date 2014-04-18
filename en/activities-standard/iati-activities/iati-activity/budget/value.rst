Example Usage
~~~~~~~~~~~~~

A date of value for currency conversions must also be provided as ISO 8601 (YYYY-MM-DD):

.. code-block:: xml

		<value currency="EUR" value-date="2014-01-01">3000</value>

Full example:

.. code-block:: xml

		<budget type="1">
		  <period-start iso-date="2014-01-01">Start of budget year 2014</period-start>
		  <value currency="EUR" value-date="2014-01-01">3000</value>
		  <period-end iso-date="2014-12-31">End of budget year 2014</period-end>
		</budget>

The ISO 4217 code for the ``currency`` in which the ``budget`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.


Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
