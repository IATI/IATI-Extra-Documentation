Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-country`` element.

| Note: this is not required, but may be useful in some contexts.

.. code-block:: xml
	:emphasize-lines: 2
	
	<recipient-country code="CI">
		<narrative>Ivory Coast<narrative>
	</recipient-country>   
    
| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute.

.. code-block:: xml
	:emphasize-lines: 3
	
	<recipient-country code="CI">
		<narrative>Ivory Coast<narrative>
		<narrative xml:lang="fr">Côte-d'Ivoire<narrative>		
	</recipient-country>
