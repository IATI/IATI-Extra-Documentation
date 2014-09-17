Example Usage
~~~~~~~~~~~~~
Example usage of ``iati-activities``. 
| 
| This element is a parent for other all other elements of the **IATI Activity Standard**.
|
| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``generated-datetime`` attribute.  
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example date time format conforms to the xsd:dateTime standard.
| 
| A ``Version`` code of *2.01* is declared using the ``version`` attribute.
| The optional ``linked-data-default`` attribute is also included.

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
