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

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->

Changelog
~~~~~~~~~

2.02
^^^^
The ``vocabulary-uri`` attribute was `added <http://support.iatistandard.org/entries/105713163-Add-URI-attribute-to-elements-where-Reporting-organisation-vocabularies-are-used>`__.

2.01
^^^^
The ``sector`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#transaction-new-child-elements>`__ as a child element of ``transaction``.
