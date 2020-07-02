Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``expense-line`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-expenditure starts-->
	:end-before: <!--total-expenditure ends-->

| Note: The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``@xml:lang`` attribute.  Example not shown.

Changelog
~~~~~~~~~
2.02
^^^^
The optional ``total-expenditure`` element was `added <http://support.iatistandard.org/entries/83404469-Add-Total-Expenditure-Element-To-Organisation-File>`__.

.. meta::
  :order: 1
