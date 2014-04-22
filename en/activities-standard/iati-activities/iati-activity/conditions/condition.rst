Example Usage
~~~~~~~~~~~~~
When ``conditions`` are attached, they can be described using a free text description. 

The ``ConditionType`` of a ``condition`` should be specified, and should be a value from the relevant ``ConditionType`` codelist.

.. code-block:: xml

    <conditions attached="1">
        <condition type="1">Condition text here.</condition>
    </conditions>
    
From version 1.04, the schema now allows the ``xml:lang`` attribute to also be included

.. code-block:: xml

    <conditions attached="1">
        <condition type="1" xml:lang="fr">Condition texte ici.</condition>
    </conditions>

Changelog
~~~~~~~~~

1.04
^^^^

| It was always the intention of the standard that a condition could be specified in different languages but the schema has never allowed it.
| This has now been fixed.
