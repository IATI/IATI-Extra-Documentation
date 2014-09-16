Example Usage
~~~~~~~~~~~~~
Example usage of ``provider-org`` of a ``transaction`` in an ``iati-activity``.

| This example declares the organisation identifier with the ``ref`` attribute.

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789-1234AA" />

| This example declares the unique ``iati-identifier`` of the reported ``iati-activity`` from where the transaction is provided, with the ``provider-activity-id``:

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789" provider-activity-id="BB-BBB-123456789-1234AA" />
        
Full example, within a ``transaction``:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 8, 10 
