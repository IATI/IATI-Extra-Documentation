Example Usage
~~~~~~~~~~~~~
Example usage of ``repayment-type`` within ``loan-terms`` in context of ``crs-add`` element.

| The ``@code`` attribute declares a valid code (*1*) from the *LoanRepaymentType* codelist.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->
	:emphasize-lines: 4

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
