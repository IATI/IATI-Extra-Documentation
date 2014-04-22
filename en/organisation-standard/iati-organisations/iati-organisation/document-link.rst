Example Usage
~~~~~~~~~~~~~
Example of an annual report link. 
Note: ``DocumentCategory`` codes with the B prefix are recommended within ``iati-organisation`` ``document-link`` elements.

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

Note: the same ``document-link`` element can be repeated for different ``language``.

.. code-block:: xml

    <document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_en.odt">
      <category code="B01"/>
	  <language code="en"/>
      <title>Annual report 2013</title>
    </document-link>
    <document-link format="application/vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_fr.odt">
      <category code="B01"/>
      <language code="fr"/>
      <title>Rapport annuel 2013</title>
    </document-link>

Changelog
~~~~~~~~~

1.02
^^^^

Removed language attribute from, and introduced an new ``language`` child element to, the ``document-link`` element.

