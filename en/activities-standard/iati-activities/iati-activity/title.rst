Example Usage
~~~~~~~~~~~~~
Example title for an ``iati-activity``:

.. code-block:: xml

        <title>Activity title</title>

If a default langage has not been declared in the ``iati-activity`` element, then a language should be specified

.. code-block:: xml

        <title xml:lang="en">Activity title</title>

It may be appropriate to repeat the ``title`` in other languages using ``xml:lang`` attribute.  In this example, the language *en* is set in the ''iati-activity'' elenment:

.. code-block:: xml

	  <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
		...
        <title>Grant Performance Report</title>
        <title xml:lang="fr">Titre de l'activité</title>
        <title xml:lang="es">Título de la actividad</title>
		...
	  </iati-activity>
	  
Note: It is recommended to provide a ``title`` in the language(s) spoken in the country(ies) where the ``iati-activity`` take place, or is aimed at.
