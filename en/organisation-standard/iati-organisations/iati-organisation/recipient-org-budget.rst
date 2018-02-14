Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-org-budget`` for an ``iati-organisation``.

| This element is a parent for other child elements.

.. code-block:: xml

	<recipient-org-budget status="1">
	...
	</recipient-org-budget>

| Full example with all child elements.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->

| The ``recipient-org-budget`` element can be repeated in any ``iati-organisation``.

Changelog
~~~~~~~~~

2.02
^^^^
The ``status`` attribute was `added <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__.
