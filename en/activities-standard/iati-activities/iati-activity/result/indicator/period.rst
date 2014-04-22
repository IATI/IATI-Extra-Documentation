Example Usage
~~~~~~~~~~~~~
The ``period`` element is found within the ``indicator`` element, which sits within a ``result`` for an ''iati-activity'':



.. code-block:: xml

		<result>
			...
			<indicator>
				...	
				<period>
					...
				</period>
			</indicator>
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

