Example Usage
~~~~~~~~~~~~~
Example usage of ``tied-status`` of a ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*5*) from the *TiedStatus* codelist.

| Note: The ``tied-status`` element can override the ``default-tied-status`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 22
