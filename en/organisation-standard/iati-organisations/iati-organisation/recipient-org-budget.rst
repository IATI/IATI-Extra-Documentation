Example Usage
~~~~~~~~~~~~~
Example of ``recipient-org-budget`` in USD for a single organisation in 2014, 2015 & 2016

.. code-block:: xml

		<recipient-org-budget>
		    <recipient-org ref="123">Example Recipient Organisation</recipient-org>
			<period-start iso-date="2014-01-01">2014</period-start>
			<period-end iso-date="2014-12-31">2014</period-end>
			<value currency="USD" value-date="2014-01-01">2500000<value>
		</recipient-org-budget>
		<recipient-org-budget>
		    <recipient-org ref="123">Example Recipient Organisation</recipient-org>
			<period-start iso-date="2015-01-01">2015</period-start>
			<period-end iso-date="2015-12-31">2015</period-end>
			<value currency="USD" value-date="2015-01-01">3000000<value>
		</recipient-org-budget>
		<recipient-org-budget>
		    <recipient-org ref="123">Example Recipient Organisation</recipient-org>
			<period-start iso-date="2016-01-01">2016</period-start>
			<period-end iso-date="2016-12-31">2016</period-end>
			<value currency="USD" value-date="2016-01-01">3500000<value>
		</recipient-org-budget>


Changelog
~~~~~~~~~
