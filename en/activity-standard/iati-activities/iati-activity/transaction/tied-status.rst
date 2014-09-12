Example Usage
~~~~~~~~~~~~~
Example usage of ``tied-status`` of a ``transaction`` in an ``iati-activity``.

| This example declares the ``TiedStatus`` code *5* (*Untied*) with the ``code`` attribute.

| Note: The ``tied-status`` element can override the ``default-tied-status`` value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 20
