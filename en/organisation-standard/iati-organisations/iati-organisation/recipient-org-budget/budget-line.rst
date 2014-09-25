Example Usage
~~~~~~~~~~~~~
Example ``budget-line`` for ``recipient-org-budget`` of an ``iati-orgaisation``.

| An example ``@ref`` attribute is included.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 8, 11

| The ``budget-line`` element can be repeated in any ``recipient-org-budget``. 

			
Changelog
~~~~~~~~~

2.01
^^^^
| The ``budget-line`` element was introduced in 2.01.

1.03
^^^^
| Currency values are now allowed to be declared as decimals instead of integers.
