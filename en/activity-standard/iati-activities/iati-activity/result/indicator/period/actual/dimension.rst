Example Usage
~~~~~~~~~~~~~
Example of ``dimension`` in context of an ``actual`` element (as part of a parent ``result``/``indicator`` element).

| This example declares ``@name`` as *sex*, with a ``@value`` of *female*:
.. code-block:: xml

    <dimension name="sex" value="female" />


| The ``dimension`` element can be repeated within any ``actual`` element:

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 38, 39

Changelog
~~~~~~~~~

2.02
^^^^
The optional ``dimension`` element was `added <http://support.iatistandard.org/entries/79499149-Support-disaggregation-of-performance-data>`__.