Example Usage
~~~~~~~~~~~~~
Example usage of ``provider-org`` of a ``planned-disbursement`` in an ``iati-activity``.

| This example declares the organisation identifier with the ``@ref`` attribute.

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789-1234AA" />

| This example declares the unique ``iati-identifier`` of the reported ``iati-activity`` from where the transaction is provided, with the ``@provider-activity-id`` attribute.

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789" provider-activity-id="BB-BBB-123456789-1234AA" />
        
Full example, within a ``planned-disbursement``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 5, 7 

Changelog
~~~~~~~~~

2.02
^^^^
The optional ``provider-org`` element was `added <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__.
