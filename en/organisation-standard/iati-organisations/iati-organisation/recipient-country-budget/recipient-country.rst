Example Usage
~~~~~~~~~~~~~
Example in context of a single ``recipient-country-budget`` element:

.. code-block:: xml

		<recipient-country-budget>
		    <recipient-country code="AA">Country Name</recipient-org>
			<period-start iso-date="2015-01-01">2015</period-start>
			<period-end iso-date="2015-12-31">2015</period-end>
			<value currency="USD" value-date="2015-01-01">30000000<value>
		</recipient-country-budget>

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
