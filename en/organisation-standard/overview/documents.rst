Documents
=========

Definition
----------
Within the **IATI organisation standard** any number of links to relevant *documents* can be declared using:

* ``document-link`` - a categorized link to an external document.


Considerations
--------------
When declaring various *documents* in the **IATI organisation standard** the following should be considered:

* In the **IATI organisation standard**, documents that relate to the organisation/agency would be referred to.  Activity/project specific documents are published via the IATI activity standard.

* All ``document-link`` should be presented as in the form of URLs (eg: http://example.org/exampledocument.odt)

* The URL must resolve to a valid internet address that provides direct access to the document in question.

* Attention should be paid by the publisher to any links that become obsolete

* The same document can be presented in different languages via separate ``document-link`` elements.

* For every document presented either a ``title`` or ``category`` is expected (or both)

* For document ``category`` in the **IATI organisation standard**, it is expected that the ``DocumentCategory`` code would be have the B prefix

* Using the ``format`` attribute helps inform what to expect from the document

* Use of the ``format`` must be accompanied by a code on the ``FileFormat`` codelist.

Further guidance
----------------

* :doc:`document-link </organisation-standard/iati-organisations/iati-organisation/document-link/>`
