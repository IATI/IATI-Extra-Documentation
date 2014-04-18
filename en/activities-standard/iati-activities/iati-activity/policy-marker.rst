Example Usage
~~~~~~~~~~~~~
Example ``policy-marker`` that declares a ``PolicyMarker`` code *04`, with a ``PolicySignificance`` code of *2*.  In this example, the ``vocabulary`` *DAC* is also declared:

.. code-block:: xml

    <policy-marker vocabulary="DAC" code="04" significance="2"/>

Additionally, a text description for the ``PolicyMarker`` code can be provided:

.. code-block:: xml

    <policy-marker vocabulary="DAC" code="04">Trade Development</policy-marker>

Should a description be used that is different to the default language set for the activity, then this should be declared as follows:

It may be appropriate to repeat the ``policy-marker`` description text in other languages using ``xml:lang`` attribute.  In this example, the language *en* is set in the ''iati-activity'' elenment:

.. code-block:: xml

  <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
	...
	<policy-marker vocabulary="DAC" code="04" significance="2">Trade Development</policy-marker>
	<policy-marker vocabulary="DAC" code="04" significance="2" xml:lang="fr">Developpement du commerce</policy-marker>
	...
  </iati-activity>
