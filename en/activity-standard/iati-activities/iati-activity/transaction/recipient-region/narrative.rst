Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-region`` element.

| Note: this is not required, but may be useful in some contexts.

.. code-block:: xml
	:emphasize-lines: 2
	
	<recipient-region code="289">
		<narrative>South of Sahara, regional<narrative>
	</recipient-region>   

    
| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute.

.. code-block:: xml
	:emphasize-lines: 3
	
	<recipient-region code="289">
		<narrative>South of Sahara, regional<narrative>
		<narrative xml:lang="fr">Sud du Sahara , régional</narrative>
	</recipient-region>   
