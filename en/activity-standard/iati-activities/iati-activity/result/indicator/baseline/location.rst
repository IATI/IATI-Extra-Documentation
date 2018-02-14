Example Usage
~~~~~~~~~~~~~
Example of ``location`` in context of a ``baseline`` element (as part of a parent ``result``/``indicator`` element).

| This example declares ``@ref`` as *AF-KAN*, which matches the ``@ref`` value for a location already referenced in iati-activity/location:
.. code-block:: xml

    <location ref="AF-KAN" />


| The ``location`` element can be repeated within any ``actual`` element:

.. literalinclude:: ../../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->

Changelog
~~~~~~~~~

2.03
^^^^
The optional ``location`` element was `added <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.
