Example Usage
=============

Definition
----------
This page presents example XML for the **IATI activity standard**

Considerations
--------------
This is sample XML and not intended to reflect any real activities, organisations or entities

Extracts from this example are used throughout this documentation

This example file can also be `downloaded <>`__.

.. code-block:: xml

					<iati-activities generated-datetime="2014-04-03T18:27:37" version="1.04">
					  <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
						<reporting-org ref="AA-AAA-123456789" type="21">Agency A</reporting-org>
						<iati-identifier>AA-AAA-123456789-ABC123</iati-identifier>
						<other-identifier owner-name="Agency A" owner-ref="AA-AAA-123456789">ABC123-XYZ</other-identifier>
						<title>Activity title</title>
						<description type="1">General activity description text.  	Long description of the activity with no particular structure.</description>
						<description type="2">Objectives for the activity, for example from a logical framework.</description>
						<description type="3">Statement of groups targeted to benefit from the activity.</description>
						<activity-status code="Implementation">2</activity-status>
						<activity-date iso-date="2012-04-15" type="start-planned">2012-04-15</activity-date>
						<activity-date iso-date="2012-04-28" type="start-actual">2012-04-28</activity-date>
						<activity-date iso-date="2015-12-31" type="end-planned">2015-12-31</activity-date>
						<contact-info type="1">
						  <organisation>Agency A</organisation>
						  <person-name>A. Example</person-name>
						  <job-title>Transparency Lead</job-title>
						  <mailing-address>Transparency House, The Street, Town, City, Postcode</mailing-address>
						  <telephone>0044111222333444</telephone>
						  <email>transparency@example.org</email>
						  <website>http://www.example.org</website>
						</contact-info>
						<participating-org ref="BB-BBB-123456789" role="Funding" type="40">Agency B</participating-org>
						<participating-org ref="CC-CCC-123456789" role="Extending" type="10">Agency C</participating-org>
						<participating-org ref="AA-AAA-123456789" role="Implementing" type="21">Agency A</participating-org>
						<activity-scope code="3">Multi-national</activity-scope>
						<!--Note: only country OR region has to be declared-->
						<recipient-country code="AA">Country AA</recipient-country>
						<recipient-region code="456" vocabulary="1">Region 2</recipient-region>
						<!--location example to follow-->
						<sector code="111" vocabulary="DAC">Sector 1</sector>
						<country-budget-items vocabulary="2">
						  <budget-item code="ABC" percentage="50">
							<description>Description text</description>
						  </budget-item>
						</country-budget-items>
						<policy-marker code="01" significance="3" vocabulary="DAC">Policy Marker 1</policy-marker>
						<policy-marker code="02" significance="3" vocabulary="DAC">Policy Marker 2</policy-marker>
						<collaboration-type code="1">Bilateral</collaboration-type>
						<default-finance-type code="110">Aid grant excluding debt reorganisation</default-finance-type>
						<default-flow-type code="10">ODA</default-flow-type>
						<default-aid-type code="A01">General budget support</default-aid-type>
						<default-tied-status code="3">Partially tied</default-tied-status>
						<budget type="1">
						  <period-start iso-date="2014-01-01">Start of budget year 2014</period-start>
						  <value currency="EUR" value-date="2014-01-01">3000</value>
						  <period-end iso-date="2014-12-31">End of budget year 2014</period-end>
						</budget>
						<budget type="2">
						  <period-start iso-date="2013-01-01">Start of budget year 2013</period-start>
						  <value currency="EUR" value-date="2013-01-01">2001</value>
						  <period-end iso-date="2013-12-31">End of budget year 2013</period-end>
						</budget>
						<budget type="1">
						  <period-start iso-date="2012-01-01">Start of budget year 2012</period-start>
						  <value currency="EUR" value-date="2012-01-01">1000</value>
						  <period-end iso-date="2012-12-31">End of budget year 2012</period-end>
						</budget>
						<budget type="1">
						  <period-start iso-date="2013-01-01">Start of budget year 2013</period-start>
						  <value currency="EUR" value-date="2013-01-01">2000</value>
						  <period-end iso-date="2013-12-31">End of budget year 2013</period-end>
						</budget>
						<planned-disbursement updated="2012-03-31">
						  <period-end iso-date="2012-03-31">2012-03-31</period-end>
						  <period-start iso-date="2012-03-31">2012-03-31</period-start>
						  <value currency="EUR" value-date="2012-03-31">1000</value>
						</planned-disbursement>
						<planned-disbursement updated="2013-03-31">
						  <period-end iso-date="2013-03-31">2013-03-31</period-end>
						  <period-start iso-date="2013-03-31">2013-03-31</period-start>
						  <value currency="EUR" value-date="2013-03-31">2000</value>
						</planned-disbursement>
						<planned-disbursement updated="2014-03-31">
						  <period-end iso-date="2014-03-31">2014-03-31</period-end>
						  <period-start iso-date="2014-03-31">2014-03-31</period-start>
						  <value currency="EUR" value-date="2014-03-31">3000</value>
						</planned-disbursement>
						<capital-spend percentage="50.5" />
						<transaction ref="XYZ">
						  <aid-type code="A01">General budget support</aid-type>
						  <flow-type code="10">ODA</flow-type>
						  <provider-org provider-activity-id="BB-BBB-123456789-1234" ref="BB-BBB-123456789">Agency B</provider-org>
						  <receiver-org receiver-activity-id="CC-CCC-123456789-1234" ref="CC-CCC-123456789">Agency C</receiver-org>
						  <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
						  <value currency="EUR" value-date="2012-01-31">1000</value>
						  <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
						  <tied-status code="3">Partially tied</tied-status>
						  <transaction-date iso-date="2012-01-31">2012-01-31</transaction-date>
						  <transaction-type code="C">Commitment</transaction-type>
						  <description>Description text</description>
						</transaction>
						<transaction ref="ABC">
						  <aid-type code="A01">General budget support</aid-type>
						  <flow-type code="10">ODA</flow-type>
						  <provider-org provider-activity-id="BB-BBB-123456789-1234" ref="BB-BBB-123456789">Agency B</provider-org>
						  <receiver-org receiver-activity-id="CC-CCC-123456789-1234" ref="CC-CCC-123456789">Agency C</receiver-org>
						  <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
						  <value currency="EUR" value-date="2012-01-01">1000</value>
						  <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
						  <tied-status code="3">Partially tied</tied-status>
						  <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
						  <transaction-type code="C">Commitment</transaction-type>
						  <description>Description text</description>
						</transaction>
						<transaction ref="1234">
						  <aid-type code="A01">General budget support</aid-type>
						  <flow-type code="10">ODA</flow-type>
						  <provider-org provider-activity-id="BB-BBB-123456789-1234AA" ref="BB-BBB-123456789">Agency B</provider-org>
						  <receiver-org receiver-activity-id="AA-AAA-123456789-1234" ref="AA-AAA-123456789">Agency A</receiver-org>
						  <disbursement-channel code="1">Money is disbursed through central Ministry of Finance or Treasury</disbursement-channel>
						  <value currency="EUR" value-date="2012-01-01">1000</value>
						  <finance-type code="110">Aid grant excluding debt reorganisation</finance-type>
						  <tied-status code="3">Partially tied</tied-status>
						  <transaction-date iso-date="2012-01-01">2012-01-01</transaction-date>
						  <transaction-type code="IF">Incoming Funds</transaction-type>
						  <description>Description text</description>
						</transaction>
						<document-link format="application/odt" url="http:www.example.org/docs/evaluation.odt">
						  <category code="A07">Review of project performance and evaluation</category>
						  <language code="en">English</language>
						  <title>Project evaluation document</title>
						</document-link>
						<document-link format="application/odt" url="http:www.example.org/docs/project.odt">
						  <category code="A01">Pre- and post-project impact appraisal</category>
						  <language code="en">English</language>
						  <title>Project document</title>
						</document-link>
						<activity-website>http://example.org/activities/123456789</activity-website>
						<related-activity ref="AA-AAA-123456789-ABC" type="3">Related activity name</related-activity>
						<related-activity ref="AA-AAA-123456789-6789" type="1">Related activity name</related-activity>
						<conditions attached="1">
						  <condition type="1">Conditions text</condition>
						</conditions>
						<conditions attached="1">
						  <condition type="2">Conditions text</condition>
						</conditions>
						<legacy-data iati-equivalent="transaction" name="cost" value="1000">Legacy</legacy-data>
					  </iati-activity>
					</iati-activities>


Further guidance
----------------

* :doc:`IATI organisation standard - reference pages </activity-standard/iati-activities/>`
