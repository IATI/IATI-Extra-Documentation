Example Usage
~~~~~~~~~~~~~
The ``transaction`` element acts as a container for other sub elements.

At the ``transaction`` level, the attribute ``ref`` can be used to describe reference to this ``transaction`` in another system:

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

Example ``transaction``:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 1, 9

Full example with additional elements which can override the default value set in ``iati-activity``: 

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 1, 13
	    
An ``iati-activity`` can have multiple ``transaction`` elements.

.. literalinclude:: ../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 1, 14, 15, 28
