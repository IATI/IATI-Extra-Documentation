Example Usage
~~~~~~~~~~~~~
Example usage of  ``iati-organisation``.

| This element is a parent for other child elements.

| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``@last-updated-datetime`` attribute.  
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example dateTime format conforms to the *xsd:dateTime* standard.

| The ``@xml:lang`` attribute declares a valid code (*en*) from the *Language* codelist.
| The ``@default-currency`` attribute declares a valid code (*EUR*) from the *Currency* codelist.

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisation starts-->
	:end-before: <!--organisation-identifier starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-country-document-link ends-->	
	:end-before: <!--iati-organisation ends-->

Changelog
~~~~~~~~~

This element has not been changed.
