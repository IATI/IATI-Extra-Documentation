Example Usage
~~~~~~~~~~~~~
Example of ``iati-activity`` with ``last updated-datetime`` of on 2nd September 2014.

| This element is a parent for other child elements.

| This example declares a ``Language`` as *en* (*English*) with the ``xml:lang`` attribute.

| A ``Currency`` of *EUR* (*Euros*) is set with the ``default-currency`` attribute.  

| An optional attribute of ``hierarchy`` is set as *1*

| A further optional attribute ``linked-data-uri`` is also included:

.. literalinclude:: ../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-activity starts-->
	:end-before: <!--iati-identifier starts-->

The ``iati-activity`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: ../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--fss ends-->	
	:end-before: <!--iati-activity ends-->
	
Changelog
~~~~~~~~~
2.01
^^^^
The ``version`` attribute was removed in 2.01

1.02
^^^^

Introduced the ``linked-data-uri`` attribute on iati-activity element

1.01
^^^^

See previous version on the IATI Standard
`wiki <http://wiki.iatistandard.org/standard/documentation/1.0/iati-activity>`__
and
`website <http://iatistandard.org/101/activity-standard/container-elements/record-header/>`__
