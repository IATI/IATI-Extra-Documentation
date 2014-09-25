Example Usage
~~~~~~~~~~~~~
Example usage of ``recipient-org`` in context of ``recipient-org-budget`` element:

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 2, 4
	
Changelog
~~~~~~~~~
2.01
^^^^
| Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
