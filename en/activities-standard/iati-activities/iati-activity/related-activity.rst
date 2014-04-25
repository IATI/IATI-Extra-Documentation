Example Usage
~~~~~~~~~~~~~
Example ``related-activity`` with ``RelatedActivityType`` code *1* and ``ref`` for another ``iati-activity``: *AA-AAA-123456789-6789*:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--related-activity starts-->
	:end-before: <!--related-activity ends-->

Multiple ``related-activity`` can be declared:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--related-activity starts-->
	:end-before: <!--related-activity ends-->
	
Additionally, a text title of the specific related ``iati-activity`` can be provided:

.. code-block:: xml

        <related-activity ref="AA-AAA-123456789-ABC" type="3">Related activity name</related-activity>


  

