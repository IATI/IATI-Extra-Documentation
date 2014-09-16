Example Usage
~~~~~~~~~~~~~
Example ``transaction`` in an ``iati-activity``.

| This element is a parent for other child elements.

| This example declares the example value of *1234* with the ``ref`` attribute.

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 1, 22
	    
| Note: multiple budgets are expressed by repeating the ``budget`` element.
