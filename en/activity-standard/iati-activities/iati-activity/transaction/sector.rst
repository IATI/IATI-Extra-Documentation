Example Usage
~~~~~~~~~~~~~
Example ``sector`` of a ``transaction`` within an ``iati-activity``.

| The ``@vocabulary`` attribute declares a valid code (*2*) from the *SectorVocabulary* codelist.
| An example value *111* from this vocabulary is declared with the ``@code`` attribute.

.. code-block:: xml

	<sector vocabulary="2" code="111" />
        
| The ``sector`` element can be repeated in any ``transaction``. 
  
| The ``vocabulary`` is used to declare which ``SectorVocabulary`` classification list is in use. If this is omitted, then IATI assumes a *SectorVocabulary* of *1* (OECD DAC CRS Purpose Codes (5 digit)).

| If a vocabulary is not on the *SectorVocabulary* codelist, then the value of *99* or *98* (Reporting Organisation) should be declared.

| If a publisher uses a vocabulary of 98 or 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:
.. code-block:: xml

    <sector vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="A1" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 15

Changelog
~~~~~~~~~

2.02
^^^^
The ``vocabulary-uri`` attribute was `added <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__.

2.01
^^^^
The ``sector`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#transaction-new-child-elements>`__ as a child element of ``transaction``.
