Example Usage
~~~~~~~~~~~~~
Example declaring just the ``FlowType`` code *10*:

.. code-block:: xml

        <default-flow-type code="10"/>

Additionally, a text description of the ``FlowType`` code can be provided:

.. code-block:: xml

        <default-flow-type code="10">ODA</default-flow-type>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang``:

.. code-block:: xml

        <default-flow-type code="10" xml:lang="fr">APD</default-flow-type>
