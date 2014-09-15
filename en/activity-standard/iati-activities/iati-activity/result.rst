Example Usage
~~~~~~~~~~~~~
Example ``result`` for an ``iati-activity``.

| This element is a parent for other child elements.

| This example declares ``ResultType`` code *1* (*Output*) with the ``type`` attribute..  

| This ``result`` example is suitable for aggregation, as the ``aggregation-status`` boolean is set to *1*:

.. code-block:: xml

        <result type="1" aggregation-status="1">
			...
        </result>

| Full example with all child elements:
 
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 1, 42

| Note: multiple results are expressed by repeating the ``result`` element.

