Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``comment`` of a ``actual``.

.. code-block:: xml
	:emphasize-lines: 2	
	
		<comment>
			<narrative>Actual comment text</narrative>
			<narrative xml:lang="fr">Actual comment texte</narrative>      
		</comment>

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute:

.. code-block:: xml
	:emphasize-lines: 3	
	
		<comment>
			<narrative>Actual comment text</narrative>
			<narrative xml:lang="fr">Actual comment texte</narrative>      
		</comment>
	
	
Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
