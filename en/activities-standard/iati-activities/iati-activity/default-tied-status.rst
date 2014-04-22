Example Usage
~~~~~~~~~~~~~
Example declaring just the ``TiedStatus`` code *5*:

.. code-block:: xml

        <default-tied-status code="5"/>

Additionally, a text description of the ``TiedStatus`` code can be provided:

.. code-block:: xml

        <default-tied-status code="5">Untied</default-tied-status>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang``:

.. code-block:: xml

        <default-tied-status code="5" xml:lang="fr">Aide non-liee</default-tied-status>
