Example Usage
~~~~~~~~~~~~~
Example of ``location`` in context of an ``target`` element (as part of a parent ``result``/``indicator`` element).

| This example declares ``@ref`` as *AF-KAN*, which matches the ``@ref`` value for a location already referenced in iati-activity/location:
.. code-block:: xml

    <location ref="AF-KAN" />


| The ``location`` element can be repeated within any ``target`` element:

.. literalinclude:: ../../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 27, 28

Changelog
~~~~~~~~~

2.02
^^^^
The optional ``location`` element was `added <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__.