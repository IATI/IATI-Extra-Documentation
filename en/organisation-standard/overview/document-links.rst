Documents
=========

Definition
----------
Within the IATI organisation standard any number of links to supporting documents can be declared.

In the IATI organisations standard, documents that relate to the organisation/agency would be refered to.  Activity/project specific documents are published via the IATI activity standard.


Considerations
--------------
All documents should be presented as links in the form of URLs (eg: http://example.org/exampledocument.odt)

The URL must resolve to a valid internet address that provides direct access to the document in question

Attention should be paid by the publisher to any links that become obsolete

The same document can be presented in different languages via seperate ``document-link`` elements.

For every document presented either a ``title`` or ``category`` is expected (or both)

For document ``category`` in the organisation standard, it is expected that the ``DocumentCategory`` code would be have the B prefix

Use of the ``format`` attribute help inform what to expect from the document

Although many different kinds of ``format`` can be presented, it is recommended to utilise the ones represented in the ``FileFormat`` codelist


Further guidance
----------------
*``document-link``
