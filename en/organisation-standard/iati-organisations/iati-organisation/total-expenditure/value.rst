Example Usage
~~~~~~~~~~~~~
Example ``value`` of ``total-expenditure`` for an ``iati-organisation``.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares a *Currency* code *USD*, using the ``@currency`` attribute.
| Note: A ``Currency`` code should only be declared if different to ``@default-currency`` in the ``iati-organisation`` element.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-expenditure starts-->
	:end-before: <!--total-expenditure ends-->

Changelog
~~~~~~~~~

2.02
^^^^
The optional ``total-expenditure`` element was `added <http://support.iatistandard.org/entries/83404469-Add-Total-Expenditure-Element-To-Organisation-File>`__.

.. meta::
  :order: 2
