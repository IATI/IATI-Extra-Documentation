Example Usage
~~~~~~~~~~~~~
Example ``policy-marker`` of an ``iati-activity``.

| This example declares a ``PolicyMarkerVocabulary`` code *1* (*OECD DAC CRS*), using the ``code`` attribute.
| A ``PolicyMarker`` code *2* is declared with the ``code`` attribute, 
| A ``PolicySignificance`` code of *3* with the ``significance`` attribute.
 
.. code-block:: xml

	<policy-marker vocabulary="1" code="2" significance="3" />

| The ``policy-marker`` element can be repeated in any ``iati-activity``.  

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--policy-marker starts-->
	:end-before: <!--policy-marker ends-->

| If a vocabulary is not on the ``Vocabulary`` codelist, then the value of *99* (*Reporting Organisation*) should be declared.	
	
	
