Example Usage
~~~~~~~~~~~~~
The ``result`` element is a container for other sub-elements.  It is used to contain data for a result set.

Example ``result`` that uses ``ResultType`` code *1* (Output).  This ``result`` is suitable for aggregation, as the ``aggregation-status`` boolean is set to *1*:

.. code-block:: xml

        <result type="1" aggregation-status="1">
			...
        </result>
 
.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 1, 21


The ``result`` element can be repeated within any ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->
	:emphasize-lines: 1, 15, 16, 30
