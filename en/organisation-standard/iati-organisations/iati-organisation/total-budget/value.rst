Example Usage
~~~~~~~~~~~~~

Example in context of a single ``total-budget`` element:

.. code-block:: xml

		<total-budget>
			<period-start iso-date="2015-01-01">2015</period-start>
			<period-end iso-date="2015-12-31">2015</period-end>
			<value currency="USD" value-date="2013-01-01">300000000</value>
		</total-budget>
Changelog
~~~~~~~~~

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
