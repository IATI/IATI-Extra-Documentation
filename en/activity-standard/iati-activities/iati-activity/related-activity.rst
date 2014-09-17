Example Usage
~~~~~~~~~~~~~
Example ``related-activity`` of an ``iati-activity``.

| This example declares a ``RelatedActivityType`` code *1* (*Parent*), using the ``type`` attribute.
| An example ``ref`` for another ``iati-activity`` of *AA-AAA-123456789-6789* is provided.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--related-activity starts-->
	:end-before: <!--related-activity ends-->

| Note: multiple related activities are expressed by repeating the ``related-activity`` element.	


