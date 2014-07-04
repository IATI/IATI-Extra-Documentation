Example Usage
~~~~~~~~~~~~~
Example usage of ``forecast`` in context of ``fss`` element.

Example declares ``year`` as *2014*, with a ``value`` of *10000*:

A date in ISO 8601 format (YYYY-MM-DD) is required for ``value-date`` date of the ``forecast``:

The ISO 4217 code for the ``currency`` in which the ``forecast`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--fss starts-->
	:end-before: <!--fss ends-->
	:emphasize-lines: 2

Example of multiple ``forecast`` elements:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--fss starts-->
	:end-before: <!--fss ends-->    
	:emphasize-lines: 2, 3  

Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``fss`` element and its child elements
