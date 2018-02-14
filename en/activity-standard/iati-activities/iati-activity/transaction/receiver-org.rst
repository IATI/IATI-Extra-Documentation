Example Usage
~~~~~~~~~~~~~
Example usage of ``receiver-org`` of a ``transaction`` in an ``iati-activity``.

| This example declares the organisation identifier with the ``@ref`` attribute.
| This example declares the type of organisation receiving the funds, using the ``@type`` attribute.

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" type="23">
          <narrative>Agency B</narrative>
        </receiver-org>

| This example additionally declares the unique ``iati-identifier`` of the reported ``iati-activity`` to where the transaction is received, with the ``@receiver-activity-id`` attribute.

.. code-block:: xml

        <receiver-org ref="AA-AAA-123456789" type="23" receiver-activity-id="AA-AAA-123456789-1234">
          <narrative>Agency A</narrative>
        </receiver-org>

Full example, within a ``transaction``.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->

Changelog
~~~~~~~~~

2.03
^^^^
| The definition of the ``@ref`` attribute was `updated <https://discuss.iatistandard.org/t/migration-of-organisationregistrationagency-codelist-to-org-id-guide-included-2-03/851>`__.

2.02
^^^^
| The attribute ``@type`` was `added <http://support.iatistandard.org/entries/81683876-provider-receiver-og-adding-type>`__.

2.01
^^^^
| Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
