Example Usage
~~~~~~~~~~~~~
Example usage of ``finance-type`` of a ``transaction`` in an ``iati-activity``.

| This example declares the ``FinanceType`` code *111* (*Subsidies to national private investors*) with the ``code`` attribute.

| Note: The ``finance-type`` element can override the ``default-finance-type`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 18
