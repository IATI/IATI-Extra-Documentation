Example Usage
~~~~~~~~~~~~~
Example ``other-identifier`` of an ``iati-activity``.

| An example ``@ref`` of *ABC123-XYZ* is declared.
| The ``@type`` attribute declares a valid code (*A1*) from the *OtherIdentifierType* codelist.
 
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--other-identifier starts-->
	:end-before: <!--other-identifier ends-->
	:emphasize-lines: 1, 5	

2.01
^^^^
| Freetext support of the ``other-identifier`` was removed.  A new ``other-identifier/@ref`` was `added as a replacement <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#other-identifier-removed-new-attributes>`__.

| A new attribute ``other-identifier/@type`` was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#other-identifier-removed-new-attributes>`__, to be used with new code list *OtherIdentifierType*.

| The ``other-identifier/@owner-ref`` and ``other-identifier/@owner-name`` attributes were `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#other-identifier-removed-new-attributes>`__.

| The ``owner-org`` child element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/##other-identifier-new-child-elements>`__.
