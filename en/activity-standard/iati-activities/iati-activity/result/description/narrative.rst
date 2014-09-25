Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``description`` of a ``result``.

.. code-block:: xml
	:emphasize-lines: 2	
	
		<description>
			<narrative>Result description text</narrative>
			<narrative xml:lang="fr">Result texte de description</narrative>      
		</description>

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute:

.. code-block:: xml
	:emphasize-lines: 3	
	
		<description>
			<narrative>Result description text</narrative>
			<narrative xml:lang="fr">Result texte de description</narrative>   
		</description>
	
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
