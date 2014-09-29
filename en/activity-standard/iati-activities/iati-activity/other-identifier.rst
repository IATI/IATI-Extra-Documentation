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
| Freetext support of the ``other-identifier`` was removed.  A new ``other-identifier/@ref`` was added as a replacement.

| A new attribute ``other-identifier/@type`` was introduce in 2.01, to be used with new code list ``OtherIdentifierType``.

| The ``other-identifier/@owner-ref`` and ``other-identifier/@owner-ref`` attributes were removed in 2.01.

| The ``owner-org`` child element was added in version 2.01.
