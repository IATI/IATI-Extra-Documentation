Example Usage
~~~~~~~~~~~~~
The full name of the organisation receiving the financial ``transaction``
(receiving in the case of loan and interest repayments).:

.. code-block:: xml

        <receiver-org>Agency A</receiver-org>

The unique Organisation Identifier for the ``receiver-org``.:

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789">Agency A</receiver-org>


If the funds are being provided from another reported ``iati-activity``, this
must record the unique ``iati-identifier`` for that ``iati-activity``:

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" receiver-activity-id="AA-AAA-123456789-1234" >Agency A</receiver-org>

Full example:

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 7
	
Full example with additional elements which can override the default value set in ``iati-activity``: 

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 7
