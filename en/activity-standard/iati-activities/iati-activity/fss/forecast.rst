Example Usage
~~~~~~~~~~~~~
Example of ``forecast`` for the ``fss`` of an ``iati-activity``.

| A date in ISO 8601 format (YYYY-MM-DD) for the ``value-date`` attribute is required.

| This example declares ``year`` as *2014*, with a ``value`` of *10000*.

| The ISO 4217 code for the ``currency`` in which the ``forecast`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--fss starts-->
	:end-before: <!--fss ends-->
	:emphasize-lines: 2

| Note: multiple forecasts are expressed by repeating the ``forecast`` element.

Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``fss`` element and its child elements
