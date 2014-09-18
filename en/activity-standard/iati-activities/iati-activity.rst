Example Usage
~~~~~~~~~~~~~
Example of ``iati-activity``.
| 
| This element is a parent for other child elements.
| 
| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``last-updated-datetime`` attribute.  
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example date time format conforms to the xsd:dateTime standard.
| 
| This example declares a ``Language`` as *en* (*English*), using the ``xml:lang`` attribute.
| This example declares a ``Currency`` code of *USD*, using the ``default-currency`` attribute.  
| An optional attribute of ``hierarchy`` is set as *1*
| The optional attribute ``linked-data-uri`` is also included.

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
