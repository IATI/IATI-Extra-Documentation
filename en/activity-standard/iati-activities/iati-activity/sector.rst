Example Usage
~~~~~~~~~~~~~
Example ``sector`` of an ``iati-activity``.

| The ``@vocabulary`` attribute declares a valid code (*2*) from the *SectorVocabulary* codelist.
| An example value *111* from this vocabulary is declared with the ``@code`` attribute.

.. code-block:: xml

	<sector vocabulary="2" code="111" />
	
| The ``sector`` element can be repeated in any ``iati-activity``.        
| When multiple ``sector`` are declared, then the ``@percentage`` values should sum to 100% for the specific ``iati-activity``.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--sector starts-->
	:end-before: <!--sector ends-->
    
| The ``vocabulary`` is used to declare which ``SectorVocabulary`` classification list is in use. If this is omitted, then IATI assumes a *SectorVocabulary* of *1* (OECD DAC CRS Purpose Codes (5 digit)).

| If a vocabulary is not on the *SectorVocabulary* codelist, then the value of *99* or *98* (Reporting Organisation) should be declared.

| If a publisher uses a vocabulary of 98 or 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:

.. code-block:: xml

    <sector vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="A1" />


Changelog
~~~~~~~~~

2.02
^^^^
The ``vocabulary-uri`` attribute was `added <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__.

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element, but only in particular use-cases.

1.03
^^^^
Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
