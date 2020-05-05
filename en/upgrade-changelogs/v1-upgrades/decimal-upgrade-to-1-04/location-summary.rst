Location: Summary of changes in IATI Standard version 1.04
==========================================================

**See also:**
`Overview table of changes <https://docs.google.com/spreadsheets/d/1lr1sKwxCKKER4_eDTK254ivAOtpDCqh4k7Ki-y1XZn4/edit#gid=0>`__

Overview
--------

In order to improve the quality and effectiveness of geolocation data a
number of enhancements were made in the upgrade to `version 1.04 <http://iatistandard.org//upgrades/decimal-upgrade-to-1-04/>`__ of the
IATI Standard. Should publishers want to move from previous versions of
the IATI Standard (1.01, 1.02, 1.03) to 1.04, two things should be
considered:

1. Review current use of location related elements and attributes to
identify any possible changes (see Table 1 below)

2. Review the new location elements introduced in version 1.04 to
determine what additional location information could be published (see
Table 2 below)

A note on deprecation
---------------------

Some elements and attributes have been deprecated in version 1.04 of the
IATI Standard. You are strongly advised to no longer use those elements
and attributes.

However, in version 1.04 deprecated elements and attributes are NOT
removed. This means data published to version 1.04 of the IATI Standard
may still contain deprecated elements. Publishers may incorporate other
changes introduced in version 1.04, without making specific changes to
their location data elements. 

However, for those publishers using the location element it is advised to read this guidance and attempt to update data accordingly.

Deletion of Deprecated items
----------------------------

It is the intention of the IATI Secretariat to remove deprecated items
from the IATI Standard at each integer upgrade. Therefore those items
deprecated in version(s) 1.x of the IATI Standard will be removed in
version(s) 2.x

A note on codelist values and (text) names
------------------------------------------

Whilst versions 1.0x of the IATI Standard allow for codes to be
accompanied by a (text) name, this has not been included in this
guidance. Version 2.01 of the standard proposes language neutral use of
codes, hence the guidance here is to utilise:

.. code-block:: xml
    
    <exactness code="1"/>

rather than

.. code-block:: xml
    
    <exactness code="1">Exact</exactness>

For this reason, this guidance note omits details on use of (text) names
for code values.

Table 1: Comparison of location elements between versions 1.01/1.02/1.03 and 1.04
---------------------------------------------------------------------------------

(Click on Element\* name link for official IATI Standard V1.04
definition and examples)

.. list-table::
  :header-rows: 1

  * - **Element\***

    - **Attributes**

    - **In Use** **V1.03**

    - **In Use** **V1.04**

    - **Description of Change &** **Publisher Action Required (if any)**

    - **Example XML**

  * - `location <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/>`__

    -

    - Y

    - Y

    - No change

    -

  * -

    - @ref

    - N

    - Y

    - New.
      An internal reference that uniquely describes the location in the reporting organisation’s own system.
      Check if useful to include.

    - <location ref="AF-KAN">
      ….
      </location>

  * -

    - @percentage

    - Y

    - N

    - Deprecated. Should no longer be used.

      Consensus is that splitting activity costs pro rata is not feasible.

    -

  * - `location-type <http://iatistandard.org/105/activity-standard/iati-activities/iati-activity/location/location-type/>`__

    -

    - Y

    - N

    - Deprecated.
      Remove and replace with new location/location-class and
      location/feature-designation elements.

    - n/a

  * -

    - @code

    - Y

    - N

    - As above

    -

  * -

    - @xml:lang

    - Y

    - N

    - As above

    -

  * - `name <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/name/>`__
  
    -

    - Y

    - Y

    - No change

    - <name>Location name</name>

  * -
  
    - @xml:lang

    - Y

    - Y

    - As above

    -

  * - `description <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/description/>`__

    -

    - Y

    - Y

    - Partially changed.

      No change to element definition but the Standard now allows for two
      separate descriptions:
      
      1 - a description of the location itself
      
      2 - a (new) description of the activity taking place at the location.
      
      See new element location/activity-description to check if the
      information provided here is still correct for the new definitions.
      
    - <description>Location description</description>

  * -

    - @xml:lang

    - Y

    - Y

    - As above.

    -

  * - `administrative <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/administrative/>`__

    -

    - Y

    - Y

    - Partially changed.
      
      Changes to this element have been made to allow any number of
      administrative levels to be reported (as opposed to only two in versions
      up to 1.03) and for accurate encoding of these areas according to recognised
      vocabularies.
      
      Where possible, it is encouraged to include information on every
      possible administrative level and vocabulary simultaneously.

    - <administrative level="1" code="1453782" vocabulary="G1" />

      example with multiple administrative elements:
      
      <administrative vocabulary="GADM" level="1" code="8">Shinyanga</administrative>
      <administrative vocabulary="GADM" level="2" code="36">Kigoma Urban</administrative>
      <administrative vocabulary="GADM" level="3" code="771">Kigoma Bangwe</administrative>

  * -

    - @country

    - Y

    - N

    - Deprecated. Should no longer be used.

    - 

  * -
  
    - @adm1

    - Y

    - N

    - Deprecated. Should no longer be used.

    -

  * -

    - @adm2

    - Y

    - N

    - Deprecated. Should no longer be used.

    -

  * -

    - @code

    - N

    - Y

    - New. The code for the administrative area being reported from the
      vocabulary specified

    -

  * -
  
    - @level

    - N

    - Y

    - New. A number defining a subdivision within a hierarchical system of administrative areas. The precise system for defining the particular meaning of each @level value is determined by the @vocabulary being used.

    -

  * -
  
    - @vocabulary

    - N

    - Y

    - New. The code for a recognised administrative boundary repository from
      the new IATI
      `Geographic Vocabulary <http://iatistandard.org/codelists/GeographicVocabulary/>`__
      code list.

    -

  * -
  
    - @xml:lang

    - N

    - Y

    - New. The language of the description [only if different from default
      language]

    -

  * - `coordinates <http://iatistandard.org/105/activity-standard/iati-activities/iati-activity/location/coordinates/>`__

    -

    - Y

    - N

    - Deprecated. Should no longer be used.
      
      To align the geocoding standard with the more generic
      `Geographic Markup Language <http://www.opengeospatial.org/standards/gml>`__
      (GML) the Coordinates element has been replaced by the new Location /
      Point element

    - n/a

  * -
  
    - @latitude

    - Y

    - N

    - Deprecated. Remove and replace with new location/point/pos

    -

  * -
  
    - @longitude

    - Y

    - N

    - Deprecated. Remove and replace with new location/point/pos

    -

  * -
  
    - @precision

    - Y

    - N

    - Deprecated. Remove and replace with new location/exactness

    -

  * - `gazetteer-entry <http://iatistandard.org/105/activity-standard/iati-activities/iati-activity/location/gazetteer-entry/>`__

    -

    - Y

    - N

    - Deprecated. Should no longer be used.
      
      The location/gazetteer-entry element has been subsumed into the
      location/location-id element which identifies both gazetteer and
      administrative area vocabularies and codes.

    - n/a

  * -
  
    - @gazeteer-ref

    - Y

    - N

    - Deprecated. Should no longer be used.
      Remove and replace with the new location/location-id/@vocabulary

    -

  * -
  
    - (text)

    - Y

    - N

    - Deprecated. Should no longer be used.
      Remove and replace with the new location/location-id/@code

    -


Table 2: New location elements, introduced in version 1.04
----------------------------------------------------------

(Click on Element\* name link for official IATI Standard V1.04
definition and examples)

.. list-table::
  :header-rows: 1


  * - **Element**

    - **Attributes**

    - **In Use** **V1.03**

    - **In Use** **V1.04**

    - **Element Description**

    - **Example XML**

  * - `location <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/location-id/>`__\ `- <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/location-id/>`__\ `id <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/location-id/>`__

    -

    - N

    - Y

    - New. Allows for the reporting of an identifier for a location that is
      defined in a globally recognised third party system. Currently
      identifiers relating to gazetteers and sub-national administrative areas
      that are specified in the
      `Geographic Vocabulary codelist <http://iatistandard.org/codelists/GeographicVocabulary/>`__
      are catered for.

      This element replaces the gazetteer-entry element. For administrative
      areas this identifier should only be used if the location being defined
      is the administrative area itself. For describing the administrative
      area/s within which a location falls the location/administrative element
      should be used.

    - <location-id vocabulary="G1" code="1453782" />

  * -
  
    - @vocabulary

    - N

    - Y

    - New. A code from the new
      `Geographic Vocabulary <http://iatistandard.org/codelists/GeographicVocabulary/>`__
      code list

    -

  * -
  
    - @code

    - N

    - Y

    - New. The location code from the specified vocabulary

    -

  * - `activity-description <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/activity-description/>`__

    -

    - N

    - Y

    - New. Allows for a description of the activity taking place at a
      location, in addition to the description of the location itself (which
      should be reported in location/description). The element can be repeated
      for different languages.

    - <activity-description>A description that qualifies the activity taking
      place at the location</activity-description>

  * -
  
    - (text)

    - N

    - Y

    - New. The description of the activity taking place at this location

    -

  * - `location-reach <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/location-reach/>`__

    -

    - N

    - Y

    - New. Clarifies whether the location being described covers the activity
      itself, or the intended beneficiaries of the activity.

    - <location-reach code="1" />

  * -
  
    - @code

    - N

    - Y

    - New. A code from the new
      `Geographic Location Reach <http://iatistandard.org/codelists/GeographicLocationReach/>`__
      code list

    -

  * - `point <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/point/>`__

    -

    - N

    - Y

    - New. To align the geocoding standard with the more generic
      `Geographic Markup Language <http://www.opengeospatial.org/standards/gml>`__
      (GML) the Coordinates element has been replaced by the location/point
      element.

    - <point srsName="http://www.opengis.net/def/crs/EPSG/0/4326">

      <pos>31.616944 65.716944</pos>

      </point>

  * -
  
    - @srsName

    - N

    - Y

    - New. The name of the spatial reference system used by the coordinates.

      This should ALWAYS be: http://www.opengis.net/def/crs/EPSG/0/4326

    -

  * - `pos <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/point/pos/>`__
  
    -

    - N

    - Y

    - New. The latitude and longitude coordinates expressed as decimals and
      separated by a space, within a location/point element.

    - <point srsName="http://www.opengis.net/def/crs/EPSG/0/4326">

      <pos>31.616944 65.716944</pos>

      </point>

  * - `exactness <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/exactness/>`__

    -

    - N

    - Y

    - New. Defines whether the location represents the most distinct point
      reasonably possible for this type of activity or is an approximation due
      to lack of more detailed information.

      Replaces the location/coordinates/@precision attribute

    - <exactness code="1"/>

  * -
  
    - @code

    - N

    - Y

    - New. A code from the IATI
      `Geographic Exactness <http://iatistandard.org/codelists/GeographicExactness/>`__
      code list.

    -

  * - `location-class <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/location-class/>`__

    -

    - N

    - Y

    - New. Replaces the existing location-type element. It clarifies whether
      the location refers to a structure, a populated place (e.g. city or
      village), an administrative division, or another topological feature
      (e.g. river, nature reserve).

    - <location-class code="2"/>

  * -
  
    - @code

    - N

    - Y

    - New. A code from the new IATI
      `Geographic Location Class <http://iatistandard.org/codelists/GeographicLocationClass/>`__
      code list

    -

  * - `feature-designation <http://iatistandard.org/activity-standard/iati-activities/iati-activity/location/feature-designation/>`__

    -

    - N

    - Y

    - New. Allows for a more refined coded classification of the type of
      feature referred to by this location, making use of the USA National
      Geospatial-Intelligence Agency (NGA) list of feature designation codes.

    - <feature-designation code="PRNQ"/>

  * -
  
    - @code

    - N

    - Y

    - New. A feature designation code from
      `Location Type <http://iatistandard.org/codelists/LocationType/>`__
      code list

    -

XML Examples
------------

.. list-table::
  :header-rows: 1

  * - Version 1.03

    - Version 1.04

  * - .. code-block:: xml
  
          <location>
              <name>Herat</name>
              <description>Location description</description>
              <coordinates latitude="34.341944400000003000"
              longitude="62.203055599999971000" precision="2" />
              <gazetteer-entry gazeteer-ref="GEO">1140026</gazetteer-entry>
              <location-type code="PPL" />
              <administrative country="AF">Afghanistan, Herat, Injil</administrative>
          </location>
      
    - .. code-block:: xml
    
          <location ref="AF-KAN">
              <location-id vocabulary="G1" code="1453782" />
              <name>Location name</name>
              <description>Location description</description>
              <activity-description>A description that qualifies the activity taking place at the location</activity-description>
              <administrative level="1" code="1453782" vocabulary="G1" />
              <point srsName="http://www.opengis.net/def/crs/EPSG/0/4326">
                  <pos>31.616944 65.716944</pos>
              </point>
              <exactness code="1"/>
              <location-reach code="1" />
              <location-class code="2"/>
              <feature-designation code="PRNQ"/>
          </location>


  * -
      
    - Example multiple <administrative> elements:

      .. code-block:: xml
      
          <!-GADM Administrative Areas->
          <administrative vocabulary="GADM" level="1"
          code="8">Shinyanga</administrative>
          <administrative vocabulary="GADM" level="2" code="36">Kigoma
          Urban</administrative>
          <administrative vocabulary="GADM" level="3" code="771">Kigoma
          Bangwe</administrative>

          <!-GAUL Administrative Areas->
          <administrative vocabulary="GAUL" level="1"
          code="48362">Kigoma</administrative>
          <administrative vocabulary="GAUL" level="2" code="48412">Kigoma
          Urban</administrative>
          <administrative vocabulary="GAUL" level="3"
          code="49196">Gungu</administrative>
      
          <!-OSM Administrative Areas->
          <administrative vocabulary="OSM" level="5"
          code="1600842">Kigoma</administrative>
