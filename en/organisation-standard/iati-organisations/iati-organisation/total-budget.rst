Example Usage
~~~~~~~~~~~~~
| Example of ``total-budget`` for an ``iati-organisation``.

| This element is a parent for other child elements.

.. code-block:: xml

	<total-budget status="1">
	...
	</total-budget>

| Full example with all child elements.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
	:emphasize-lines: 1, 9

| The ``total-budget`` element can be repeated in any ``iati-organisation``. 

Changelog
~~~~~~~~~

2.02
^^^^
The ``status`` attribute was `added <http://support.iatistandard.org/entries/21150501-Budgets-and-tentativeness>`__.
