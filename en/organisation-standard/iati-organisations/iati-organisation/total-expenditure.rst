Example Usage
~~~~~~~~~~~~~
| Example of ``total-expenditure`` for an ``iati-organisation``.

| This element is a parent for other child elements.

.. code-block:: xml

	<total-expenditure>
	...
	</total-expenditure>

| Full example with all child elements.

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-expenditure starts-->
	:end-before: <!--total-expenditure ends-->
	:emphasize-lines: 1, 9

| The ``total-expenditure`` element can be repeated in any ``iati-organisation``. 

Changelog
~~~~~~~~~
2.02
^^^^
The optional ``total-expenditure`` element was `added <http://support.iatistandard.org/entries/83404469-Add-Total-Expenditure-Element-To-Organisation-File>`__.
