Example Usage
~~~~~~~~~~~~~
The ``indicator`` element is contained within a ``result`` element.  It also
acts as a container for other sub-elements.

Example ``indicator`` with the ``IndicatorMeasure`` code of *1* (Unit). This example also declares that the data is ascending:

.. code-block:: xml

    <result>
    ....
        <indicator measure="1" ascending="1">
        ....
        </indicator>
    .....
    </result>    

Full example

.. code-block:: xml

		<result type="1" aggregation-status="1">
			<title>Result 1 title</title>
			<description>Result 1 description text</description>
			<indicator measure="1" ascending="1">
				<title>Indicator 1 title</title>
				<description>Indicator 1 description text</description>
				<baseline year="2012" value="10"/>
				<period> 
					<period-start iso-date="2013-01-01"/> 
					<period-end iso-date="2013-03-31"/> 
					<target value="10"/> 
					<actual value="11"/> 
				</period> 
			</indicator>
		</result>


The ``indicator`` element can be repeated within any ``result`` element:

.. code-block:: xml

		<result type="1" aggregation-status="1">
			<title>Result 1 title</title>
			<description>Result 1 description text</description>
			<indicator measure="1" ascending="1">
				<title>Indicator 1 title</title>
				<description>Indicator 1 description text</description>
				<baseline year="2012" value="10"/>
				<period> 
					<period-start iso-date="2013-01-01"/> 
					<period-end iso-date="2013-03-31"/> 
					<target value="10"/> 
					<actual value="11"/> 
				</period> 
			</indicator>
			<indicator measure="1" ascending="1">
				<title>Indicator 2 title</title>
				<description>Indicator 2 description text</description>
				<baseline year="2012" value="10"/>
				<period> 
					<period-start iso-date="2013-04-01"/> 
					<period-end iso-date="2013-06-30"/> 
					<target value="11"/> 
					<actual value="12"/> 
				</period> 
			</indicator>
		</result>
