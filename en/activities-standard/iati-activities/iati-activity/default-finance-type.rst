Example Usage
~~~~~~~~~~~~~
Example declaring just the ``FinanceType`` code *100*:

.. code-block:: xml

        <default-finance-type code="100"/>

Additionally, a text description of the ``FinanceType`` code can be provided:

.. code-block:: xml

        <default-finance-type code="100">Grant</default-finance-type>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang``:

.. code-block:: xml

        <default-finance-type code="100" xml:lang="fr">Don</default-finance-type>
