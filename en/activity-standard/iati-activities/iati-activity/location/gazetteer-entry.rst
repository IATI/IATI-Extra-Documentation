

Example Usage
~~~~~~~~~~~~~

Example for the **Herat region of Afghanistan** - which has an ID of
**1140026** on `geonames.org <http://www.geonames.org/>`__.

To find Herat on geonames.org you would create a link like this:
http://www.geonames.org/1140026/

The IATI gazeteer-ref for geonames is ``GEO``, so the element would
look like:

.. code-block:: xml

    <location>
      ....
      <gazetteer-entry gazeteer-ref="GEO">1140026</gazetteer-entry>
      ....
    </location>


Changelog
~~~~~~~~~

1.04
^^^^

| Deprecated in 1.04
| The location/location-id element which identifies both gazetteer and administrative area vocabularies and codes should be used instead.
