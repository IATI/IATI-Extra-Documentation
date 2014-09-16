Example Usage
~~~~~~~~~~~~~
Example of ``fss`` of an ``iati-activity``.

| A date in ISO 8601 format (YYYY-MM-DD) for the ``extraction-date`` attribute is required.

| This example declares the attribute ``phaseout-year`` as *2016*.

| A boolean declares that this ``fss`` example is a partner country priority.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--fss starts-->
	:end-before: <!--fss ends-->
	:emphasize-lines: 1, 3
      

Changelog
~~~~~~~~~

1.03
^^^^

| New in 1.03
| Added the optional ``fss`` element and its child elements
