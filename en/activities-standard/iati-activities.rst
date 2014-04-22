Example Usage
~~~~~~~~~~~~~
Example generated on 3rd March 2014 and uses ``version`` 1.04:

.. code-block:: xml

        <iati-activities generated-datetime="2014-04-03T18:27:37" version="1.04">
           ....
        </iati-activities>

With the optional ``linked-data-default`` attribute, introduced in decimal upgrade 1.02

.. code-block:: xml

        <iati-activities generated-datetime="2014-04-03T18:27:37" version="1.04" linked-data-default="http://data.example.org/">
           ....
        </iati-activities>

Changelog
~~~~~~~~~

1.02
^^^^

Introduced the ``linked-data-default`` attribute on ``iati-activities`` element

1.01
^^^^

See previous version on the IATI Standard
`wiki <http://wiki.iatistandard.org/standard/documentation/1.0/iati-activities>`__
and
`website <http://iatistandard.org/101/activities-standard/container-elements/file-header/>`__
