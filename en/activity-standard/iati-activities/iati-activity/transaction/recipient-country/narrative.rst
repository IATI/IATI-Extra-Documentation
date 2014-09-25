Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-country`` element.

| Note: the ``narrative`` element is optional and should only be used to provide any essential clarification additional to name available in the ``Country`` codelist.  

.. code-block:: xml
	:emphasize-lines: 2
	
	<recipient-country code="XK">
		<narrative>Kosovo (As per UNSCR 1244)<narrative>
	</recipient-country>   
    
| The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``xml:lang`` attribute.  Example not shown.
