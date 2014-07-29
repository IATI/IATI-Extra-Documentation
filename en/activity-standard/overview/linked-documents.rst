Related Documents
=================

Definition
----------
Within the **IATI activity standard** any number of links to supporting documents can be declared.

The main element for this is:

* ``document-link`` - a categorized link to an external document.

The following also enable the links from the ``iati-activity`` to external resources:

* ``activity-website``  - a website that provides more information about the specific ``iati-activity``
* linked data - declaring the path at which information on the specific ``iati-activity`` is available as linked-data


Considerations
--------------
When using the **IATI activity standard** to declare *documents*, the following should be considered:

* All ``document-link`` should be presented in the form of URLs (eg: http://example.org/exampledocument.odt)
* The URL must resolve to a valid internet address that provides direct access to the document in question.
* Attention should be paid by the publisher to any links that become obsolete.
* The same document can be presented in different languages via separate ``document-link`` elements.
* For every document presented either a ``title`` or ``category`` is expected (or both).
* The ``title`` element can be repeated for different languages, regardless of the language of the actual document.
* The free-text instances of ``title`` should avoid use of text in CAPITALS, where possible.
* In the **IATI activity standard**, documents that relate to the specific ``iati-activity`` would be linked to.  Organisation/agency specific documents are published via the **IATI organisation standard**.
* For document ``category`` in the **IATI activity standard**, it is expected that the ``DocumentCategory`` code would be have the A prefix.
* Using the ``format`` attribute helps inform what to expect from the document.
* Use of the ``format`` must be accompanied by a code on the ``FileFormat`` codelist.
* The ``activity-website`` should be a URL to a page or website that is specifically about the ``iati-activity`` - not generic information (eg: http://www.example.com/en/activity/ABC123).

