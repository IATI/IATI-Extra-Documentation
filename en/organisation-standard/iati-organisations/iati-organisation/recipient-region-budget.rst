Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-region-budget`` for an ``iati-organisation``.

| This element is a parent for other child elements.

.. code-block:: xml

	<recipient-region-budget>
	...
	</recipient-region-budget>

| Full example with all child elements.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-region-budget starts-->
	:end-before: <!--recipient-region-budget ends-->
	:emphasize-lines: 1, 10
	
| The ``recipient-region-budget`` element can be repeated in any ``iati-organisation``. 

Changelog
~~~~~~~~~
2.02
^^^^
The optional ``recipient-region-budget`` element was `added <http://support.iatistandard.org/entries/79323113-Org-Standard-recipient-region-budget>`__.
