Example Usage
~~~~~~~~~~~~~
Example usage of ``transaction-type`` in context of ``transaction`` element.

Example declares ``TransactionType`` code *IF* (Incoming Funds)

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 4
	
Full example with additional elements which can override the default value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 4
	    
An ``iati-activity`` can have multiple ``transaction`` elements, with different ``TransactionType`` codes:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 5, 19
