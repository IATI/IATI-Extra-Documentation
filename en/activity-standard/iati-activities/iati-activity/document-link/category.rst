Example Usage
~~~~~~~~~~~~~
| Example  usage of ``category`` of a ``document-link`` in an ``iati-activity``.

| This examples declares the ``DocumentCategory`` code *A01*, using the ``@code`` attribute.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--document-link starts-->
	:end-before: <!--document-link ends-->
	:emphasize-lines: 6

| The ``category`` element can be repeated in any ``document-link``.		

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.
