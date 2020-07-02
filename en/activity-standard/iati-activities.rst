Example Usage
~~~~~~~~~~~~~
Example of ``iati-activities`` with ``generated-datetime`` of on 6th May 2014.

The ``version`` of *1.04* of the **IATI activity standard** is stated.

The optional ``linked-data-default`` is also included

.. literalinclude:: activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-activities starts-->
	:end-before: <!--iati-activity starts-->

The ``iati-activities`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-activity ends-->
	:end-before: <!--iati-activities ends-->

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
`website <http://iatistandard.org/101/activity-standard/container-elements/file-header/>`__

.. meta::
  :order: 0
