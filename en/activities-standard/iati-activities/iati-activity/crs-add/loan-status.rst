Example Usage
~~~~~~~~~~~~~
The ``loan-status`` element acts as a container for other elements.

Example usage of ``loan-status`` in context of ``crs-add`` element.

Example declares ``year`` as *2014*.

A date in ISO 8601 format (YYYY-MM-DD) is required for ``value-date`` date of the reporting ``period``:

The ISO 4217 code for the ``currency`` in which the ``loan-status`` is denominated should be declared using the ``Currency`` codelist, but only if different to ``default-currency`` in the ``iati-activity`` element.

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--crs-add starts-->
	:end-before: <!--crs-add ends-->
	:emphasize-lines: 10, 15


Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``crs-add`` element and its child elements
