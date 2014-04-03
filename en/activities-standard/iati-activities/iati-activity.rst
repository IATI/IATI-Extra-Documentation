
Usage
~~~~~~~~~~~~~

This example declares that the activity has a default language of English (``en``) and a default currency of Euros. It was last updated
on the 3rd March 2014, and has a hierarchy value of 1.

.. code-block:: xml

     <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" hierarchy="1" xml:lang="en">
           ....
     </iati-activity>

Additional attributes
~~~~

An IATI ``version`` can be declared. NB: This would already be within the ``iati-activities`` element, but can be used if the particular activity differs.

.. code-block:: xml

     <iati-activity default-currency="EUR" last-updated-datetime="2014-04-03T18:27:37" hierarchy="1" version="1.04">
           ....
     </iati-activity>

This example includes the linked-data-uri attribute, introduced in the decimal upgrade 1.02.  This can be used to override ``iati-activities/@linked-data-default``.

.. code-block:: xml

     <iati-activity xml:lang="en" default-currency="USD" last-updated-datetime="2012-03-31T01:01:01" hierarchy="1" version="1.01" linked-data-uri="">
           ....
     </iati-activity>

Changelog
~~~~~~~~~

1.02
^^^^

Introduced the @linked-data-uri attribute on iati-activity element

1.01
^^^^

See previous version on the IATI Standard
`wiki <http://wiki.iatistandard.org/standard/documentation/1.0/iati-activity>`__
and
`website <http://iatistandard.org/101/activities-standard/container-elements/record-header/>`__
