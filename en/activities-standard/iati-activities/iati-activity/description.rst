Example Usage
~~~~~~~~~~~~~
Example of a ``description`` of an ``iati-activity``, with a ``DescriptionType`` of *1* (General):

.. code-block:: xml

        <description type="1">General activity description text. Long description of the activity with no particular structure.</description>

Additional ``description`` elements can be added for further ``DescriptionType``:

.. code-block:: xml

    <description type="1">General activity description text.  	Long description of the activity with no particular structure.</description>
    <description type="2">Objectives for the activity, for example from a logical framework.</description>
    <description type="3">Statement of groups targeted to benefit from the activity.</description>
    
It may be appropriate to repeat the ``description`` in other languages using ``xml:lang`` attribute.  In this example, the language *en* is set in the ''iati-activity'' elenment:

.. code-block:: xml

  <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
	...
    <description type="1">General activity description text.  	Long description of the activity with no particular structure.</description>
    <description type="2">Objectives for the activity, for example from a logical framework.</description>
    <description type="3">Statement of groups targeted to benefit from the activity.</description>
    <description type="1" xml:lang="fr" >Activité générale du texte de description. Longue description de l'activité sans structure particulière.</description>
    <description type="2" xml:lang="fr">Objectifs de l'activité, par exemple à partir d'un cadre logique.</description>
    <description type="3" xml:lang="fr">Déclaration de groupes ciblés pour bénéficier de l'activité.</description>
	...
  </iati-activity>
