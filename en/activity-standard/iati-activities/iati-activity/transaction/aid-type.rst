Example Usage
~~~~~~~~~~~~~
Example usage of ``aid-type`` of a ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*A02*) from the *AidType* codelist.

| Note: The ``aid-type`` element can override the ``default-aid-type`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 21
