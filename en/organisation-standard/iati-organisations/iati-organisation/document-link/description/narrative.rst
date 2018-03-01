Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``description`` element.

.. literalinclude:: ../../../../organisation-standard-example-annotated.xml
    :language: xml
    :start-after: <!--document-link starts-->
    :end-before: <!--document-link ends-->

  | The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-organisation``, by using the ``xml:lang`` attribute.

  | Note: This relates to the language of the text in the XML.

Changelog
~~~~~~~~~

2.03
^^^^
| This mandatory ``narrative`` element of a ``description`` in a ``document-link`` element was `added <https://discuss.iatistandard.org/t/document-link-description-included-2-03/841>`__.
