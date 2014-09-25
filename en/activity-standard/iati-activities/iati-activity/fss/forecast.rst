Example Usage
~~~~~~~~~~~~~
Example of ``forecast`` for the ``fss`` of an ``iati-activity``.

| An example date is declared in the ``@value-date`` attribute.
| This example date format conform to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

| This example declares the attribute ``@year`` as *2014*.

| This example declares a *Curency* code *GBP*, using the ``@currency`` attribute.
| Note: A *Currency* code should only be declared if different to ``@default-currency`` in the ``iati-activity`` element.

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
