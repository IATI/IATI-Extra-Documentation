Humanitarian Reporting
======================

Definition
----------
Within the **IATI activity** standard there are a number of elements and vocabularies that enable humanitarian specific information to be published.

* ``humanitarian-scope`` defines the emergency or event that a specific activity is in response to.

The ``humanitarian-scope`` element uses the following vocabularies:

* ``HumanitarianScopeType`` codelist is used to describe types of humanitarian events.
* ``HumanitarianScopeVocabulary`` is used to define the public list(s) on which an emergency is referenced.

Humanitarian related information is also on:

* ``SectorVocabulary`` –  code ``"10"``: The Humanitarian Global Clusters (Inter-Agency Standing Committee) defines the global clusters to which a a specific activity relates.
* ``PolicyMarkerVocabulary`` - code ``"2"`` defines the list of UNOCHA humanitarian policies to which a specific activity relates.

The following also enables any activity or transaction that is humanitarian related to be identified:

* The ``iati-activity``/``@humanitarian`` – indicates that the relevant ``iati-activity``  is humanitarian-related.
* ``transaction``/``@humanitarian`` – indicates that a specific ``transaction``  is humanitarian-related.


Considerations
--------------
When using the IATI activity standard to declare humanitarian related activities the following should be considered:

* It is the data owner who decides if an activity should include humanitarian elements.
* It is recommended that at least the ``humanitarian-scope`` element and  ``iati-activity``/``@humanitarian``  attribute should be used for each humanitarian related activity.
* If the emergency is included on more than one on of the lists defined on HumanitarianScopeVocabulary then all references should be declared via multiple ``humanitarian-scope`` elements.
* The title of an emergency can be repeated in different languages via the use of the  ``<narrative>``  field of the ``humanitarian-scope`` element.
* If an emergency is not defined on any of the lists included on HumanitarianScopeVocabulary then a publisher can declare their own values using code ‘99’. It is recommended that the title of an emergency is constructed using the format ‘location of event + type of event + month of event + year of event’ eg ‘Nepal Earthquake April 2015’.
* When an activity relates to multiple clusters the ``sector`` element should be repeated and a ``@percentage`` attribute must be used. The total of all specified percentages must add up to 100.
* When an activity relates to multiple humanitarian policies the ``policy-marker`` element should be repeated.
* When defining a humanitarian ``policy-marker`` element, the ``policy-marker``/``@significance`` attribute is not required.
