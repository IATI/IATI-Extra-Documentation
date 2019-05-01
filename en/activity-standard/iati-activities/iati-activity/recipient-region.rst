Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` of an ``iati-activity``. 

| The ``@code`` attribute declares a valid code (*489*) from the *Region* codelist.
| The optional ``@vocabulary`` attribute declares a valid code (*1*) from the *RegionVocabulary* codelist.

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />

| The ``recipient-region`` element can be repeated in any ``iati-activity``.

| When multiple ``recipient-region`` are declared, then the ``@percentage`` values should sum to 100% per vocabulary for the specific ``iati-activity``.
        
.. code-block:: xml

	<recipient-region code="489" vocabulary="1" percentage="50" />
	<recipient-region code="389" vocabulary="1" percentage="50" />

| When both the ``recipient-region`` and ``recipient-country`` are declared, then the ``@percentage`` values should sum to 100% per region vocabulary for the specific ``iati-activity``.

.. code-block:: xml

	<recipient-country code="AF" percentage="50" />
	<recipient-region code="489" vocabulary="1" percentage="50" />
	<recipient-region code="A1" vocabulary="99" percentage="50" vocabulary-uri="http://example.com/vocab.html" />
	
	
Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element, but only in particular use-cases.

1.03
^^^^
Where used, the ``@percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
