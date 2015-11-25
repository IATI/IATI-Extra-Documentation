Example Usage
~~~~~~~~~~~~~
Example usage of ``receiver-org`` of a ``planned-disbursement`` in an ``iati-activity``.

| This example declares the organisation identifier with the ``@ref`` attribute.
| This example also declares the type of organisation which received the funds, using the @type attribute.

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" type="23">Agency A</receiver-org>

| This example declares the unique ``iati-identifier`` of the reported ``iati-activity`` to where the transaction is received, with the ``@receiver-activity-id`` attribute.

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" type="23" receiver-activity-id="AA-AAA-123456789-1234" />

Full example, within a ``planned-disbursement``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 8, 10

Changelog
~~~~~~~~~

2.02
^^^^
The optional ``receiver-org`` element was `added <http://support.iatistandard.org/entries/29665337-Add-provider-org-and-receiver-org-to-planned-disbursement-element>`__.
