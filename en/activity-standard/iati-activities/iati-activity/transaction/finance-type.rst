Example Usage
~~~~~~~~~~~~~
Example usage of ``finance-type`` of a ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*111*) from the *FinanceType* codelist.

| Note: The ``finance-type`` element can override the ``default-finance-type`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 20
