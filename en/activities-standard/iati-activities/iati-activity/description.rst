
Example Usage
~~~~~~~~~~~~~

Below is a General description (type = ``1``) of an activity in English.

This also assumes that English has NOT been declared as the default language for this activity in the ``iati-activity`` element. If it had been, it is recommended not to re-declare the language attribute again.

.. code-block:: xml

        <description type="1">General activity description text. Long description of the activity with no particular structure.</description>

Additional ``description`` elements can be added for further types:

.. code-block:: xml

    <description type="1">General activity description text.  	Long description of the activity with no particular structure.</description>
    <description type="2">Objectives for the activity, for example from a logical framework.</description>
    <description type="3">Statement of groups targeted to benefit from the activity.</description>
    
It may be appropriate to repeat this description in other languages.  In this example, English is the default language of the activty, with French also declared:

.. code-block:: xml

    <description type="1">General activity description text.  	Long description of the activity with no particular structure.</description>
    <description type="2">Objectives for the activity, for example from a logical framework.</description>
    <description type="3">Statement of groups targeted to benefit from the activity.</description>
    <description type="1" xml:lang="fr" >Activité générale du texte de description. Description longue de l'activité sans structure particulière.</description>
    <description type="2" xml:lang="fr">Objectifs de l'activité, par exemple à partir d'un cadre logique.</description>
    <description type="3" xml:lang="fr">Déclaration de groupes ciblés de bénéficier de l'activité.</description>

