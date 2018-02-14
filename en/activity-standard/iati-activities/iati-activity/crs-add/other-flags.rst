Example Usage
~~~~~~~~~~~~~
Example usage of ``other-flags`` of ``crs-add`` for an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*1*) from the *CRSAddOtherFlags* codelist.

| A ``@significance`` boolean of *1* indicates that this flag is reported.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->


Changelog
~~~~~~~~~
2.01
^^^^
The element ``aid-type-flag`` has been `renamed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#other-flags-renamed-element>`__.

The associated codelist *AidTypeFlag* has been renamed as *CRSAddOtherFlags*

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
