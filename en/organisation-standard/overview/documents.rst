Documents
=========

*Please note: these overview pages are currently being updated for the `final release of version 2.01 of the IATI standard <https://github.com/IATI/IATI-Extra-Documentation/milestones/2.01%20Release%20Date>`__ *.

Definition
----------
Within the **IATI organisation standard** any number of links to relevant *documents* can be declared using:

* ``document-link`` - a categorized link to an external document.


Considerations
--------------
When using the **IATI organisation standard** to declare *documents*, the following should be considered:

* In the **IATI organisation standard**, documents that relate to the organisation/agency would be linked to.  ``iati-activity`` specific documents are published via the **IATI activity standard**.
* All ``document-link`` should be presented in the form of URLs (eg: http://example.org/exampledocument.odt)
* The URL must resolve to a valid internet address that provides direct access to the document in question.
* Attention should be paid by the publisher to any links that become obsolete.
* The same document can be presented in different languages via separate ``document-link`` elements.
* For every document presented either a ``title`` or ``category`` is expected (or both).
* The ``title`` element can be repeated for different languages, regardless of the language of the actual document.
* The free-text instances of ``title`` should avoid use of text in CAPITALS, where possible.
* For document ``category`` in the **IATI organisation standard**, it is expected that the ``DocumentCategory`` code would be have the B prefix.
* ``DocumentCategory`` code A documents should only be reported if there is a good reason for the document not to be linked to a specific ``iati-activity``.
* Using the ``format`` attribute helps inform what to expect from the document.
* Use of the ``format`` must be accompanied by a code on the ``FileFormat`` codelist.

