Example Usage
~~~~~~~~~~~~~
A ''comment'' for ''target'' can be declared as such:

.. code-block:: xml

        <comment>Target comment text</comment>

Should the ``comment`` be in a language other than the default language declared in ``iati-activity``, then it should be described:

.. code-block:: xml

        <comment xml:lang="fr">Commentaire de texte de "target"</comment>

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
					<target value="10">
						<comment>Baseline comment text</comment> 
					</target>
					<actual value="11"/>
				</period> 
			</indicator>
		</result>
