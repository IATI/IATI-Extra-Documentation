Example Usage
~~~~~~~~~~~~~
Example ``policy-marker`` of an ``iati-activity``.

| The ``@vocabulary`` attribute declares a valid code (*1*) from the *PolicyMarkerVocabulary* codelist.
| The ``@code`` attribute declares a valid code (*1*) from the *PolicyMarker* codelist.
| The ``@significance`` attribute declares a valid code (*3*) from the *PolicySignificance* codelist.
 
.. code-block:: xml

	<policy-marker vocabulary="1" code="2" significance="3" />

If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:
.. code-block:: xml

	<policy-marker vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="A1" significance="3" />

| The ``policy-marker`` element can be repeated in any ``iati-activity``.  

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--policy-marker starts-->
	:end-before: <!--policy-marker ends-->

| If a vocabulary is not on the *PolicyMarkerVocabulary* codelist, then the value of *99* (*Reporting Organisation*) should be declared.	

Changelog
~~~~~~~~~

2.02
^^^^
The ``vocabulary-uri`` attribute was `added <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__.

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element, but only in particular use-cases.
	
	
