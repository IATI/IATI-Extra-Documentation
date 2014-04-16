Related Documents
=================

Definition
----------
Within the **IATI activity standard** any number of links to supporting documents can be declared.

In the **IATI activity standard**, documents that relate to the specific activity would be referred to.  Organisation/agency specific documents are published via the IATI activity standard.

The main element for this is:

* ``document-link`` - providing a categorised link to an external document.

Additionally, the following also enable the links to external resources:

* ``activity-website``  - a website that provides more information about the specific ``iati-activity``
* linked data - declaring the path at which information on this activity is available as linked-date

Considerations
--------------
All documents should be presented as links in the form of URLs (eg: http://example.org/exampledocument.odt)

The URL must resolve to a valid internet address that provides direct access to the document in question

Attention should be paid by the publisher to any links that become obsolete

The same document can be presented in different languages via separate ``document-link`` elements.

For every document presented either a ``title`` or ``category`` is expected (or both)

For document ``category`` in the activity standard, it is expected that the ``DocumentCategory`` code would be have the A prefix

Use of the ``format`` attribute help inform what to expect from the document

Although many different kinds of ``format`` can be presented, it is recommended to utilise the ones represented in the ``FileFormat`` codelist

The ``activity-website`` should be a URL to a page or website that is specifically about the ``iati-activity`` - not generic information.



Further guidance
----------------

* :doc:`document-link </activity-standard/iati-activities/iati-activity/document-link/>`
