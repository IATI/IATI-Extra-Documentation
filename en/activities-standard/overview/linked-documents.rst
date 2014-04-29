Related Documents
=================

Definition
----------
Within the **IATI activity standard** any number of links to supporting documents can be declared.

| In the **IATI activity standard**, documents that relate to the specific activity would be referred to.  Organisation/agency specific documents are published via the IATI activity standard.

| The main element for this is:

* ``document-link`` - a categorized link to an external document.

| Additionally, the following also enable the links from the ``iati-activity`` to external resources:

* ``activity-website``  - a website that provides more information about the specific ``iati-activity``
* linked data - declaring the path at which information on the specific ``iati-activity`` is available as linked-data

Considerations
--------------
When using the **IATI activity standard** to declare *documents*,  the following should be considered:

* In the **IATI activity standard**, documents that relate to the specific ``iati-activity`` would be linked to.  Organisation/agency specific documents are published via the **IATI organisation standard**.

* All ``document-link`` should be presented as in the form of URLs (eg: http://example.org/exampledocument.odt)

* The URL must resolve to a valid internet address that provides direct access to the document in question.

* Attention should be paid by the publisher to any links that become obsolete.

* The same document can be presented in different languages via separate ``document-link`` elements.

* For every document presented either a ``title`` or ``category`` is expected (or both).

* The free-text instances of ``title`` should avoid use of text in CAPITALS, where possible.

* For document ``category`` in the **IATI organisation standard**, it is expected that the ``DocumentCategory`` code would be have the B prefix.

* Using the ``format`` attribute helps inform what to expect from the document.

* Use of the ``format`` must be accompanied by a code on the ``FileFormat`` codelist.

* The ``activity-website`` should be a URL to a page or website that is specifically about the ``iati-activity`` - not generic information (eg: http://www.example.com/en/activity/ABC123).


Further guidance
----------------

Reference pages:

* :doc:`document-link </activity-standard/iati-activities/iati-activity/document-link/>`
* :doc:`activity-website/ </activities-standard/iati-activities/iati-activity/activity-website/>`

* :doc:`iati-activities </activities-standard/iati-activities/>`
* :doc:`iati-activity </activities-standard/iati-activities/iati-activity/>`
