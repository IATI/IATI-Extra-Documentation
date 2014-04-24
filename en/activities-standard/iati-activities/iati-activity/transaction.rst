Example Usage
~~~~~~~~~~~~~
The ``transaction`` element acts as a container for other sub elements.

At the ``transaction level, the attribute ``ref`` can be used to describe reference to this ``transaction`` in another system:

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

Example:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->

Full example with additional elements, some of which can override the value set in ``iati-activity``: 

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
    
An ``iati-activity`` can have multiple ``transaction`` elements:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
