Example Usage
~~~~~~~~~~~~~

When conditions are attached, they can be described using the @type code list, along with a free text description: 

.. code-block:: xml

    <conditions attached="1">
        <condition type="1">Condition text here.</condition>
    </conditions>
    
From version 1.04, a language attribute can also be included

.. code-block:: xml

    <conditions attached="1">
        <condition type="1" xml:lang="fr">Condition texte ici.</condition>
    </conditions>
