Example Usage
~~~~~~~~~~~~~
The ``result`` element is a container for other sub-elements.  It is used to contain data for a result set.

Example ``result`` that uses ``ResultType`` code *1* (Output).  This ``result`` is suitable for aggregation, as the ``aggregation-status`` boolean is set to *1*:

.. code-block:: xml

        <result type="1" aggregation-status="1">
			...
        </result>
 
Full example: 
        
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


The ``result`` element can be repeated within any ``iati-activity``:

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
		
		<result type="1" aggregation-status="1">
			<title>Result 2 title</title>
			<description>Result 2 description text</description>
			<indicator measure="1" ascending="1">
				<title>Indicator 1 title</title>
				<description>Indicator 1 description text</description>
				<baseline year="2012" value="110"/>
				<period> 
					<period-start iso-date="2013-01-01"/> 
					<period-end iso-date="2013-03-31"/> 
					<target value="110"/> 
					<actual value="111"/> 
				</period> 
			</indicator>
		</result>

