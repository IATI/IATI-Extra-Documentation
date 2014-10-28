Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` of an ``iati-activity``. 

| The ``@code`` attribute declares a valid code (*489*) from the *Region* codelist.
| The optional ``@vocabulary`` attribute declares a valid code (*1*) from the *RegionVocabulary* codelist.

.. code-block:: xml

	<recipient-region code="489" vocabulary="1" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 18

Changelog
~~~~~~~~~

2.01
^^^^
The ``sector`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#transaction-new-child-elements>`__ as a child element of ``transaction``.
