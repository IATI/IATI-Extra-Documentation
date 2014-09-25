Example Usage
~~~~~~~~~~~~~
Example usage of ``iati-organisations``.

| This element is a parent for other all other elements of the **IATI Organisation Standard**.

| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``@generated-datetime`` attribute.  
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example dateTime format conforms to the *xsd:dateTime* standard.

| The ``@version`` attribute declares a valid code (*2.01*) from the *Version* codelist.

.. literalinclude:: organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisations starts-->
	:end-before: <!--iati-organisation starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisation ends-->	
	:end-before: <!--iati-organisations ends-->
	
Changelog
~~~~~~~~~

This element has not been changed.
