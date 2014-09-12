Example Usage
~~~~~~~~~~~~~
Example usage of ``receiver-org`` of a ``transaction`` in an ``iati-activity``.

| This example declares the organisation identifier with the ``ref`` attribute.

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789">Agency A</receiver-org>

| This example declares the unique ``iati-identifier`` of the reported ``iati-activity`` to where the transaction is received, with the ``receiver-activity-id``:

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" receiver-activity-id="AA-AAA-123456789-1234" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 11, 13

