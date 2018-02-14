Example Usage
~~~~~~~~~~~~~
| Example  usage of ``category`` of a ``document-link`` in an ``iati-organisation``.

| This examples declares the ``DocumentCategory`` code *B01*, using the ``@code`` attribute.

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->

| The ``category`` element can be repeated in any ``document-link``.
| Example declaring multiple ``DocumentCategory`` codes for the same ``document-link``:

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-cat-document-link starts-->
	:end-before: <!--multi-cat-document-link ends-->

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.
