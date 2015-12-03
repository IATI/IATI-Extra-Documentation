Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` of an ``iati-activity``. 

| The ``@code`` attribute declares a valid code (*489*) from the *Region* codelist.
| The optional ``@vocabulary`` attribute declares a valid code (*1*) from the *RegionVocabulary* codelist.

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />


If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:

.. code-block:: xml

	<recipient-region code="A1" vocabulary="99" vocabulary-uri="http://example.com/vocab.html" />

Please note, if using your own vocabulary (i.e. code 99), it is recommended that this is used in addition to the DAC OECD region vocabulary (code 1).

| The ``recipient-region`` element can be repeated in any ``iati-activity``.

| When multiple ``recipient-region`` are declared, then the ``@percentage`` values should sum to 100% for the specific ``iati-activity``.
        
.. code-block:: xml

	<recipient-region code="489" vocabulary="1" percentage="50" />
	<recipient-region code="389" vocabulary="1" percentage="50" />

| When both the ``recipient-region`` and ``recipient-country``, then the ``@percentage`` values should sum to 100% for the specific ``iati-activity``.

.. code-block:: xml

	<recipient-country code="AF" percentage="50" />
	<recipient-region code="489" vocabulary="1" percentage="50" />
	
	
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
Where used, the ``@percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
