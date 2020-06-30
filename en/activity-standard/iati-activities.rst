Example Usage
~~~~~~~~~~~~~
Example usage of ``iati-activities``.

| This element is a parent for other all other elements of the **IATI Activity Standard**.

| This example provides a dateTime of *2014-09-10T07:15:37Z*  for the ``@generated-datetime`` attribute.
| A dateTime in UTC time is indicated by adding a *Z* behind the time
| This example date time format conforms to the *xsd:dateTime* standard.

| The ``@version`` attribute declares a valid code (*2.x*) from the *Version* codelist.
| The optional ``@linked-data-default`` attribute is also included.

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
Introduced the ``@linked-data-default`` attribute on ``iati-activities`` element

.. meta::
  :order: 0
