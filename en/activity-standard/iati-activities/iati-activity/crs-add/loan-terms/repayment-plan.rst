Example Usage
~~~~~~~~~~~~~
Example usage of ``repayment-plan`` within ``loan-terms`` in context of ``crs-add`` element.

| The ``@code`` attribute declares a valid code (*4*) from the *LoanRepaymentPeriod* codelist.

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
