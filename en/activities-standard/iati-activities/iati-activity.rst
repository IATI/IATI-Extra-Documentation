Example Usage
~~~~~~~~~~~~~
Activity last updated on 3rd March 2014, with a ``hierarchy`` value of 1. Default language of English (``en``) and a ``default-currency`` of Euros.

.. code-block:: xml

     <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" hierarchy="1" xml:lang="en">
           ....
     </iati-activity>


An IATI ``version`` is included. 

.. code-block:: xml

     <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" hierarchy="1" version="1.04">
           ....
     </iati-activity>

Inclusion of ``linked-data-uri`` attribute, introduced in the decimal upgrade 1.02.

.. code-block:: xml

     <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" hierarchy="1" version="1.04" linked-data-uri="http://data.example.org/123456789">
           ....
     </iati-activity>

Changelog
~~~~~~~~~

1.02
^^^^

Introduced the ``linked-data-uri`` attribute on iati-activity element

1.01
^^^^

See previous version on the IATI Standard
`wiki <http://wiki.iatistandard.org/standard/documentation/1.0/iati-activity>`__
and
`website <http://iatistandard.org/101/activities-standard/container-elements/record-header/>`__
