Example Usage
~~~~~~~~~~~~~
Example of ``iati-activity`` with ``last updated-datetime`` of on 6th May 2014. 
Language set as *en* (English) and a ``default-currency`` to *EUR* (Euros).  
The optional ``version`` of *1.04* is also stated.
The optional ``linked-data-uri`` attribute, introduced in the decimal upgrade 1.02, is also included:

.. literalinclude:: ../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--iati-activity starts-->
	:end-before: <!--reporting-org starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: ../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--crs-add ends-->	
	:end-before: <!--iati-activity ends-->
	
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
