Example Usage
~~~~~~~~~~~~~
Example ``related-activity`` with ``RelatedActivityType`` code *1* and ``ref`` for another ``iati-activity``: *GB-1-105838*:

.. code-block:: xml

       <related-activity type="1" ref="GB-1-105838"/>

Additionally, a text title of the specific related ``iati-activity`` can be provided:

.. code-block:: xml

        <related-activity type="1" ref="GB-1-105838">Trade Sector Programme</related-activity>

Where this text is in a language that differs from the default set in ``iati-activity``, then this should be declared accordingly using ``xml:lang`` attribute.  In this example, the language *en* is set in the ''iati-activity'' elenment::

.. code-block:: xml

  <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" xml:lang="en">
	...
        <related-activity type="1" ref="GB-1-105838" xml:lang="fr">Programme du secteur commercial</related-activity>
	...
  </iati-activity>
