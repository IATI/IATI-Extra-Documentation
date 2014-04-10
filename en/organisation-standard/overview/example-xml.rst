Example Usage
=============

Definition
----------
This page presents example XML for the IATI organisation standard

Considerations
--------------
This is sample XML and not intended to reflect any real organisations or entities

Extracts from this example are used throughout this documentation

This example file can also be :doc:`downloaded </organisation-standard-example.xml/>`

.. code-block:: xml

	<iati-organisations generated-datetime="2014-04-03T18:27:37" version="1.04">
		<iati-organisation default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
			<reporting-org ref="AA-AAA-123456789" type="40">Organisation name</reporting-org>
			<iati-identifier>AA-AAA-123456789</iati-identifier>
			<name xml:lang="fr">Nom de l'organisme</name>
			<total-budget>
				<period-start iso-date="2014-01-01">2014</period-start>
				<period-end iso-date="2014-12-31">2014</period-end>
				<value currency="USD" value-date="2012-01-01">250000000</value>
			</total-budget>
			<total-budget>
				<period-start iso-date="2015-01-01">2015</period-start>
				<period-end iso-date="2015-12-31">2015</period-end>
				<value currency="USD" value-date="2013-01-01">300000000</value>
			</total-budget>
			<total-budget>
				<period-start iso-date="2016-01-01">2016</period-start>
				<period-end iso-date="2016-12-31">2016</period-end>
				<value currency="USD" value-date="2012-01-01">350000000</value>
			</total-budget>
			<recipient-org-budget>
				<recipient-org ref="123">Example Recipient Organisation</recipient-org>
				<period-start iso-date="2014-01-01">2014</period-start>
				<period-end iso-date="2014-12-31">2014</period-end>
				<value currency="USD" value-date="2014-01-01">2500000</value>
			</recipient-org-budget>
			<recipient-org-budget>
				<recipient-org ref="123">Example Recipient Organisation</recipient-org>
				<period-start iso-date="2015-01-01">2015</period-start>
				<period-end iso-date="2015-12-31">2015</period-end>
				<value currency="USD" value-date="2015-01-01">3000000</value>
			</recipient-org-budget>
			<recipient-org-budget>
				<recipient-org ref="123">Example Recipient Organisation</recipient-org>
				<period-start iso-date="2016-01-01">2016</period-start>
				<period-end iso-date="2016-12-31">2016</period-end>
				<value currency="USD" value-date="2016-01-01">3500000</value>
			</recipient-org-budget>
			<recipient-country-budget>
				<recipient-country code="AA">Country Name</recipient-country>
				<period-start iso-date="2014-01-01">2014</period-start>
				<period-end iso-date="2014-12-31">2014</period-end>
				<value currency="USD" value-date="2014-01-01">25000000</value>
			</recipient-country-budget>
			<recipient-country-budget>
				<recipient-country code="AA">Country Name</recipient-country>
				<period-start iso-date="2015-01-01">2015</period-start>
				<period-end iso-date="2015-12-31">2015</period-end>
				<value currency="USD" value-date="2015-01-01">30000000</value>
			</recipient-country-budget>
			<recipient-country-budget>
				<recipient-country code="AA">Country Name</recipient-country>
				<period-start iso-date="2016-01-01">2016</period-start>
				<period-end iso-date="2016-12-31">2016</period-end>
				<value currency="USD" value-date="2016-01-01">35000000</value>
			</recipient-country-budget>
			<document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_en.odt">
				<category code="B01"/>
				<language code="en"/>
				<title>Annual Report 2013</title>
			</document-link>
			<document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_fr.odt">
				<category code="B01"/>
				<language code="fr"/>
				<title>Rapport annuel 2013</title>
			</document-link>		
		</iati-organisation>
	</iati-organisations>

Further guidance
----------------

* :doc:`IATI organisation standard - reference pages </organisation-standard/iati-organisations/>`
