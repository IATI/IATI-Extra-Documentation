Example Usage
~~~~~~~~~~~~~

Example when default language has already been declared in the ``iati-activity`` element:

.. code-block:: xml

        <title>Activity title</title>

If a default langage has NOT been declared in the ``iati-activity`` element, then a language must be specified

.. code-block:: xml

        <title xml:lang="en">Activity title</title>

A title may be repeated in many languages. This example assumes a default language of English has been declared in ``iati-activies``.  A French and Spanish title are provided:

.. code-block:: xml

        <title>Grant Performance Report</title>
        <title xml:lang="fr">Titre de l'activité</title>
        <title xml:lang="es">Título de la actividad</title>

It is good practice to provide activity titles in the language(s) spoken in the country(ies) where the activity take place, or is aimed at.
