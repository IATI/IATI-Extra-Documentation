

Example Usage
~~~~~~~~~~~~~

The location element is used a contain various other elements

.. code-block:: xml

        <location>
           ....
        </location>

Example:

.. code-block:: xml

    <location ref="">
      <name>Kandahar</name>
      <location-reach code=""></location-reach>
      <location-id code=""></location-id>
      <description>West end of Kandahar-Kabul highway</description>
      <activity-description xml:lang="fr">xxxxxx</activity-description>
      <administrative code="xxxxxx" vocabulary="OSM" level="1">Kandahar Province, Afghanistan</administrative>
      <point srsName="http://www.opengis.net/def/crs/EPSG/0/4326">
        <coordinates>31.616944 65.716944</coordinates>
      </point>
    </location>
    
NOTE: The @srsName currently should always be http://www.opengis.net/def/crs/EPSG/0/4326

|The @percentage attribute has been deprecated as of 1.04. 
|However, in 1.03, it was used if more than one location was reported to specify the percentage of activity commitment allocated to this location (if available).

.. code-block:: xml

        <location percentage="85>
           ....
        </location>
        <location percentage="15>
           ....
        </location>


Changelog
~~~~~~~~~

1.04
^^^^
|The @ref attribute was introduced to provide a cross reference that a publisher can use to link back to their own internal system.
|The @percentage attribute was deemed unworkable and deprecated in 1.04


1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
