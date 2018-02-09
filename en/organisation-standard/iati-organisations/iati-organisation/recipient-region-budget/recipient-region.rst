Example Usage
~~~~~~~~~~~~~
Example usage of ``recipient-region`` in context of ``recipient-region-budget`` element:

| The ``@code`` attribute declares a valid code (*489*) from the *Region* codelist.
| The optional ``@vocabulary`` attribute declares a valid code (*1*) from the *RegionVocabulary* codelist.

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />

If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:
.. code-block:: xml

	<recipient-region code="A1" vocabulary="99" vocabulary-uri="http://example.com/vocab.html" />

Example of ``recipient-region`` in context of a complete ``recipient-region-budget`` element:

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-region-budget starts-->
	:end-before: <!--recipient-region-budget ends-->

Changelog
~~~~~~~~~
2.02
^^^^
The optional ``recipient-region-budget`` element was `added <http://support.iatistandard.org/entries/79323113-Org-Standard-recipient-region-budget>`__.
