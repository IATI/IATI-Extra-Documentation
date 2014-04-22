Example Usage
~~~~~~~~~~~~~
Example declaring just the ``AidType`` code *A02*:

.. code-block:: xml

       <default-aid-type code="A02"/>

Additionally, a text description of the ``AidType`` code can be provided:

.. code-block:: xml

        <default-aid-type code="A02">Sector Budget Support</default-aid-type>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang``:

.. code-block:: xml

        <default-aid-type code="A02" xml:lang="fr">Soutien budgetaire sectoriel</default-aid-type>
