Example Usage
~~~~~~~~~~~~~
Example of ``fss`` of an ``iati-activity``.
| 
| An example date is declared in the ``extraction-date`` attribute.
| This example date format conform to the xsd:date standard - for most cases *YYYY-MM-DD* is sufficient.
| 
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
