Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``recipient-country`` element.

| Note: Both the ``recipient-region`` and ``recipient-country`` elements still allow both a ``@code`` and descriptive text to be specified. This is to cover the isolated cases where the organisation publishing the data may not agree with name of a country or region given by the lookup codelists IATI uses.

.. code-block:: xml
	:emphasize-lines: 2
	
	<recipient-country code="XK">
		<narrative>Kosovo (As per UNSCR 1244)<narrative>
	</recipient-country>   

| Note: The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``@xml:lang`` attribute.  Example not shown.
	
Changelog
~~~~~~~~~

2.02
^^^^
The optional ``recipient-region-budget`` element was `added <http://support.iatistandard.org/entries/79323113-Org-Standard-recipient-region-budget>`__.
