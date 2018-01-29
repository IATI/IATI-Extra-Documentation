Example Usage
~~~~~~~~~~~~~
Example of ``baseline`` in context of an ``indicator`` in a ``result`` element.

| This example declares ``@year`` as *2012*, ``@iso-date`` as *2012-01-01*,with a ``@value`` of *10*:

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 18, 22

Changelog
~~~~~~~~~

2.03
^^^^
The attribute ``@iso-date`` was `added <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.
The ``baseline`` element in ``indicator`` in a ``result`` element can be reported multiple times `added <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.
The attribute ``@value`` was made optional and rules for its use `added <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__.
