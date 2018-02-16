Example Usage
~~~~~~~~~~~~~
Example of ``baseline`` in context of an ``indicator`` in a ``result`` element.

| This example declares ``@year`` as *2012*, ``@iso-date`` as *2012-01-01*,with a ``@value`` of *10*:

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-indicator starts-->
	:end-before: <!--result-indicator ends-->

Changelog
~~~~~~~~~

2.03
^^^^

The occurance rules of the ``baseline`` element were amended so that `it can be reported multiple times <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.

The attribute ``@iso-date`` was `added <https://discuss.iatistandard.org/t/results-improve-consistency-of-results-standard-included-2-03/874>`__.

The attribute ``@value`` was made optional and rules for its use `added <https://discuss.iatistandard.org/t/results-represent-more-than-quantitative-data-included-2-03/872>`__.
