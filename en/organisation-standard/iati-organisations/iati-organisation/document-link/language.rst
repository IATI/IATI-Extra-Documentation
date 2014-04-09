Example Usage
~~~~~~~~~~~~~
The code should be declared in any usage of this element:

.. code-block:: xml

        <language code="en"/>
        <language code="fr"/>

Additionally, a text description of the code can be provided:

.. code-block:: xml

        <language code="en">English</language>
        <language code="fr">Francais</language>

Full example:

    <document-link format="vnd.oasis.opendocument.text" url="http:www.example.org/docs/report_fr.odt">
      <category code="B01"/>
      <language code="fr"/>
      <title>Rapport annuel 2013</title>
    </document-link>


Changelog
~~~~~~~~~

1.02
^^^^

Addition of a language element as a child of the document-link element:
document-link/language/text() (0..1) - The ISO 639 code for the language
of the document

1.01
^^^^

This element did not exist
