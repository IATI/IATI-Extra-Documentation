Example Usage
~~~~~~~~~~~~~
Example ``humanitarian-scope`` of an ``iati-activity``.

| The ``@type`` attribute declares a valid code (*1*) from the *HumanitarianScopeType* codelist.
| The ``@vocabulary`` attribute declares a valid code (*1-2*) from the *HumanitarianScopeVocabulary* codelist.
| The ``@code`` attribute declares a valid code (*EQ-2015-000048-NPL*) from the specified vocabulary.
 
.. code-block:: xml

	<humanitarian-scope type="1" vocabulary="1-2" code="EQ-2015-000048-NPL">
	...
	</humanitarian-scope>

If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:

.. code-block:: xml

	<humanitarian-scope type="1" vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="5">
	  <narrative>Nepal Earthquake (April 2015)</narrative>
	</humanitarian-scope>


| The ``humanitarian-scope`` element can be repeated in any ``iati-activity``.  

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--humanitarian-scope starts-->
	:end-before: <!--humanitarian-scope ends-->
	:emphasize-lines: 1, 2, 4

| If a vocabulary is not on the *HumanitarianScopeVocabulary* codelist, then the value of *99* (*Reporting Organisation*) should be declared.	

Changelog
~~~~~~~~~

2.02
^^^^
The ``humanitarian-scope`` element was `added <http://support.iatistandard.org/entries/105778163-Humanitarian-Emergencies-and-Appeals>`__.
