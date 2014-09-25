Example Usage
~~~~~~~~~~~~~
| Example usage of ``title`` of a ``document-link`` in an ``iati-organisation``.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 2, 4

Changelog
~~~~~~~~~
2.01
^^^^
Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
