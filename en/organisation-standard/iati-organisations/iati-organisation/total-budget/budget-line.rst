Example Usage
~~~~~~~~~~~~~
Example ``budget-line`` for ``total-budget`` of an ``iati-organisation``.

| An example ``@ref`` attribute is included.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
	:emphasize-lines: 5, 8

| The ``budget-line`` element can be repeated in any ``total-budget``.


Changelog
~~~~~~~~~

2.01
^^^^
| The ``budget-line`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#budget-line-new-element>`__ as a child element of ``total-budget``.

.. meta::
  :order: 3
