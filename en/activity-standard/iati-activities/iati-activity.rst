Example Usage
~~~~~~~~~~~~~
Example of ``iati-activity``.

| This element is a parent for other child elements.

| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``@last-updated-datetime`` attribute.  
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example date time format conforms to the *xsd:dateTime* standard.

| The ``@xml:lang`` attribute declares a valid code (*en*) from the *Language* codelist.
| The ``@default-currency`` attribute declares a valid code (*USD*) from the *Currency* codelist.

| The optional ``@hierarchy`` attribute of  is set as *1*
| The optional ``@linked-data-uri`` attribute  is also included.

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

2.02
^^^^
| The ``humanitarian`` attribute was `added <http://support.iatistandard.org/entries/106937796-Humanitarian-Flag>`__.  

2.01
^^^^
| The ``version`` attribute was `removed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#iati-activity-removed-attribute>`__.  

1.02
^^^^
| Introduced the ``linked-data-uri`` attribute on iati-activity element



