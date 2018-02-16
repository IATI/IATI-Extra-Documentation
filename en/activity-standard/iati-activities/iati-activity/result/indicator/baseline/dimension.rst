Example Usage
~~~~~~~~~~~~~
Example of ``dimension`` in context of a ``baseline`` element (as part of a parent ``result``/``indicator`` element).

| This example declares ``@name`` as *sex*, with a ``@value`` of *female*:
.. code-block:: xml

    <dimension name="sex" value="female" />


| The ``dimension`` element can be repeated within any ``target`` element:

.. literalinclude:: ../../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-baseline starts-->
	:end-before: <!--result-baseline ends-->

Changelog
~~~~~~~~~

2.03
^^^^
The optional ``dimension`` element was `added <https://discuss.iatistandard.org/t/results-allow-disaggregations-of-results-data-included-2-03/871>`__.
