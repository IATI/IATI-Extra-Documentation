Example Usage
~~~~~~~~~~~~~
The full name of the organisation making the financial ``transaction``
(receiving in the case of loan and interest repayments).:

.. code-block:: xml

        <provider-org>Agency B</provider-org>

The unique Organisation Identifier for the ``provider-org``:

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789-1234AA">Agency B</provider-org>

If the funds are being provided from another reported ``iati-activity``, this
must record the unique ``iati-identifier`` for that ``iati-activity``:

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789" provider-activity-id="BB-BBB-123456789-1234AA" >Agency B</provider-org>
        
Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 6

Full example with additional elements which can override the default value set in ``iati-activity``:  

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 6
