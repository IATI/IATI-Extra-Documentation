Example Usage
~~~~~~~~~~~~~
Example declaring just the ``CollaborationType`` code *1*:

.. code-block:: xml

    <collaboration-type code="1"/>

Additionally, a description of the ``CollaborationType`` code can be declared:

.. code-block:: xml

    <collaboration-type code="1">Bilateral</collaboration-type>

Where this description differs to the default language of the ``iati-activity``, then this should be declared using ``xml:lang`` - example of Dutch:

.. code-block:: xml

    <collaboration-type code="1" xml:lang="nl">Bilateraal</collaboration-type>
