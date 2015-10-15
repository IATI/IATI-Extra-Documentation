Related Documents
=================

Definition
----------
Within the **IATI activity standard** any number of links to supporting documents can be declared.

The main element for this is:

* ``document-link`` - a categorized link to an external document.

The following also enable the links from the ``iati-activity`` to external resources:

* linked data - declaring the path at which information on the specific ``iati-activity`` is available as linked-data


Considerations
--------------
When using the **IATI activity standard** to declare *related documents*, the following should be considered:

* All ``document-link`` should be presented in the form of URLs (eg: http://example.org/exampledocument.odt)
* The URL must resolve to a valid internet address that provides direct access to the document in question.
* Attention should be paid by the publisher to any links that become obsolete.
* If the documents are in different languages, which are available at different URLs, then repeat the ``document-link`` element
* If the same document has multiple languages within it, then repeat the ``language`` element.
* For every document presented a ``title`` and at least one ``category`` is required
* The ``title`` element can be repeated for different languages, regardless of the language of the actual document.
* The free-text instances of ``title`` should avoid use of text in CAPITALS, where possible.
* In the **IATI activity standard**, documents that relate to the specific ``iati-activity`` would be linked to.  Organisation/agency specific documents are published via the **IATI organisation standard**.
* For document ``category`` in the **IATI activity standard**, it is expected that the *DocumentCategory* code would be have the *A* prefix.
* When a document has multiple categories, then the ``category`` element can be repeated.
* Using the ``@format`` attribute helps inform what to expect from the document.
* Use of the ``@format`` must be accompanied by a code on the ``FileFormat`` codelist.
* The ``document-date/@iso-date`` would normally be the production or published date of the relevant document to identify the specific document version.


2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* The schema data type used for some data fields where a URL is expected is now set as *xsd:anyURI*.
* The ``activity-website`` element has been removed.  These can now be expressed as a ``document-link`` with the relevant *FileFormat* and *DocumentType* codes.
* Any freetext title must be included in the child ``narrative`` element, which can be repeated for different languages. 
