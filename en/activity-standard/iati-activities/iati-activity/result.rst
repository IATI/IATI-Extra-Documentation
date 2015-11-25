Example Usage
~~~~~~~~~~~~~
Example ``result`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@type`` attribute declares a valid code (*1*) from the *ResultType* codelist.
| The ``@aggregation-status`` *1* boolean is included, for illustration of suitability for aggregation.

.. code-block:: xml

        <result type="1" aggregation-status="1">
			...
        </result>

| Full example with all child elements:
 
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 1, 46

| The ``result`` element can be repeated in any ``iati-activity``.

