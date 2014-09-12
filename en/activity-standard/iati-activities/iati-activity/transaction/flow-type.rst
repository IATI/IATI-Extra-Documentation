Example Usage
~~~~~~~~~~~~~
Example usage of ``flow-type`` of a ``transaction`` in an ``iati-activity``.

| This example declares the ``FlowType`` code *20* (*OOF*) with the ``code`` attribute.

| Note: The ``flow-type`` element can override the ``default-flow-type`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 17
