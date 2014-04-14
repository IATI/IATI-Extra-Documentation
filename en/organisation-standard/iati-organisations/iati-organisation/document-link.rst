Example Usage
~~~~~~~~~~~~~
Example of an annual report link. 
Please note that B type ``DocumentCategory`` codes are used within ``iati-organisation`` documents.

.. code-block:: xml

    <document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_en.odt">
      <category code="B01"/>
	  <language code="en"/>
      <title>Annual report 2013</title>
    </document-link>

The ``language`` element can be used to declare the language of documents.  
    
.. code-block:: xml
 
    <document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_fr.odt">
      <category code="B01"/>
      <language code="fr"/>
      <title>Rapport annuel 2013</title>
    </document-link>

Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new language child element to, the document-link element.

1.01
^^^^

See previous version on the IATI Standard
`wiki <http://wiki.iatistandard.org/standard/documentation/1.0/document-link>`__
and
`website <http://iatistandard.org/101/activities-standard/related-documents/activity-documents/>`__
